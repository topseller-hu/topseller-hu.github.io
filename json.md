Csillaggal jelölt mezők megadása kötelező.

- id*  
Típus: integer, string  
Termék azonosítója.

- name*  
Típus: string  
Termék neve.

- description  
Típus: string  
Termék leírása.

- price*  
Típus: integer  
Termék ára áfával.

- discount_price  
Típus: integer  
Termék akciós ára áfával.

- images  
Típus: string-array  
Termék képei listában.

- category*  
Típus: object  
Termék kategóriája.

  - id*  
Típus: integer, string  
Termék kategóriájának azonosítója.

  - name*  
Típus: string  
Termék kategóriájának legalsó neve.

  - route
  Típus: string
  Termék kategóriájának elérési útvonala.

- attributes  
Típus: object-array  
Termék tulajdonságai.

  - id  
  Típus: integer, string  
  Termék tulajdonságnak azonosítója.
  
  - name  
  Típus: string  
  Termék tulajdonságnak a neve.
  
  - value  
  Típus: integer, string, boolean  
  Termék tulajdonságnak az értéke.


```json
[
	{
		"id": 123,
		"name": "Teszt termék",
		"description": "Teszt termék leírása",
		"price": 27000,
		"discount_price": 20000,
		"images": [
			"https://example.com/product-image1.jpg",
			"https://example.com/product-image2.png"
		],
		"category": {
			"id": 123,
			"name": "Teszt kategória",
			"route": "Fő teszt kategória / Al teszt kategória / Teszt kategória"
		},
		"attributes": [
			{
				"id": 123,
				"name": "Szín",
				"value": "fekete"
			},
			{
				"id": 124,
				"name": "Hosszúság (cm)",
				"value": 27
			},
			{
				"id": 125,
				"name": "Mosható",
				"value": false
			}
		]
	}
]
```
