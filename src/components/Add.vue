<template>
  <div>
    <b-row>
      <b-col>
        <b-form-group>
          <label>Tour Name</label>
          <b-input v-model="tour.name"/>
        </b-form-group>
      </b-col>
      <b-col>
        <b-form-group>
          <label>Tour Code</label>
          <b-input v-model="tour.code"/>
        </b-form-group>
      </b-col>
      <b-col>
        <b-form-group>
          <label>Date</label>
          <b-input type="date" v-model="tour.date"/>
        </b-form-group>
      </b-col>
    </b-row>
    <b-row>
      <b-col>
        <b-form-group>
          <label>Name of Participant</label>
          <b-input v-model="participant.name"/>
        </b-form-group>
      </b-col>
      <b-col>
        <b-form-group>
          <label>Phone</label>
          <b-input v-model="participant.phone"/>
        </b-form-group>
      </b-col>
      <b-col>
        <b-form-group>
          <label>Email</label>
          <b-input type="email" v-model="participant.email"/>
        </b-form-group>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  name: 'Add',
  data () {
    return {
      tour: {
        name: null,
        code: null,
        date: new Date().toISOString().split('T')[0]
      },
      participant: {
        name: null,
        phone: null,
        email: null
      }
    }
  }
}
</script>
