import pandas as pd

# Örnek Spotify verisi
data = {
    "track_name": ["Song A", "Song B", "Song C", "Song D", "Song E"],
    "artist": ["Artist 1", "Artist 2", "Artist 3", "Artist 4", "Artist 5"],
    "play_count": [120, 340, 290, 150, 410]
}

# DataFrame oluştur
df = pd.DataFrame(data)

# İlk 5 satırı göster
print("İlk 5 satır:")
print(df.head())

# En çok dinlenen şarkıları sırala
top_tracks = df.sort_values(by="play_count", ascending=False)

print("\nEn çok dinlenen şarkılar:")
print(top_tracks)
