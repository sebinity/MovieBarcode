# MovieBarcode
Generate movie Barcode in python. Forked from Thomas Poulet, read his blog post here: https://blog.thomaspoulet.fr/posts/how-to-generate-movie-barcodes/. The movie barcode is an extract of the dominant color of every frame. Condensed in one image it can show the mood of the film.

## Usage

1. Install python3 from here https://www.python.org/downloads/
2. Install dependencies:
   * python3 -m pip install numpy
   * python3 -m pip install tqdm
   * python3 -m pip install opencv-python
  
3. Download all three .py files and save them in a folder together with your desired movie
4. Script accepts the following options:
   * -f: Input video path (default: input.mp4)
   * -m: Method for extracting dominant color (mean, hsv, rgb, kmean) — default is hsv
   * -t: Start timestamp (in milliseconds) — default: 0
   * -w: Desired width of output image (i.e., how many frames to sample) — default: all frames
  
## Example usage
python3 VideoMood.py -f Wish.mp4 -m kmean -t 0 -w 1000

## Results

Toy Story (1995)
![hsv_toystory](https://cloud.githubusercontent.com/assets/1039134/11017234/53136f92-8599-11e5-9c2a-854e8652045f.jpg)

Aladdin (1992)
![hsv_aladdin](https://cloud.githubusercontent.com/assets/1039134/11017235/5319ac2c-8599-11e5-94ef-3708967dee55.jpg)

