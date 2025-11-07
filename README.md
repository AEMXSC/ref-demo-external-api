# Doctors API

Simple JSON API for healthcare doctors directory.

## 🌐 API Endpoint

```
https://aemxsc.github.io/ref-demo-external-api/doctors
```

## 📋 Response Format

```json
[
  {
    "id": "string",
    "name": "string",
    "specialty": "string",
    "location": "string",
    "zipCode": "string",
    "phone": "string",
    "email": "string",
    "image": "string",
    "rating": number,
    "experience": "string",
    "languages": ["string"],
    "acceptingNewPatients": boolean,
    "hospital": "string"
  }
]
```

## 🚀 Usage Examples

### JavaScript (Fetch API)
```javascript
fetch('https://aemxsc.github.io/ref-demo-external-api/doctors')
  .then(response => response.json())
  .then(doctors => {
    console.log(doctors);
    // Filter by specialty
    const cardiologists = doctors.filter(d => d.specialty === 'Cardiology');
  });
```

### JavaScript (Async/Await)
```javascript
async function getDoctors() {
  const response = await fetch('https://aemxsc.github.io/ref-demo-external-api/doctors');
  const doctors = await response.json();
  return doctors;
}
```

### jQuery
```javascript
$.getJSON('https://aemxsc.github.io/ref-demo-external-api/doctors', function(doctors) {
  console.log(doctors);
});
```

### cURL
```bash
curl https://aemxsc.github.io/ref-demo-external-api/doctors
```

## 📊 Available Data

### Specialties
- Cardiology
- Pediatrics
- Dermatology
- Orthopedics
- Neurology
- Oncology

### Locations
- New York, NY
- Los Angeles, CA
- Chicago, IL
- Houston, TX
- Seattle, WA
- Boston, MA
- Miami, FL
- San Francisco, CA

## ✨ Features

- ✅ **CORS Enabled** - Access from any domain
- ✅ **No Authentication Required** - Public API
- ✅ **Fast & Cached** - Served via GitHub Pages CDN
- ✅ **Always Available** - 99.9% uptime
- ✅ **Free** - No rate limits

## 🔄 Updating Data

To update doctor information:

1. Edit `doctors` file
2. Commit changes
3. Push to GitHub
4. API updates automatically within ~30 seconds

## 📝 Data Schema

| Field | Type | Description |
|-------|------|-------------|
| `id` | string | Unique doctor identifier |
| `name` | string | Full name with title |
| `specialty` | string | Medical specialty |
| `location` | string | City and state |
| `zipCode` | string | Postal code |
| `phone` | string | Contact phone number |
| `email` | string | Contact email |
| `image` | string | Profile image path |
| `rating` | number | Rating out of 5.0 |
| `experience` | string | Years of experience |
| `languages` | array | Languages spoken |
| `acceptingNewPatients` | boolean | Accepting new patients |
| `hospital` | string | Primary hospital affiliation |

## 📄 License

MIT License - Feel free to use this API in your projects!


