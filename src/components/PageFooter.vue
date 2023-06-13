<script>
export default {
    name: 'PageFooter'
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="form">
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
                    <textarea cols="30" rows="10" placeholder="Message" required></textarea>
                    <button class="btn primary">
                        SEND
                    </button>
                </form>
            </div>
            <div class="contacts">

            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use './../styles/variables' as *;

footer {
    padding-block: 80px;

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

        .form {
            width: 55%;

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
                    width: 100%;
                    border: none;
                    border-radius: 3px;
                    height: 100px;
                    background-color: #ececec;
                    padding: 10px;
                }
            }
        }

        .contacts {
            width: 40%;
        }
    }
}
</style>