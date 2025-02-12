# Boston Parking Regulations Digitization Project

## Project Overview
This project aims to create a comprehensive digital map of parking regulations in Boston by automatically processing street sign imagery and location data. The system processes street-level imagery to identify parking signs, extracts regulations from these signs, and maps them to specific curb zones.

## System Components
1. Mapping Curb Zones
   - Integration with Cartegraph or Civis for sign location datas
   - Filtering out non-parking regulations signs
   - Plot all street signs
   - Turning sign plots into curb zone polygons

2. Computer Vision Processing
   - Integration with Panorama API for street-level imagery
   - Text extraction from identified signs
   - Classification of sign types and regulations

3. Policy Engine
   - Extraction of rules from sign text
   - Assignment of regulations to specific curb zones
   - Handling of time-based and conditional regulations

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
│   ├── curb_zone_mapping     # Creating curb zone polygons
│   ├── computer_vision/      # Panorama API integration andSign detection and text extraction
│   ├── policy_engine/        # Rule processing and zone assignment
│   └── api/                  # API endpoints and schemas
├── tests/                    # Unit and integration tests
├── docs/                     # Documentation
└── scripts/                  # Utility scripts
```




## Current Status
- [x] Initial project setup
- [ ] Panorama API integration
- [ ] Rules extraction system
- [ ] Policy engine
- [ ] Curb Zone Mapping
- [ ] Documentation

## License
This project is licensed under the MIT License - see the LICENSE file for details.
