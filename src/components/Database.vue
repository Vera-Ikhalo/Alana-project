<template>
    <div class="database py-2 px-3 d-flex">
        <div class="image-area">
            <div class="db-image d-flex align-items-center justify-content-center text-blue-20 text-sm pointer">Image from database</div>
            <div class="details">
                <p class="text-black-10 text-sm-2">Data from database</p>
                <p class="text-black-10">Data string</p>
                <p class="text-black-10">A long data string of information</p>
            </div>
        </div>
        <div class="field-content">
            <div>
                <p class="text-sm text-black-10">Title of field Content</p>
                <p class="text-md text-black-10">Important data from the selected object</p>
                <p class="text-sm-2 text-black-10">Less important data from selected row</p>
            </div>
            <div class="d-flex">
                <div>
                    <p class="text-sm-2 text-black-10">Cell: <span class="figure">(571) 123-4567</span></p>
                    <p class="text-sm-2 text-black-10">Cell: <span class="figure">(703) 123-4567</span></p>
                    <p class="text-sm-2 text-black-10">Cell: <span class="figure">(703) 123-4567</span></p>
                </div>
                <div>
                    <p class="text-sm-2 text-black-10">Office: <span class="figure">(703) 123-4567</span></p>
                    <p class="text-sm-2 text-black-10">Office: <span class="figure">(703) 123-4567</span></p>
                    <p class="text-sm-2 text-black-10">Office: <span class="figure">(703) 123-4567</span></p>
                </div>
            </div>
        </div>
        <div class="data-label">
            <p class="text-sm-2 text-black-10">Data label:Data from Field</p>
            <p class="text-sm-2 text-black-10">Data label:Data from Field</p>
            <div class="data-from-field">
                <p class="text-sm-2 text-black-10">Data from Field</p>
                <p class="text-sm-2 text-black-10">Data from Field</p>
                <p class="text-sm-2 text-black-10">Data from Field</p>
            </div>
            <p class="text-sm-2 text-black-10">Data label:Data from Field</p>
        </div>
        <div class="icons d-flex flex-column align-items-center justify-content-between">
            <div class= "d-flex flex-column align-items-center justify-content-between">
                <img src="../assets/Icon-edit.svg" width="37" class="pointer mb-2">
                <img src="../assets/Icon-check.svg" width="35" class="pointer mb-2">
                <img src="../assets/Icon-Billing-Button.svg" width="15" class="pointer mb-2">
            </div>
            <img src="../assets/Icon-chevron-double-right.svg" width="54" class="pointer mt-4">
        </div>
    </div>
</template>

<script>

export default{
    name: 'DataBase',

}

</script>

<style lang="scss">
.database{
font-family: 'Open Sans';
margin-left:30px;
width: auto;
height: 225px;
background: #FFFFFF 0% 0% no-repeat padding-box;
border: 1px solid #A9ADCC;
    .image-area{
    margin-right:41px;
        .db-image{
            background-color: #CEC9C9;
            width: 255px;
            height: 110px;
        }
        .details{
            line-height:13px;
            margin-top:13px;
        }
    }
    .field-content{
        line-height:19px;
        span.figure{
            margin-right:58px;
        }
    }
    .data-label{
        border: 1px solid #30313A;
        padding:12px 11px;
        line-height:15px;
        margin-left:7px;
        .data-from-field{
            padding-left:30px;
        }
    }
}   

  
</style>