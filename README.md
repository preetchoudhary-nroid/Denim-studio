Denim Studio
A handcrafted denim clothing store based in Delhi, India. This is the official e-commerce website for Denim Studio — featuring handmade clothes, custom orders, and embroidery work on shirts, pants, jackets, t-shirts, and accessories.

About the Store
Denim Studio is a Delhi-based clothing brand that specializes in handmade denim and fabric garments. Every piece is cut, stitched, and finished by hand in our Delhi studio. We offer full customization — from fit and wash to hand and machine embroidery — on all our products.

Features

Browse full product catalog — jeans, jackets, shirts, shorts, and accessories
Filter products by category
Product detail page with size selector
Add to cart and manage cart items
UPI checkout with QR code — supports GPay, PhonePe, Paytm, and all UPI apps
After payment, customers submit their UTR/Transaction ID which is sent directly to WhatsApp for order confirmation
About page with brand story
Contact form
Fully responsive design


Tech Stack
LayerTechnologyFrontendHTML, CSS, JavaScriptDatabase & AuthSupabasePaymentsUPI (QR Code via 8448369385@fam)Image HostingCloudinaryHostingVercelDomainNamecheap

Project Structure
denim-studio/
├── index.html        # Main website 
├── README.md         # This file

Pages

Home — Hero banner, featured collection, brand values
Shop — Full product grid with category filters
Product Detail — Image, description, size selector, add to cart
Cart — Item list, subtotal, shipping, checkout button
Checkout — Shipping form, UPI QR code, UTR submission
About — Brand story, what we do, our promise
Contact — Inquiry form


Payment Flow

Customer adds items to cart and proceeds to checkout
Customer fills in contact and shipping details
A UPI QR code is generated for the exact order amount
Customer scans the QR or taps "Open UPI App Directly"
Customer pays via any UPI app
Customer enters their UTR / Transaction ID
On clicking "Pay & Place Order", details are sent to WhatsApp automatically
Store owner verifies payment and confirms the order


Setup & Deployment
1. Clone the repo
bashgit clone https://github.com/preetchoudhary-nroid/denim-studio.git
cd denim-studio
2. Deploy to Vercel

Push the repo to GitHub
Go to vercel.com and import the project
Select the repo and click Deploy
Done — live in under a minute

3. Connect Custom Domain (Namecheap)

Add your domain in Vercel → Project Settings → Domains
In Namecheap DNS, add:

A record → 76.76.19.61
CNAME www → cname.vercel-dns.com



4. Image Hosting (Cloudinary)
Product images are hosted on Cloudinary under cloud name dzhdwb2zl. To add new product images:

Upload the image to Cloudinary
Copy the secure_url
Add it to the products array in index.html as the img field


Customization
To add or edit products, find the products array in the <script> section of index.html:
javascript{
  id: 1,
  name: 'Product Name',
  cat: 'jacket',         // jeans | jacket | shirt | shorts | accessory
  price: 2499,
  badge: 'New',          // New | Bestseller | Limited | '' (empty for none)
  img: 'https://your-cloudinary-url.jpg',
  desc: 'Product description here.'
}

Contact

WhatsApp: +91 84483 69385
Email: hello@denimstudio.in
Location: Delhi, India


License
This project is private and intended for personal commercial use by Denim Studio, Delhi.
