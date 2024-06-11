Predict conversion rate
The goal of the competition is to predict the **conversion rate** of a product on a given day. The training dataset contains data on all products of our top 10 categories for January 2020. The test dataset contains data for February 2020 (until Feb 11).

One row = one product on one given day

s_date, s_product : primary key
s_brand: brand of the product
s_family: highest level category on the website (Gardening, Tools, …)
s_lowest_category: lowest level category on the website (Drills, swimming pools, …)
s_provider: seller of the product
s_retail_price: observed retail price
s_shipping_time: estimated shipping time
s_weight: weight of the product
m_nb_ratings: number of ratings of the product
m_avg_rating: average rating of the product
m_has_pdf: product has a pdf documentation
m_length_description: length of the product description
m_unit_price_vat_inc: product price including VAT
m_nb_images: number of images of the product on the website
m_total_vu: number of views of the product page (not present in test set)
conversion_rate : m_total_transaction / m_total_vu (our target not present in test set)
Note that you can access the number of orders by multiplying m_total_vu and conversion_rate

