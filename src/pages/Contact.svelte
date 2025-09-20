<div class="contact-tab">
  <h2 style="padding-top: 2vh; padding-bottom: 2vh;">Contact</h2>

  <!-- Social links -->
  <div class="contact-links">
    <a style="font-size: 2.7vh;" href="https://www.linkedin.com/in/eric-gutierrez-moreno" target="_blank" rel="noopener">
      <i class="bi bi-linkedin"></i> LinkedIn
    </a>
    <a style="font-size: 2.7vh;" href="https://github.com/ericGutierrezM" target="_blank" rel="noopener">
      <i class="bi bi-github"></i> GitHub
    </a>
  </div>

  <!-- Contact form -->
  <form action="mailto:gh.ericgutierrez@gmail.com" method="post" enctype="text/plain" style="font-size: 2.3vh;">
    <input type="text" name="name" placeholder="Your Name" required style="font-size: 2.2vh;"/>
    <input type="email" name="email" placeholder="Your Email" required style="font-size: 2.2vh;"/>
    <textarea name="message" placeholder="Your Message" rows="5" required style="font-size: 2.2vh;"></textarea>
    <button type="submit" style="font-size: 2.3vh;">Send</button>
  </form>
</div>

<style>
  .contact-tab {
    width: 100%;
    max-width: 500px;
    margin: 0 auto;
    text-align: center;
  }

  .contact-links {
    margin-bottom: 1.5rem;
    display: flex;
    justify-content: center;
    gap: 1.5rem;
    font-size: 1.1rem;
  }

  .contact-links a {
    text-decoration: none;
    color: #333;
    font-weight: 500;
  }

  .contact-links a:hover {
    color: rgb(1, 121, 51); /* accent color */
  }

  form {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  input, textarea {
    padding: 0.8rem;
    border-radius: 8px;
    border: 1px solid #ccc;
    font-size: 1rem;
    width: 100%;
  }

  button {
    background-color: rgb(0, 54, 23);
    color: white;
    border: none;
    padding: 0.8rem;
    border-radius: 8px;
    cursor: pointer;
    font-size: 1rem;
    font-weight: bold;
  }

  button:hover {
    background-color: rgb(1, 121, 51);
  }
</style>