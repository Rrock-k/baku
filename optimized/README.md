Пример настроек сжатия:
ffmpeg -y -i bouquet.mp4 -c:v libx264 -crf 32 -preset medium -c:a aac -b:a 32k optimized/bouquet_optimized.mp4

Создание постера (первый кадр видео):
ffmpeg -y -i video.mp4 -vframes 1 -q:v 2 optimized/poster.jpg
