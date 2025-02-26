## API Reference

### Authentication

All API requests must include an authentication token.

```bash
Authorization: Bearer YOUR_ACCESS_TOKEN
```

### Endpoints

#### 1. Get All Shifts

```http
GET /api/shifts
```

**Response:**

```json
{
  "shifts": [{ "id": 1, "employee": "John Doe", "time": "08:00 - 16:00" }]
}
```

#### 2. Create a Shift

```http
POST /api/shifts
```

**Request Body:**

```json
{
  "employee_id": 123,
  "time": "08:00 - 16:00"
}
```

#### 3. Update a Shift

```http
PUT /api/shifts/{shift_id}
```
