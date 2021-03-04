<template>
    <div class="aaa">
        <div>2021-01-26</div>
        <div class="navigation">
            <input
                type="checkbox"
                class="navigation__checkbox"
                id="navi-toggle"
            />
            <label for="navi-toggle" class="navigation__button">MENU</label>
            <div class="navigation__background">&nbsp;</div>
            <nav class="navigation__nav">
                <ul class="navigation__list">
                    <li class="navigation__item">
                        <a href="#" class="navigation__link"
                            ><span>01</span>About Natours</a
                        >
                    </li>
                    <li class="navigation__item">
                        <a href="#" class="navigation__link"
                            ><span>02</span>Your benefits</a
                        >
                    </li>
                    <li class="navigation__item">
                        <a href="#" class="navigation__link"
                            ><span>03</span>Popular tours</a
                        >
                    </li>
                    <li class="navigation__item">
                        <a href="#" class="navigation__link"
                            ><span>04</span>Stories</a
                        >
                    </li>
                    <li class="navigation__item">
                        <a href="#" class="navigation__link"
                            ><span>05</span>Book now</a
                        >
                    </li>
                </ul>
            </nav>
        </div>
        <header class="header">
            <div class="header__logo-box">
                <img
                    src="../../assets/images/natours/logo-white.png"
                    alt="image of the logo"
                    class="header__logo"
                />
            </div>

            <div class="header__text-box">
                <h1 class="heading-primary">
                    <span class="heading-primary--main">Outdoors</span>
                    <span class="heading-primary--sub"
                        >is where life happens</span
                    >
                </h1>
                <a href="#" class="btn btn--white btn--sliding">
                    Discover our tours
                </a>
            </div>
        </header>

        <main>
            <section class="section-about">
                <div class="u-center-text u-margin-bottom-big">
                    <h2 class="heading-secondary">
                        Exciting tours for adventurous people
                    </h2>
                </div>

                <div class="row">
                    <div class="col-50prc">
                        <h3 class="heading-tertiary u-margin-bottom-small">
                            You're going to fall in love with nature
                        </h3>
                        <p class="paragraph">
                            Lorem ipsum dolor sit amet consectetur adipisicing
                            elit. Neque ducimus commodi quis a expedita
                            deleniti.
                        </p>

                        <h3 class="heading-tertiary u-margin-bottom-small">
                            Live adventures like you never have before
                        </h3>
                        <p class="paragraph">
                            Lorem ipsum dolor sit amet consectetur adipisicing
                            elit.
                        </p>

                        <a href="#" class="btn-text">Learn more &rarr;</a>
                    </div>
                    <div class="col-50prc">
                        <div class="composition">
                            <img
                                src="../../assets/images/natours/nat-1-large.jpg"
                                alt="Photo 1"
                                class="composition__photo composition__photo--p1"
                            /><img
                                src="../../assets/images/natours/nat-2-large.jpg"
                                alt="Photo 2"
                                class="composition__photo composition__photo--p2"
                            /><img
                                src="../../assets/images/natours/nat-3-large.jpg"
                                alt="Photo 3"
                                class="composition__photo composition__photo--p3"
                            />
                        </div>
                    </div>
                </div>
            </section>

            <section class="section-features">
                <div class="row">
                    <div class="col-25prc">
                        <div class="feature-box">
                            <i class="feature-box__icon icon-basic-world"></i>
                            <h3 class="heading-tertiary">Explore the world</h3>
                            <p class="feature-box__text">
                                Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>

                    <div class="col-25prc">
                        <div class="feature-box">
                            <i class="feature-box__icon icon-basic-compass"></i>
                            <h3 class="heading-tertiary">Meet nature</h3>
                            <p class="feature-box__text">
                                Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>

                    <div class="col-25prc">
                        <div class="feature-box">
                            <i class="feature-box__icon icon-basic-map"></i>
                            <h3 class="heading-tertiary">Find your way</h3>
                            <p class="feature-box__text">
                                Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>

                    <div class="col-25prc">
                        <div class="feature-box">
                            <i class="feature-box__icon icon-basic-heart"></i>
                            <h3 class="heading-tertiary">
                                Live a healthier life
                            </h3>
                            <p class="feature-box__text">
                                Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit.
                            </p>
                        </div>
                    </div>
                </div>
            </section>

            <section class="section-tours">
                <div class="u-center-text u-margin-bottom-big">
                    <h2 class="heading-secondary">Most popular tours</h2>
                </div>
                <div class="row">
                    <div class="col-33prc">
                        <div class="card">
                            <div class="card__side card__side--front">
                                <div class="card__picture card__picture--1">
                                    &nbsp;
                                </div>
                                <h4 class="card__heading">
                                    <span
                                        class="card__heading-span card__heading-span--1"
                                        >The sea explorer</span
                                    >
                                </h4>
                                <div class="card__details">
                                    <ul>
                                        <li>3 day tours</li>
                                        <li>Up to 30 people</li>
                                        <li>2 tour guides</li>
                                        <li>Sleep in cozy hotels</li>
                                        <li>Difficulty: easy</li>
                                    </ul>
                                </div>
                            </div>
                            <div
                                class="card__side card__side--back card__side--back-1"
                            >
                                <div class="card__cta">
                                    <div class="card__price-box">
                                        <p class="card__price-only">Only</p>
                                        <p class="card__price-value">$100</p>
                                    </div>
                                    <a href="#" class="btn btn--white"
                                        >Book now!</a
                                    >
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-33prc">
                        <div class="card">
                            <div class="card__side card__side--front">
                                <div class="card__picture card__picture--2">
                                    &nbsp;
                                </div>
                                <h4 class="card__heading">
                                    <span
                                        class="card__heading-span card__heading-span--2"
                                        >The forest hiker</span
                                    >
                                </h4>
                                <div class="card__details">
                                    <ul>
                                        <li>7 day tours</li>
                                        <li>Up to 40 people</li>
                                        <li>6 tour guides</li>
                                        <li>Sleep in provided tents</li>
                                        <li>Difficulty: medium</li>
                                    </ul>
                                </div>
                            </div>
                            <div
                                class="card__side card__side--back card__side--back-2"
                            >
                                <div class="card__cta">
                                    <div class="card__price-box">
                                        <p class="card__price-only">Only</p>
                                        <p class="card__price-value">$500</p>
                                    </div>
                                    <a href="#" class="btn btn--white"
                                        >Book now!</a
                                    >
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-33prc">
                        <div class="card">
                            <div class="card__side card__side--front">
                                <div class="card__picture card__picture--3">
                                    &nbsp;
                                </div>
                                <h4 class="card__heading">
                                    <span
                                        class="card__heading-span card__heading-span--3"
                                        >The snow adventurer</span
                                    >
                                </h4>
                                <div class="card__details">
                                    <ul>
                                        <li>5 day tours</li>
                                        <li>Up to 15 people</li>
                                        <li>3 tour guides</li>
                                        <li>Sleep in provided tents</li>
                                        <li>Difficulty: hard</li>
                                    </ul>
                                </div>
                            </div>
                            <div
                                class="card__side card__side--back card__side--back-3"
                            >
                                <div class="card__cta">
                                    <div class="card__price-box">
                                        <p class="card__price-only">Only</p>
                                        <p class="card__price-value">$900</p>
                                    </div>
                                    <a href="#" class="btn btn--white"
                                        >Book now!</a
                                    >
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="u-center-text u-margin-top-huge">
                    <a href="#" class="btn btn--green">Discover all tours</a>
                </div>
            </section>

            <section class="section-stories">
                <div class="bg-video">
                    <video class="bg-video__content" autoplay muted loop>
                        <source
                            src="../../assets/images/natours/video.mp4"
                            type="video/mp4"
                        />
                        <source
                            src="../../assets/images/natours/video.webm"
                            type="video/webm"
                        />
                        Your browser is not supported.
                    </video>
                </div>

                <div class="u-center-text u-margin-bottom-big">
                    <h2 class="heading-secondary">
                        We make people genuinely happy
                    </h2>
                </div>

                <div class="row">
                    <div class="story">
                        <figure class="story__shape">
                            <img
                                src="../../assets/images/natours/nat-8.jpg"
                                alt="Person on a tour"
                                class="story__img"
                            />
                            <figcaption class="story__caption">
                                Mary Smith
                            </figcaption>
                        </figure>
                        <div class="story__text">
                            <h3 class="heading-tertiary u-margin-bottom-small">
                                I had the best thing with my family
                            </h3>
                            <p>
                                Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit. Veritatis quod rerum labore
                                quae nostrum maxime aperiam recusandae nesciunt
                                aliquam laboriosam natus dolorum alias, ad
                                commodi sed provident repellendus eum quasi?
                            </p>
                        </div>
                    </div>
                </div>

                <div class="row">
                    <div class="story">
                        <figure class="story__shape">
                            <img
                                src="../../assets/images/natours/nat-9.jpg"
                                alt="Person on a tour"
                                class="story__img"
                            />
                            <figcaption class="story__caption">
                                Jack Wilson
                            </figcaption>
                        </figure>
                        <div class="story__text">
                            <h3 class="heading-tertiary u-margin-bottom-small">
                                Wow! My life is completely different now.
                            </h3>
                            <p>
                                Lorem, ipsum dolor sit amet consectetur
                                adipisicing elit. Veritatis quod rerum labore
                                quae nostrum maxime aperiam recusandae nesciunt
                                aliquam laboriosam natus dolorum alias, ad
                                commodi sed provident repellendus eum quasi?
                            </p>
                        </div>
                    </div>
                </div>

                <div class="u-center-text u-margin-top-huge">
                    <a href="#" class="btn-text">Read all stories &rarr;</a>
                </div>
            </section>

            <section class="section-book">
                <div class="row">
                    <div class="book">
                        <div class="book__form">
                            <form action="#" class="form">
                                <div class="u-margin-bottom-medium">
                                    <h2 class="heading-secondary">
                                        Start booking now
                                    </h2>
                                </div>

                                <div class="form__group">
                                    <input
                                        type="text"
                                        class="form__input"
                                        placeholder="Full Name"
                                        id="name"
                                        required
                                    />
                                    <label for="name" class="form__label"
                                        >Full Name</label
                                    >
                                </div>

                                <div class="form__group">
                                    <input
                                        type="email"
                                        class="form__input"
                                        placeholder="Email address"
                                        id="email"
                                        required
                                    />
                                    <label for="email" class="form__label"
                                        >Email address</label
                                    >
                                </div>

                                <div class="form__group u-margin-bottom-medium">
                                    <div class="form__radio-group">
                                        <input
                                            type="radio"
                                            class="form__radio-input"
                                            id="small"
                                            name="size"
                                        />
                                        <label
                                            for="small"
                                            class="form__radio-label"
                                        >
                                            <span
                                                class="form__radio-button"
                                            ></span>
                                            Small tour group
                                        </label>
                                    </div>
                                    <div class="form__radio-group">
                                        <input
                                            type="radio"
                                            class="form__radio-input"
                                            id="large"
                                            name="size"
                                        />
                                        <label
                                            for="large"
                                            class="form__radio-label"
                                        >
                                            <span
                                                class="form__radio-button"
                                            ></span>
                                            Large tour group
                                        </label>
                                    </div>
                                </div>

                                <div class="form__group">
                                    <button class="btn btn--green">
                                        Next step &rarr;
                                    </button>
                                </div>
                            </form>
                        </div>
                    </div>
                </div>
            </section>
        </main>

        <footer class="footer">
            <div class="footer__logo-box">
                <img
                    src="../../assets/images/natours/logo-green-2x.png"
                    alt="Full logo"
                    class="footer__logo"
                />
            </div>
            <div class="row">
                <div class="col-50prc">
                    <div class="footer__navigation">
                        <ul class="footer__list">
                            <li class="footer__item">
                                <a href="#" class="footer__link">Company</a>
                            </li>
                            <li>
                                <a href="#" class="footer__link">Contact us</a>
                            </li>
                            <li>
                                <a href="#" class="footer__link">Careers</a>
                            </li>
                            <li>
                                <a href="#" class="footer__link"
                                    >Privacy policy</a
                                >
                            </li>
                            <li><a href="#" class="footer__link">Terms</a></li>
                        </ul>
                    </div>
                </div>
                <div class="col-50prc">
                    <p class="footer__copyright">
                        Built by
                        <a href="#" class="footer__link">IGORYEN</a>. Originally
                        built and designed by
                        <a href="#" class="footer__link">JONAS SCHMEDTMANN</a>
                        for his online course
                        <a href="" class="footer__link">ADVANCED CSS AND SASS</a
                        >. Copyright &copy; by Jonas Schmedtmann.
                    </p>
                </div>
            </div>
        </footer>

        <!-- <section class="grid-test">
            <div class="row">
                <div class="col-50prc">50%</div>
                <div class="col-50prc">50%</div>
            </div>

            <div class="row">
                <div class="col-33prc">33%</div>
                <div class="col-33prc">33%</div>
                <div class="col-33prc">33%</div>
            </div>

            <div class="row">
                <div class="col-33prc">33%</div>
                <div class="col-66prc">66%</div>
            </div>

            <div class="row">
                <div class="col-25prc">25%</div>
                <div class="col-25prc">25%</div>
                <div class="col-25prc">25%</div>
                <div class="col-25prc">25%</div>
            </div>

            <div class="row">
                <div class="col-25prc">25%</div>
                <div class="col-50prc">50%</div>
                <div class="col-25prc">25%</div>
            </div>

            <div class="row">
                <div class="col-25prc">25%</div>
                <div class="col-75prc">75%</div>
            </div>
        </section> -->
    </div>
</template>

<style lang="scss" scoped>
.aaa {
    padding-top: 5rem;
}
</style>

<script>
import "@/assets/scss/linea/icon-font/styles.css";
export default {};
</script>
