# Boston Parking Regulations Digitization Project

## Project Overview
This project aims to create a comprehensive digital map of parking regulations in Boston by automatically processing street sign imagery and location data. The system processes street-level imagery to identify parking signs, extracts regulations from these signs, and maps them to specific curb zones.

## System Components
1. Data Collection
   - Integration with Panorama API for street-level imagery
   - Identification and mapping of sign locations
   - Definition and tracking of curb zones

2. Computer Vision Processing
   - Sign detection in street-level imagery
   - Text extraction from identified signs
   - Classification of sign types and regulations

3. Policy Engine
   - Extraction of rules from sign text
   - Assignment of regulations to specific curb zones
   - Handling of time-based and conditional regulations

4. API Layer
   - Data access endpoints for regulation queries
   - Integration capabilities for external systems
   - Zone-based regulation lookup

## Getting Started

### Prerequisites
- Python 3.8+
- Access to Panorama API
- Required API keys and credentials

### Installation
1. Clone the repository
```bash
git clone https://github.com/bostonsam617/boston-parking.git
cd boston-parking
```

2. Set up virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scriptsctivate
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

### Configuration
1. Copy the example environment file
```bash
cp .env.example .env
```

2. Update the `.env` file with your API keys and configuration

## Project Structure
```
boston-parking/
├── src/
│   ├── data_collection/      # Panorama API integration and data gathering
│   ├── computer_vision/      # Sign detection and text extraction
│   ├── policy_engine/        # Rule processing and zone assignment
│   └── api/                  # API endpoints and schemas
├── tests/                    # Unit and integration tests
├── docs/                     # Documentation
└── scripts/                  # Utility scripts
```

## Development Process
1. Each component is developed independently
2. Integration tests ensure components work together
3. Continuous validation against known parking regulations

## Contributing
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## Current Status
- [ ] Initial project setup
- [ ] Panorama API integration
- [ ] Basic sign detection
- [ ] Text extraction system
- [ ] Rule processing engine
- [ ] API development
- [ ] Documentation

## License
This project is licensed under the MIT License - see the LICENSE file for details.
