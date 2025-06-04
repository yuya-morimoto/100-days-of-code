# 100 Days Of Code - Log

## Day 15: June 4, 2025

### Today's Progress

- User メタデータのマッピングクラス・ユースケースを実装

### Thoughts

- `omitempty`を利用するかどうか、良いところがいまいちわかっていないのでまた調査しよう。

### Link or Image to work

```go
type UserPrivateMetadata struct {
	Birthday             string `json:"birthday,omitempty"`
	IsBirthdayVisibility bool   `json:"is_birthday_visibility,omitempty"` // boolのゼロ値はfalseなので、omitemptyの挙動に注意
	Gender               string `json:"gender,omitempty"`
	CreatedAt            string `json:"created_at,omitempty"` // UTCタイムスタンプ (RFC3339形式)
}
```
