<template>
    <div>
        <b-modal @ok="handleOk" ref="my-modal" id="modal-1" title="BootstrapVue">
            <!-- <p class="my-4">Hello from modal!</p> -->
            <b-form inline>
                <label class="sr-only" for="inline-form-input-name">Name</label>
                <label class="sr-only" for="inline-form-input-username">Username</label>
                <b-input-group prepend="@" class="mb-2 mr-sm-2 mb-sm-0">
                    <b-form-input id="inline-form-input-username" placeholder="Username"></b-form-input>
                </b-input-group>

                <b-form-checkbox class="mb-2 mr-sm-2 mb-sm-0">Remember me</b-form-checkbox>
            </b-form>
        </b-modal>
    </div>
</template>

<script>
export default {
    name: "SignupModal",
    methods: {
        handleOk(bvModalEvent) {
            bvModalEvent.preventDefault()
            alert('Hello')
        },
    }
}

</script>


