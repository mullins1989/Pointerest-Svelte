<script>
    import {title, subTitle, navBar, welcomeBar} from "../stores"
    import LoginForm from "../components/LoginForm.svelte"
    import travelicon from "/src/assets/travelicon.png";
    title.set("Pointerest");
    subTitle.set("Please Log in");

    navBar.set({
        bar: welcomeBar
    });
</script>

<div class="uk-flex-middle uk-text-center" uk-grid>
    <div class="uk-width-2-3@m">
        <div class="uk-card uk-card-default uk-card-body uk-box-shadow-large uk-width-2xlarge ">
            <h3 class="uk-card-title uk-text-center">Welcome back!</h3>
            <LoginForm />
        </div>
    </div>
    <div class="uk-width-1-3@m ">
        <img width="300" src="{travelicon}" alt="travelicon">
    </div>
</div>