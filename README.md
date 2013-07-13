Art
===
import Gui3

def main():

   win = Gui3.Gui()
   title = input('what should we call this work of art?')
   win.title(title)
   width = int(input('How wide would you like it to be?'))
   ht = int(input( 'How tall would you like it to be?'))
   
   size = width

   canvas = win.ca(size + 50, ht + 50)

   canvas.rectangle([[-size/2, -ht/2], [size/2, ht/2]], fill='yellow' )

   canvas.oval([[-size/2, -ht/2], [size/2, ht/2]], fill='green' )

   canvas.polygon([[-size/2, 0], [0, ht/2], [size/2, 0], [0, -ht/2]],
      outline='black', fill='white')
   
   win.mainloop()

main()
