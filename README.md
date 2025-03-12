Here’s a basic structure for the document you can use for the "Kareli Amul Parlour" online product availability application:

---

### Kareli Amul Parlour - Online Product Availability Application

#### 1. Introduction

The "Kareli Amul Parlour" online product availability application is designed to provide real-time product availability updates and facilitate easy communication with customers. The application integrates with WhatsApp API for direct communication and uses AWS services for hosting and managing the application.

---

#### 2. Technologies Used

- **HTML**: Structure and layout of the application.
- **CSS**: Styling and design of the application.
- **JavaScript**: Functionality to fetch and display the product availability dynamically.
- **WhatsApp API**: Integration for customer communication via WhatsApp.

---
 
#### 3. AWS Services Used

1. **Amazon S3 Bucket**:  
   - The application files (HTML, CSS, JavaScript, images) are stored in an S3 bucket for reliable and scalable storage.
   - The bucket is configured for static website hosting.

2. **Amazon Route 53**:  
   - Route 53 is used for DNS management to route user requests to the correct location (S3 bucket hosting).

3. **DNS Mapping**:  
   - DNS mapping is configured to map the custom domain (e.g., `www.kareliamulparlour.com`) to the S3 bucket hosting the application.

4. **DNS Registration**:  
   - DNS registration is handled through Route 53 for proper domain setup and management.

---

#### 4. Application Features

- **Product Availability**:  
  Displays the availability status of Amul products in real time.

- **Dynamic Product List**:  
  The list of products can be dynamically updated via JavaScript. The availability status is fetched and updated regularly.

- **WhatsApp Integration**:  
  - Customers can send a WhatsApp message directly to inquire about product details or place orders.
  - The WhatsApp API allows for easy integration, providing a smooth customer interaction experience.

---

#### 5. WhatsApp API Integration

- The application uses WhatsApp API for easy customer interaction. When the customer clicks the "Contact us on WhatsApp" button, they will be redirected to a WhatsApp chat with a pre-filled message.
- The WhatsApp API URL format:  
  `https://wa.me/<phone_number>?text=<message>`

---

#### 6. Hosting and Configuration

1. **AWS S3 Bucket**:  
   - Create an S3 bucket and upload your website files (HTML, CSS, JavaScript).
   - Enable static website hosting in the bucket settings.

2. **Route 53 Configuration**:  
   - Set up a hosted zone in Route 53 for your custom domain.
   - Create a record set to point to the S3 bucket endpoint.

3. **DNS Registration**:  
   - Register your domain name via AWS or any third-party domain registrar.
   - Update the domain's DNS settings to point to the Route 53 hosted zone.

---

