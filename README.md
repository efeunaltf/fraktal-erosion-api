# Fraktal Erozyon Analizi API

Bu proje, fraktal boyut analizi kullanarak toprak erozyonu riskini değerlendiren bir FastAPI uygulamasıdır.

## Özellikler

- Fraktal boyut hesaplama
- Erozyon riski değerlendirmesi
- Toprak türüne göre ağaç önerileri
- Harita görselleştirme
- RESTful API

## Kurulum

```bash
pip install -r requirements.txt
```

## Çalıştırma

```bash
uvicorn main:app --host 0.0.0.0 --port 8000
```

## API Endpoints

- `GET /`: Ana sayfa
- `POST /analyze`: Erozyon analizi
- `GET /health`: Sağlık kontrolü

## Kullanım

Erozyon analizi için POST isteği:

```json
{
  "latitude": 41.0082,
  "longitude": 28.9784,
  "soil_type": "kumlu",
  "rainfall": 800
}
```

## Teknolojiler

- FastAPI
- NumPy
- Matplotlib
- Selenium
- Folium
- scikit-image
