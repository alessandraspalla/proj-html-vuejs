<script>
export default {
    name: 'PageFooter'
}
</script>

<template>
    <footer>
        <div class="container">
            <div id="form">
                <span class="summary">SEND A MESSAGE</span>
                <h2>Get In <span>Touch</span></h2>
                <p>We will respond to your message as soon as possible.</p>
                <form action="#">
                    <input type="text" placeholder="Name" required>
                    <input type="email" placeholder="Email" required>
                    <input type="tel" placeholder="Phone" required>
                    <select>
                        <option value="More info">More Info</option>
                    </select>
                    <textarea cols="40" rows="25" placeholder="Message" required></textarea>
                    <button class="btn primary">
                        SEND
                    </button>
                </form>
            </div>
            <div class="contact">
                <h3>Example Inc.</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                <p>Praesent diam lacus, lapibus sed imperdiet consectetur.</p>
                <div class="contacts">
                    <div class="phone">
                        <i class="fa-solid fa-phone"></i>
                        +1 (305) 1234-5678
                    </div>
                    <div class="email">
                        <i class="fa-solid fa-envelope"></i>
                        hello@example.com
                    </div>
                    <div class="maps">
                        <i class="fa-solid fa-location-dot"></i>
                        Main Avenue, 987
                    </div>
                    <button class="btn reverse">
                        VIEW MAP
                    </button>
                </div>
            </div>
        </div>
        <div id="copyright">
            <div class="container">
                <p>Enjoy the low price. We are tracking any intention of privacy.</p>
                <p><i class="fa-regular fa-copyright"></i> NEXGEN is Proudly Powered by <a href="#">Codings</a>.</p>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use './../styles/variables' as *;

footer {

    .container {
        display: flex;

        h2 {
            margin-top: 10px;
        }

        h2,
        p {
            color: $title-color;
        }

        h2 span {
            padding-inline: 7px;
            color: $primary-color;
            background-color: rgba($primary-color, $alpha: .15);
        }

        #form {
            padding-block: 80px;
            width: 57%;
            margin-right: 40px;

            form {
                display: flex;
                justify-content: space-between;
                flex-wrap: wrap;
                margin-top: 50px;

                input,
                select {
                    width: calc(50% - 5px);
                    border: none;
                    border-radius: 3px;
                    height: 40px;
                    background-color: #ececec;
                    margin-bottom: 10px;
                    padding-left: 5px;
                }

                select {
                    color: rgb(110, 110, 110);
                }

                textarea {
                    min-height: 80px;
                    width: 100%;
                    border: none;
                    border-radius: 3px;
                    height: 100px;
                    background-color: #ececec;
                    padding: 10px;
                }
            }
        }

        .contact {
            width: 30%;
            padding-block: 80px;


            h3,
            p {
                color: $title-color;
            }

            .contacts {
                color: $primary-color;
                line-height: 3rem;

                i {
                    padding: 10px;
                    border-radius: 50%;
                    background-color: rgba($primary-color, $alpha: .2);
                }

                button {
                    margin: 0;
                    background-color: $white;
                }
            }
        }
    }

    #copyright {
        height: 60px;
        background-color: #0d0d11;

        .container {
            display: flex;
            justify-content: space-between;
            height: 100%;
            align-items: center;
        }

        p {
            color: $white;
            font-size: .75rem;

            a {
                color: $primary-color;
            }
        }

    }
}
</style>