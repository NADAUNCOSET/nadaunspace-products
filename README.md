# nadaunspace-products

NADAUN 블로그스팟(Blogspot) 신상품 자동 동기화용 정적 JSON 저장소.

- **소스**: 아임웹 REST API V2 (`rainbowshop.imweb.me`)
- **갱신**: NAS `nadaun-scheduler` 컨테이너가 20분 주기로 푸시
- **소비**: Blogger 테마(`https://nadaunspace.blogspot.com/`)가 raw URL을 직접 fetch (CORS 허용)

## raw URL
```
https://raw.githubusercontent.com/NADAUNCOSET/nadaunspace-products/main/latest_products.json
```

## JSON 스키마
```json
{
  "updated_at": "ISO8601 KST",
  "count": 12,
  "products": [
    { "id": "...", "title": "...", "url": "...", "image": "...", "price": "...", "registered_at": "" }
  ]
}
```
