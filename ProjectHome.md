presentex is a command-line tool that allows users to easily produce high-quality, colourful equations with LaTeX for use in presentations, etc. It is written in Python and uses LaTeX, dvips, and imagemagick. It should run on Linux/UNIX/Mac systems (not sure about Windows), provided the appropriate software packages are installed.

USAGE:

from the command line
> $ presentex 'latex equation in quotes' [options](options.md)

> Options are:

> -f -fg --foreground: Foreground (text) colour, reported as 'r,g,b'
> > (quotes are required) where r,g,b can span the
> > integeer values [0,255]. The default is
> > '0, 0, 0'.


> -b -bg --background: Background color, reported as 'r,g,b' (quotes are
> > required) where r,g,b can span the integer values
> > [0,255]. The default is '255, 255, 255'.


> -e --enlargement:    Enlargement factor. The default is "1".

> -o --output: Name of output file. Extension (.jpg, .gif, .png, etc.)
> > will be interpreted by Imagemagick. Note that
> > transparency does not work for all image types,
> > but it does work for pngs and gifs. The default
> > is "./eqn.png"


> -t --transparent: Option for a transparent background.

> -h --help: Produces this help window

> -v -a --version --about: Gets information on present version

> -i --install: Gives help about setting up presentex on your computer.

> EXAMPLES:

> presentex '\gamma = \displaystyle{\frac{\mathcal{A}}{g\delta\sin^2\phi}}' -fg '190,75,75' -bg '200,200,200' -o 'gamma.jpg'

> presentex -t -o 'pi.gif' -e 3 '\pi = 3.14159\dots' -fg 200,20,20 -t
