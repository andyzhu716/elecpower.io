---
title: "Contact"
description: "Contact Shuai Zhu for busbar-related product discussion, power project support and business communication."
---

<style>
.contact-form-wrapper {
  max-width: 600px;
  margin: 0 auto;
  padding: 2rem;
  background: #f8f9fa;
  border-radius: 12px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.1);
}

.contact-form-wrapper h3 {
  margin-bottom: 1.5rem;
  color: #333;
  text-align: center;
}

.form-group {
  margin-bottom: 1.25rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 600;
  color: #555;
}

.form-group label .required {
  color: #dc3545;
}

.form-control {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #ddd;
  border-radius: 6px;
  font-size: 1rem;
  transition: border-color 0.2s, box-shadow 0.2s;
}

.form-control:focus {
  outline: none;
  border-color: #007bff;
  box-shadow: 0 0 0 3px rgba(0,123,255,0.15);
}

select.form-control {
  cursor: pointer;
}

textarea.form-control {
  min-height: 120px;
  resize: vertical;
}

.btn-submit {
  width: 100%;
  padding: 1rem;
  background: linear-gradient(135deg, #007bff 0%, #0056b3 100%);
  color: white;
  border: none;
  border-radius: 6px;
  font-size: 1.1rem;
  font-weight: 600;
  cursor: pointer;
  transition: transform 0.2s, box-shadow 0.2s;
}

.btn-submit:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0,123,255,0.4);
}

.contact-info-box {
  margin-top: 2rem;
  padding: 1.5rem;
  background: white;
  border-radius: 8px;
  border-left: 4px solid #007bff;
}

.contact-info-box h4 {
  margin-bottom: 1rem;
  color: #333;
}

.contact-item {
  display: flex;
  align-items: flex-start;
  margin-bottom: 0.75rem;
}

.contact-item i {
  width: 24px;
  margin-right: 0.75rem;
  color: #007bff;
}

.contact-item a {
  color: #007bff;
  text-decoration: none;
}

.contact-item a:hover {
  text-decoration: underline;
}

.privacy-note {
  text-align: center;
  margin-top: 1rem;
  color: #6c757d;
  font-size: 0.9rem;
}

/* 响应式调整 */
@media (max-width: 768px) {
  .contact-form-wrapper {
    padding: 1.5rem;
    margin: 0 1rem;
  }
}
</style>

<div class="row">
  <div class="col-12">
    <p class="lead mb-4">
      For business communication related to busbar products, power plant applications, or project support, please use the form below or contact us directly.
    </p>
  </div>
</div>

<div class="row">
  <!-- Contact Form -->
  <div class="col-lg-8">
    <div class="contact-form-wrapper">
      <h3>Send Us a Message</h3>
      
      <!-- Formspree Form -->
      <!-- TODO: Replace FORMSPREE_ID with your actual Formspree form ID -->
      <form action="https://formspree.io/f/mqeynvdb" method="POST">
        
        <!-- Name -->
        <div class="form-group">
          <label for="name">
            Name <span class="required">*</span>
          </label>
          <input 
            type="text" 
            id="name" 
            name="name" 
            class="form-control" 
            required
            placeholder="Your full name"
          >
        </div>
        
        <!-- Email -->
        <div class="form-group">
          <label for="email">
            Email <span class="required">*</span>
          </label>
          <input 
            type="email" 
            id="email" 
            name="email" 
            class="form-control" 
            required
            placeholder="your@email.com"
          >
        </div>
        
        <!-- Company -->
        <div class="form-group">
          <label for="company">Company</label>
          <input 
            type="text" 
            id="company" 
            name="company" 
            class="form-control"
            placeholder="Your company name (optional)"
          >
        </div>
        
        <!-- Phone -->
        <div class="form-group">
          <label for="phone">Phone / WhatsApp</label>
          <input 
            type="tel" 
            id="phone" 
            name="phone" 
            class="form-control"
            placeholder="+1 234 567 8900 (optional)"
          >
        </div>
        
        <!-- Subject -->
        <div class="form-group">
          <label for="subject">
            Subject <span class="required">*</span>
          </label>
          <select id="subject" name="subject" class="form-control" required>
            <option value="" selected disabled>Select a subject</option>
            <option value="quote">Request for Quote</option>
            <option value="technical">Technical Support</option>
            <option value="partnership">Partnership Inquiry</option>
            <option value="general">General Inquiry</option>
          </select>
        </div>
        
        <!-- Message -->
        <div class="form-group">
          <label for="message">
            Message <span class="required">*</span>
          </label>
          <textarea 
            id="message" 
            name="message" 
            class="form-control" 
            rows="5" 
            required
            placeholder="Please describe your inquiry in detail..."
          ></textarea>
        </div>
        
        <!-- Spam protection (honeypot) -->
        <input type="text" name="_gotcha" style="display:none">
        
        <!-- Submit Button -->
        <button type="submit" class="btn-submit">
          Send Message
        </button>
        
        <p class="privacy-note">
          Your information will be kept confidential and used only for responding to your inquiry.
        </p>
      </form>
    </div>
  </div>
  
  <!-- Contact Info -->
  <div class="col-lg-4">
    <div class="contact-info-box">
      <h4>Direct Contact</h4>
      
      <div class="contact-item">
        <i class="fas fa-user"></i>
        <div>
          <strong>Andy Zhu (朱帅)</strong><br>
          Customer Manager
        </div>
      </div>
      
      <div class="contact-item">
        <i class="fas fa-building"></i>
        <div>
          <strong>Wetown Electric Group</strong><br>
          <a href="https://www.wetown.com/" target="_blank" rel="noopener">www.wetown.com</a>
        </div>
      </div>
      
      <div class="contact-item">
        <i class="fas fa-envelope"></i>
        <div>
          <strong>Email</strong><br>
          <a href="mailto:andyzhu716@gmail.com">andyzhu716@gmail.com</a>
        </div>
      </div>
      
      <div class="contact-item">
        <i class="fas fa-phone"></i>
        <div>
          <strong>Phone / WhatsApp</strong><br>
          <a href="tel:+8613805291038">+86 138 0529 1038</a>
        </div>
      </div>
      
      <div class="contact-item">
        <i class="fab fa-linkedin"></i>
        <div>
          <strong>LinkedIn</strong><br>
          <a href="https://www.linkedin.com/in/andy-zhu-2ba4ba356/" target="_blank">Andy Zhu</a>
        </div>
      </div>
    </div>
  </div>
</div>
