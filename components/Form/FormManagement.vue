<template>
    <div class="form-edit">
        <div class="form-head">PROPERTY MANAGEMENT</div>
        <p class="mt-2">
            Great article. I wonder if there is a way this can be learned?
        </p>
        <form action="">
            <div>
                <label for="">Full Name</label>
                <input
                    type="text"
                    class="form-control"
                    placeholder="Enter full name"
                />
            </div>
            <div class="mt-1">
                <label for="">Email Address</label>
                <input
                    type="email"
                    class="form-control"
                    placeholder="Enter email address"
                />
            </div>
            <div class="mt-1">
                <label for="">Message</label>
                <textarea name="" id="" class="form-control"></textarea>
            </div>
            <div class="btn btn-send mt-4">Message Us</div>
        </form>
    </div>
</template>
<style scoped>
.form-edit {
    padding: 1rem 2rem 0 2rem;
}
.form-head {
    font-style: normal;
    font-weight: bold;
    font-size: 28px;
    line-height: 28px;
    letter-spacing: 0.03em;
    text-transform: uppercase;
    color: #002817;
}
label {
    color: #002817;
    font-style: normal;
    font-weight: bold;
}
input {
    background: #eff0f7;
    width: 70%;
}
textarea {
    background: #eff0f7;
    width: 70%;
}
.btn-send {
    background: #08804b;
    border-radius: 6px;
    text-align: center;
    color: #fff;
    width: 70%;
}
@media screen and (max-width: 768px) {
    .form-edit {
        padding: 1rem;
    }
    input {
        width: 100%;
    }
    textarea {
        width: 100%;
    }
    .btn-send {
        width: 100%;
    }
    .form-head {
        font-style: normal;
        font-weight: bold;
        font-size: 18px;
        line-height: 28px;
        letter-spacing: 0.03em;
        text-transform: uppercase;
        color: #002817;
        margin-top: 1rem;
    }
}
@media screen and (min-width: 1000px) and (max-width: 1024px) {
    .form-edit {
        padding: 0;
    }
}
</style>