# Shopify

This is the [Developer Intern Challenge](https://docs.google.com/document/d/1ZKRywXQLZWOqVOHC4JkF3LqdpO3Llpfk_CkZPR8bjak/edit) for SU21 Internships. This online repository was made with flask and sqlite3 and allows for the buying and selling (singly and in bulk) of images at various prices set by the user. It is written as an application for a store owner, so you can buy images at a wholesale price and sell them at your selling price. You can also add and remove images as you see fit, and edit pricing information.

To run, simply clone the repository, install flask and sqlite3 if necessary and run `python main.py`. This will host the web application, most likely at `http://127.0.0.1:5000/`. Then images can be bought and sold as expected. The `images.db` file will contain the image information, including its prices, the name and a path to the image itself. This project is a database because whenever and image is added, it is copied to the `static/images` directory, where it can also be removed if so desired.

The application logic allows users to sell their images to customers, but only if they have the required stock. There are also checks to make sure prices for images are never negative, though you can go in debt since there is no restriction on how much you buy from wholesalers.

# Future Extensions
Future extensions could include permissions and the uploading of large numbers of different images. The application could also allow store managers to get useful statistics on their products, like the most and least popular images. This could be also extended to allow for permissions for who is allowed to add and delete images. However this does constitute a Minimum Viable Product.
