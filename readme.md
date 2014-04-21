
# animated gif

record with ishowu

commands
  mplayer -ao null -endpos 5 -vo png:outdir=. iShowU-Capture.mov 
  mogrify -format gif *.png
  gifsicle --colors=64 --delay=4 --loopcount=0 -O3 *.gif > animation.gif