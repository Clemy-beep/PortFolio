<div id="contact">
  <form action="mailto:clementine.digny@gmail.com">
    <h2><span class="material-symbols-outlined"> edit </span>Write me !</h2>
    <div class="names">
      <input
        type="text"
        name="first_name"
        id="first_name"
        placeholder="First name"
        required
      />
      <input
        type="text"
        name="last_name"
        id="last_name"
        placeholder="Last name"
        required
      />
    </div>
    <div class="obj">
      <div class="email">
        <input
          type="email"
          name="email"
          id="email"
          placeholder="Email"
          required
        />
      </div>
      <div class="subject">
        <input
          type="text"
          name="subject"
          id="subject"
          placeholder="Subject"
          required
        />
      </div>
    </div>
    <div class="message">
      <textarea
        name="body"
        id="body"
        cols="30"
        rows="10"
        placeholder="Message"
        required
      />
    </div>
    <div class="submit">
      <input type="submit" value="Send your message" />
    </div>
  </form>
  <div class="social-medias">
    <h2>Where to find me ?</h2>
    <div class="social-media">
      <img src="/images/github.png" alt="github" />
      <a href="http://github.com/Clemy-beep">Github/Clemy-beep</a>
    </div>
    <div class="social-media">
      <img src="/images/linkedin.png" alt="linkedin" />
      <a href="https://www.linkedin.com/in/cl%C3%A9mentine-digny-04237b22a/"
        >LinkedIn/Clementine-Digny</a
      >
    </div>
  </div>
</div>
<span
  >design inspired by this portofolio: <a
    href="https://www.figma.com/@elalfredo?fuid=1039551130019007141"
    >@el_alfredo</a
  ></span
>

<style>
  #contact {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    flex-wrap: wrap;
    padding-bottom: 2em;
  }

  form {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 0.5em;
    width: 40%;
    height: fit-content;
  }
  .names,
  .obj {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    gap: 2em;
  }

  input,
  textarea {
    border: none;
    background-color: transparent;
    display: block;
  }

  h2 {
    text-align: center;
    font-size: 2em;
    background: linear-gradient(
      90deg,
      #bff4a6 0.11%,
      #ed7fc0 36.71%,
      #00ffa3 79.97%
    );
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  textarea {
    resize: none;
    width: 100%;
    height: 7em;
    border-style: solid;
    border-width: 2ps;
    border-color: transparent transparent #bff4a6 transparent;
  }

  #first_name {
    border-bottom: 2px solid #eb34a0;
  }

  #last_name {
    border-bottom: 2px solid #c0a2ff;
  }

  #email {
    border-bottom: 2px solid #8effd6;
  }

  #subject {
    border-bottom: 2px solid #d355ff;
  }

  input[type="submit"] {
    display: block;
    font-size: 1.5em;
    font-weight: 700;
    background: linear-gradient(
      90deg,
      #00ffa3 2.71%,
      #bff4a6 2.72%,
      #eb34a0 96.75%
    );
    background-clip: text;
    -webkit-text-fill-color: transparent;
    cursor: pointer;
  }

  input[type=submit]:hover{
    border: none;
    background-color: transparent;
    border-bottom: 2px solid #eb34a0;
  }
  

  .social-media img {
    width: 4em;
    height: 4em;
    margin: 1em;
    vertical-align: middle;
  }

  .social-media a {
    text-decoration: none;
  }

  .social-media a:hover {
    font-weight: bold;
    text-decoration: line-through;
  }

  span{
    font-size: 0.8em;
    text-align: end;
    display: block;
  }

  @media (max-width: 800px) {
    #contact {
      width: 90%;
    }
    form {
      width: 90%;
    }
    .names,
    .obj {
      flex-direction: column;
      align-items: flex-start;
      width: 100%;
    }
    .names input,
    .obj input {
      width: 100%;
    }
    .names input {
      margin-bottom: 1em;
    }
    .obj input {
      margin-bottom: 1em;
    }
    .message {
      width: 100%;
    }
    .social-medias {
      width: 100%;
    }

  }
  
</style>
