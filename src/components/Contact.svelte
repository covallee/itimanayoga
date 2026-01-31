<script>
  let contact = {
    social: {
      instagram: "https://www.instagram.com/itimanayoga/",
      facebook: "https://www.facebook.com/itimanayoga/",
      email: "itimanayoga@gmail.com",
    },
    address: "1 place de la résistance, 64400, Oloron Ste Marie",
    newAddress: "La Friche, 5 bis rue de Rocgrand, 64400 Oloron-Sainte-Marie",
    newAddressDate: "1er mars 2026",
    phone: "06.98.98.64.16",
    pricing: {
      single: "12€",
      package: "50€",
      trial: "offert",
    },
  };
</script>

<div class="contact">
  <h2>Contact</h2>
  <h3>Social</h3>
  <div class="social">
    <a href={contact.social.instagram}>
      <span class="sr-only">Pour voir ma page Instagram</span>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        x="0px"
        y="0px"
        width="100"
        height="100"
        viewBox="0 0 50 50"
      >
        <path
          d="M 16 3 C 8.83 3 3 8.83 3 16 L 3 34 C 3 41.17 8.83 47 16 47 L 34 47 C 41.17 47 47 41.17 47 34 L 47 16 C 47 8.83 41.17 3 34 3 L 16 3 z M 37 11 C 38.1 11 39 11.9 39 13 C 39 14.1 38.1 15 37 15 C 35.9 15 35 14.1 35 13 C 35 11.9 35.9 11 37 11 z M 25 14 C 31.07 14 36 18.93 36 25 C 36 31.07 31.07 36 25 36 C 18.93 36 14 31.07 14 25 C 14 18.93 18.93 14 25 14 z M 25 16 C 20.04 16 16 20.04 16 25 C 16 29.96 20.04 34 25 34 C 29.96 34 34 29.96 34 25 C 34 20.04 29.96 16 25 16 z"
        ></path>
      </svg></a
    >

    <a href={contact.social.facebook}>
      <span class="sr-only">Pour voir ma page Facebook</span>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        x="0px"
        y="0px"
        width="100"
        height="100"
        viewBox="0 0 50 50"
      >
        <path
          d="M25,3C12.85,3,3,12.85,3,25c0,11.03,8.125,20.137,18.712,21.728V30.831h-5.443v-5.783h5.443v-3.848 c0-6.371,3.104-9.168,8.399-9.168c2.536,0,3.877,0.188,4.512,0.274v5.048h-3.612c-2.248,0-3.033,2.131-3.033,4.533v3.161h6.588 l-0.894,5.783h-5.694v15.944C38.716,45.318,47,36.137,47,25C47,12.85,37.15,3,25,3z"
        ></path>
      </svg>
    </a>
  </div>
  <div class="contact">
    <h3>Email</h3>
    <p>
      ✉️ <a href="mailto={contact.social.email}">{contact.social.email}</a>
    </p>
    <h3>Télephone</h3>
    <div class="booking">
      <p>Réservation par SMS ou WhatsApp au</p>
      <a href="tel:{contact.phone}">{contact.phone}</a>
    </div>
  </div>

  <address>
    <h3>Adresse</h3>
    <p>{contact.address}</p>
    <p class="new-address">
      <strong>À partir du {contact.newAddressDate} :</strong><br />
      {contact.newAddress}
    </p>
  </address>

  <div class="pricing">
    <h3>Tarifs</h3>
    <p>Cours à l'unité: {contact.pricing.single}</p>
    <p>Pass 5 cours: {contact.pricing.package} (valable 3 mois)</p>
    <!-- <p>Cours d'essai {contact.pricing.trial}</p> -->
  </div>
</div>

<style>
  .contact {
    /* padding: 2rem;
    background-color: var(--background-color);
    border-radius: 8px; */
  }

  .social {
    display: flex;
    gap: 1rem;
    justify-content: center;
  }

  .social a {
    display: block;
    width: 60px;
    height: 60px;
  }

  .social svg {
    fill: var(--primary-color);
    width: 100%;
    height: 100%;
  }

  .contact {
    text-align: center;
  }

  .contact a {
    color: var(--primary-color);
  }

  h2 {
    font-family: "Libre Caslon Text", serif;
    color: var(--primary-color);
    margin-bottom: 1.5rem;
    font-size: 1.7rem;
    font-weight: 400;
    font-style: italic;
    letter-spacing: 0.15rem;
    text-align: center;
  }

  h3 {
    margin-top: 2rem;
    text-align: center;
    color: var(--primary-color);
  }

  p {
    margin: 0.5rem 0;
    color: var(--primary-color);
  }

  address {
    text-align: center;
    margin: 1rem 0;
    font-style: normal;
    color: var(--primary-color);
  }

  .new-address {
    margin-top: 1rem;
    padding: 1rem;
    background-color: rgba(139, 115, 85, 0.1);
    border-radius: 8px;
  }

  .pricing {
    /* margin-top: 1.5rem; */
    /* font-weight: bold; */
  }

  .pricing p {
    text-align: center;
    color: var(--primary-color);
  }
</style>
