<script lang="ts">
    // assign variables their interfaces for type check
    // let button = document.getElementById("submitButton") as HTMLButtonElement;
    // var userName = document.getElementById("name") as HTMLFormElement;
    let button: HTMLButtonElement;
    let userName: string;
    async function fetchType(name: string) {
        console.log(name);
        const response = await fetch(
            `https://api.agify.io?name=${name.toLowerCase()}`
        );
        const data = await response.json();
        printFact(data.age);
    }
    function start() {
        fetchType(userName);
    }
    // let factEl: HTMLDivElement;
    let textField: HTMLElement;
    function printFact(age: string | null | undefined) {
        // var factEl = document.getElementById("fact");
        console.log(age);
        if (age === null) {
            document.getElementById("fact")!.innerHTML = "Incorrect name!";
        }
        // check if this element is not null
        //    if (factEl === null) throw new Error("Cannot find the fact element");
        // check if age is currect
        // else we can safely assign value without type checking
        else {
            document.getElementById("fact")!.innerHTML = "Your age - " + age;
        }
        // assign interface
        // var textField = document.getElementById("fact") as HTMLElement;
        textField.style.visibility = "visible";
    }
</script>

<div class="wrapper">
    <div class="row">
        <div class="col span6 box">
            <div class="buttons">
                <input
                    id="name"
                    type="text"
                    bind:value={userName}
                    placeholder="Enter your name"
                />
                <button
                    type="submit"
                    bind:this={button}
                    on:click={start}
                    id="submitButton"
                >
                    Submit
                </button>
            </div>
            <div id="fact" bind:this={textField} />
        </div>
    </div>
</div>

<style>
    .box {
        margin-top: 2%;
        margin-bottom: 2%;
        padding-top: 1%;
        padding-bottom: 1%;
        background-color: #7f55db;
        border-radius: 15px;
        word-break: break-word;
        max-height: 700px;
        overflow: auto;
        text-align: center;
    }

    #fact {
        margin: 5% 10% 5% 10%;
        padding: 2% 2% 2% 2%;
        border-radius: 15px;
        border-style: dashed;
        visibility: hidden;
    }

    #name {
        color: black;
        padding: 3% 2% 3% 2%;
        height: 1rem;
        width: 50%;
    }

    #submitButton {
        width: 20%;
        color: black;
        margin-left: 3%;
        padding-left: 3%;
        padding-right: 3%;
    }

    .buttons {
        color: black;
        margin-top: 3%;
        display: flex;
        justify-content: center;
    }

</style>
