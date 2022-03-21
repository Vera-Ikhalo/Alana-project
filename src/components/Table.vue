<template>
    <div class="position-relative group d-flex">
        <div class="table-one">
            <div class="position-relative table-dash">
                <p class="position-absolute title active">Active</p>
                <table class="active table-striped table-hover">
                    <thead>
                        <tr class="d-flex">
                            <!--<img src="../assets/Icon-Fix-Car.svg" alt="car-tool" width="30" class="mr-2">
                            <img src="../assets/Icon-Owner.svg" alt="owner" width="30" >
                            <img src="../assets/Icon-Billing-Button.svg" alt="billing" width="15">-->
                        </tr>  
                        <tr >
                            <th>
                                
                            </th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr 
                            v-for="(item, ix) in first.items" 
                            :key="ix"
                            :class="{
                                        'background-one': first.items[ix].position === 'odd',
                                        'background-two': first.items[ix].position === 'even',
                                        'background-active': first.items[ix].status === 'active',
                                    }"
                        >
                            <td><label class="d-flex justify-content-center align-items-center form-checkbox"><input type="checkbox" :value="item.id" v-model="selected"><i class="form-icon"></i></label></td>
                            <td>{{first.items[ix].headOne}}</td>
                            <td>{{first.items[ix].headTwo}}</td>
                            <td>{{first.items[ix].headThree}}</td>
                            <td>{{first.items[ix].headFour}}</td>
                            <td>{{first.items[ix].headFive}}</td>
                            <td>{{first.items[ix].headSix}}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
        <!-------------------Table Two------------------>
        <div class="table-two">
            <div class="position-relative table-dash">
                <p class="position-absolute title">Inactive Tab Label</p>
                <table class="table-striped table-hover others">
                    <thead>
                        <tr class="font-weight-bold">
                            <th>
                                
                            </th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr 
                            v-for="(item, ix) in second.items" 
                            :key="ix"
                            :class="{
                                        'background-one': second.items[ix].position === 'odd',
                                        'background-two': second.items[ix].position === 'even',
                                        'background-active': second.items[ix].status === 'active',
                                    }"
                        >
                            <td><label class="d-flex justify-content-center align-items-center form-checkbox"><input type="checkbox" :value="item.id" v-model="selected"><i class="form-icon"></i></label></td>
                            <td>{{second.items[ix].headOne}}</td>
                            <td>{{second.items[ix].headTwo}}</td>
                            <td>{{second.items[ix].headThree}}</td>
                            <td>{{second.items[ix].headFour}}</td>
                            <td>{{second.items[ix].headFive}}</td>
                            <td>{{second.items[ix].headSix}}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
        <!-----------------Table Three------------------>
        <div class="table-three">
            <div class="position-relative table-dash">
                <p class="position-absolute title">Inactive Tab Label</p>
                <table class="table-striped table-hover others">
                    <thead>
                        <tr class="font-weight-bold">
                            <th>
                                
                            </th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr 
                            v-for="(item, ix) in third.items" 
                            :key="ix"
                            :class="{
                                        'background-one': third.items[ix].position === 'odd',
                                        'background-two': third.items[ix].position === 'even',
                                        'background-active': third.items[ix].status === 'active',
                                    }"
                        >
                            <td><label class="d-flex justify-content-center align-items-center form-checkbox"><input type="checkbox" :value="item.id" v-model="selected"><i class="form-icon"></i></label></td>
                            <td>{{third.items[ix].headOne}}</td>
                            <td>{{third.items[ix].headTwo}}</td>
                            <td>{{third.items[ix].headThree}}</td>
                            <td>{{third.items[ix].headFour}}</td>
                            <td>{{third.items[ix].headFive}}</td>
                            <td>{{third.items[ix].headSix}}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
        <!-----------------Table Four------------------>
        <div class="table-four">
            <div class="position-relative table-dash">
                <p class="position-absolute title">Inactive Tab Label</p>
                <table class="table-striped table-hover others">
                    <thead>
                        <tr class="font-weight-bold">
                            <th>
                                
                            </th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr 
                            v-for="(item, ix) in fourth.items" 
                            :key="ix"
                            :class="{
                                        'background-one': fourth.items[ix].position === 'odd',
                                        'background-two': fourth.items[ix].position === 'even',
                                        'background-active': fourth.items[ix].status === 'active',
                                    }"
                        >
                            <td><label class="d-flex justify-content-center align-items-center form-checkbox"><input type="checkbox" :value="item.id" v-model="selected"><i class="form-icon"></i></label></td>
                            <td>{{fourth.items[ix].headOne}}</td>
                            <td>{{fourth.items[ix].headTwo}}</td>
                            <td>{{fourth.items[ix].headThree}}</td>
                            <td>{{fourth.items[ix].headFour}}</td>
                            <td>{{fourth.items[ix].headFive}}</td>
                            <td>{{fourth.items[ix].headSix}}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
        <!------------------Table Five------------------>
        <div class="table-five">
            <div class="position-relative table-dash">
                <p class="position-absolute title">Small Inactive Tab Label</p>
                <table class="table-striped table-hover others">
                    <thead>
                        <tr class="font-weight-bold">
                            <th>
                                
                            </th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                            <th>Head</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr 
                            v-for="(item, ix) in fifth.items" 
                            :key="ix"
                            :class="{
                                        'background-one': fifth.items[ix].position === 'odd',
                                        'background-two': fifth.items[ix].position === 'even',
                                        'background-active': fifth.items[ix].status === 'active',
                                    }"
                        >
                            <td><label class="d-flex justify-content-center align-items-center form-checkbox"><input type="checkbox" :value="item.id" v-model="selected"><i class="form-icon"></i></label></td>
                            <td>{{fifth.items[ix].headOne}}</td>
                            <td>{{fifth.items[ix].headTwo}}</td>
                            <td>{{fifth.items[ix].headThree}}</td>
                            <td>{{fifth.items[ix].headFour}}</td>
                            <td>{{fifth.items[ix].headFive}}</td>
                            <td>{{fifth.items[ix].headSix}}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
    </div>
</template>

<script>

export default{
    name: 'TableView',
    data() {
        return {
           first: {
                items: [
                {
                    id: "id1",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "active"
                },
                {
                    id: "id2",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id3",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "active"
                },
                {
                    id: "id4",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id5",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "active"
                },
                {
                    id: "id6",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
            ],
            selected: [],
            selectAll: false,
           },
           second: {
                items: [
                {
                    id: "id1",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id2",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id3",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id4",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id5",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id6",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
            ],
            selected: [],
            selectAll: false,
           },
           third: {
                items: [
                {
                    id: "id1",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id2",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id3",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id4",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id5",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id6",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
            ],
            selected: [],
            selectAll: false,
           },
           fourth: {
                items: [
                {
                    id: "id1",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id2",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id3",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id4",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id5",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id6",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
            ],
            selected: [],
            selectAll: false,
           },
           fifth: {
                items: [
                {
                    id: "id1",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id2",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id3",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id4",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
                {
                    id: "id5",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "odd",
                    status: "inactive"
                },
                {
                    id: "id6",
                    headOne: "Body",
                    headTwo: "Body",
                    headThree: "Body",
                    headFour: "Body",
                    headFive: "Body",
                    headSix: "Body",
                    position: "even"
                },
            ],
            selected: [],
            selectAll: false,
           },
        }
    },
	methods: {
		select() {
			this.selected = [];
			if (!this.selectAll) {
				for (let i in this.items) {
					this.selected.push(this.items[i].id);
				}
			}
		}
	}
}
</script>

<style lang="scss" scoped>
.group{
    margin-bottom:20px;
    .table-one{
            z-index:999;
            .title.active{
                border: 1px solid #0086FA;
                border-bottom: 1px solid white ;
            }
            table.active{
                opacity:100%;
                border: 1px solid #0086FA;
                color:#000000;
                th{
                    font-weight:bold;
                    font-family:'Helvetica Neue';
                    
                }
                td{
                    font-family: 'Helvetica Neue';
                    color:#000000;
                    font-weight:normal;
                }
              }
            }
            table.others{
                th{
                    font-weight:bold;
                    font-family:'Helvetica Neue';
                    color:#B7B7B7;
                    
                }
                td{
                    font-family: 'Helvetica Neue';
                    color:#000000;
                    font-weight:normal;
                    opacity:52%;
                }
            }
            .table-two{
               left:310px;
               position:absolute;
               z-index:3;
               
            }
            .table-three{
                left:680px;
                position:absolute;
                z-index:2;
            }
            .table-four{
               left:1030px;
               position:absolute;
               z-index:1;
               
            }
            .table-five{
                 left:1400px;
                position:absolute;
                z-index:-1;
                .title{
                    border-bottom:1px solid #A9ADCC !important;
                    padding: 12px 30px !important;     
            }
            }
    .table-dash{
        padding: 50px 31px 10px;
        .title{
            border:1px solid #A9ADCC;
            border-bottom:1px solid white;
            z-index:999;
            height: 42px;
            background:white;
            left:41px;
            font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
            top:10px;
            padding: 12px 97px;
            width: auto;
            margin-bottom:0;
            }
            
            table{
                position:relative;
                border: 1px solid #A9ADCC;
                margin-top:0;
                border-radius:5px;
                padding-left:20px;
                padding-right:20px;
                td:nth-child(2){
                    border-left:1px solid white;
                }
                th:nth-child(1),
                td:nth-child(1){
                     margin-right:0 ;
                    padding-right:10px;
                     margin-left:0 ;
                    padding-left:10px;
                }
                }
               
                .background-one{
                    background: #EBEBEB;
                    border-bottom :1px solid #B7B7B7;
                    color:#B7B7B7;
                }
                .background-active{
                    background: #B7B7B7;
                    border-bottom :1px solid #30313A;
                    color:#000;
                }
                .background-two{
                    background:#FFF;
                }
                td{
                    padding:0 45px 0 10px;
                    height:51px;
                }
                th{
                    background-color:white;
                    padding:0 45px 0 10px;
                    height:51px;
                }
        }
    }



</style>