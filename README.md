# Poniendo en marcha el entorno local

Este sitio está construído usando
[jekyll](http://jekyllrb.com/). Jekyll necesita una versión reciente
de ruby que podemos instalarla usando [rvm](https://rvm.io/):

	$ \curl -sSL https://get.rvm.io | bash -s stable --ruby

Además, para que funcione es necesario tener una versión reciente de
nodejs. Podemos instalarla con:

	$ sudo apt-get install nodejs

O utilizar [nvm](https://github.com/creationix/nvm).

# Activando ruby

	$ bash --login
	$ rvm use default

# Clonar el repo

	$ git clone https://github.com/tryton-ar/tryton-ar.github.io.git

# Instalar las dependencias.

	$ gem install bundler
	$ cd tryton-ar.github.io/
	$ bundle install

# Correr el servidor local

	$ jekyll serve --watch

Así nos dirigimos a `http://localhost:4000` para ver como van quedando
los cambios que estamos haciendo.

# Editando...

Las páginas son archivos markdown que reciden en la carpeta inicial. Los noticias (post) están dentro de la carpeta `_post` o se pueden crear con:

	$ rake new_post[titulo]
