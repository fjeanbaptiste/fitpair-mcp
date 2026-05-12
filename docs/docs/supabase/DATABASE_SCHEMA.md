# FitPair Database Schema

## Users Table
| Field | Type |
|---|---|
| id | UUID |
| username | text |
| email | text |
| password_hash | text |
| age_range | text |
| city | text |
| bio | text |
| profile_photo | text |
| created_at | timestamp |

---

## Interests Table
| Field | Type |
|---|---|
| id | UUID |
| interest_name | text |

Examples:
- Gym
- Running
- Hiking
- Yoga
- Basketball
- Wellness
- Coffee Walks

---

## User_Interests Table
| Field | Type |
|---|---|
| id | UUID |
| user_id | UUID |
| interest_id | UUID |

---

## Matches Table
| Field | Type |
|---|---|
| id | UUID |
| user_1 | UUID |
| user_2 | UUID |
| matched_at | timestamp |

---

## Messages Table
| Field | Type |
|---|---|
| id | UUID |
| sender_id | UUID |
| receiver_id | UUID |
| message_text | text |
| created_at | timestamp |

---

## Events Table
| Field | Type |
|---|---|
| id | UUID |
| title | text |
| description | text |
| city | text |
| event_date | timestamp |
| created_by | UUID |

---

## Reports Table
| Field | Type |
|---|---|
| id | UUID |
| reported_user | UUID |
| reporter_user | UUID |
| reason | text |
| created_at | timestamp |
