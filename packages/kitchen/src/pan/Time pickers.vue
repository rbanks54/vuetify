<template>
  <v-container>
    <v-layout column>
      <main-header>Time pickers</main-header>

      <core-title>
        Default
      </core-title>
      <core-section center>
        <v-time-picker value="9:41" />
      </core-section>

      <core-title>
        Landscape
      </core-title>
      <core-section center>
        <v-time-picker
          value="9:41"
          landscape
        />
      </core-section>

      <core-title>
        Disabled
      </core-title>
      <core-section>
        <v-layout
          justify-space-around
          align-center
        >
          <v-time-picker
            value="9:41"
            disabled
          />
          <v-time-picker
            value="9:41"
            disabled
            landscape
          />
        </v-layout>
      </core-section>

      <core-title>
        With AM/PM switch in title
      </core-title>
      <core-section>
        <v-layout
          justify-space-around
          align-center
          wrap
        >
          <v-time-picker
            value="9:41"
            ampm-in-title
          />
          <v-time-picker
            value="9:41"
            ampm-in-title
            landscape
          />
          <v-time-picker
            value="9:41"
            ampm-in-title
            disabled
          />
          <v-time-picker
            value="9:41"
            ampm-in-title
            landscape
            disabled
          />
        </v-layout>
      </core-section>

      <core-title>
        Colors
      </core-title>
      <core-section>
        <v-layout
          wrap
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            class="mt-6"
            color="success"
          />
          <v-time-picker
            value="9:41"
            class="mt-6"
            color="warning"
          />
          <v-time-picker
            value="9:41"
            class="mt-6"
            color="teal lighten-1"
          />
        </v-layout>

        <v-layout
          wrap
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            class="mt-6"
            landscape
            color="success"
          />
          <v-time-picker
            value="9:41"
            class="mt-6"
            landscape
            color="warning"
          />
          <v-time-picker
            value="9:41"
            class="mt-6"
            landscape
            color="teal lighten-1"
          />
        </v-layout>
      </core-section>

      <core-title>
        24 hour format
      </core-title>
      <core-section>
        <v-layout
          wrap
          justify-space-around
          align-center
        >
          <v-time-picker
            value="9:41"
            format="24hr"
          />
          <v-time-picker
            value="9:41"
            landscape
            format="24hr"
          />
        </v-layout>
      </core-section>

      <core-title>
        Disabled with 24 hour format
      </core-title>
      <core-section>
        <v-layout
          wrap
          justify-space-around
          align-center
        >
          <v-time-picker
            value="9:41"
            disabled
            format="24hr"
          />
          <v-time-picker
            value="9:41"
            disabled
            landscape
            format="24hr"
          />
        </v-layout>
      </core-section>

      <core-title>
        Allowed hours
      </core-title>
      <core-section>
        <v-layout
          wrap
          align-center
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            :allowed-hours="v => v >= 2 && v <= 13"
            class="mt-4"
            format="24hr"
          />

          <v-time-picker
            value="9:41"
            :allowed-hours="v => v >= 3 && v <= 11"
            class="mt-4"
            format="24hr"
          />

          <v-time-picker
            value="9:41"
            :allowed-hours="v => v >= 8 && v <= 17"
            class="mt-4"
            format="24hr"
          />
        </v-layout>
      </core-section>

      <core-title>
        Allowed minutes
      </core-title>
      <core-section>
        <v-layout
          wrap
          align-center
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            :allowed-minutes="v => v >= 10 && v <= 50"
            class="mt-4"
            format="24hr"
          />

          <v-time-picker
            value="9:41"
            :allowed-minutes="v => v >= 5 && v <= 40"
            class="mt-4"
            format="24hr"
          />

          <v-time-picker
            value="9:41"
            :allowed-minutes="v => v >= 20 && v <= 40"
            class="mt-4"
            format="24hr"
          />
        </v-layout>
      </core-section>

      <core-title>
        Allowed hours & minutes
      </core-title>
      <core-section>
        <v-layout
          wrap
          align-center
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            :allowed-hours="v => v >= 2 && v <= 13"
            :allowed-minutes="v => v >= 10 && v <= 50"
            class="mt-4"
            format="24hr"
          />

          <v-time-picker
            value="9:41"
            :allowed-hours="v => v >= 3 && v <= 11"
            :allowed-minutes="v => v >= 5 && v <= 40"
            class="mt-4"
            format="24hr"
          />

          <v-time-picker
            value="9:41"
            :allowed-hours="v => v >= 8 && v <= 17"
            :allowed-minutes="v => v >= 20 && v <= 40"
            class="mt-4"
            format="24hr"
          />
        </v-layout>
      </core-section>

      <core-title>
        Custom width
      </core-title>
      <core-section>
        <v-layout
          wrap
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            class="mt-6 center"
            width="150"
          />
          <v-time-picker
            value="9:41"
            class="mt-6 center"
            width="200"
          />
          <v-time-picker
            value="9:41"
            class="mt-6 center"
            width="300"
          />
        </v-layout>

        <v-layout
          wrap
          justify-space-around
        >
          <v-time-picker
            value="9:41"
            class="mt-6 center"
            landscape
            width="150"
          />
          <v-time-picker
            value="9:41"
            class="mt-6 center"
            landscape
            width="200"
          />
          <v-time-picker
            value="9:41"
            class="mt-6 center"
            landscape
            width="400"
          />
        </v-layout>
      </core-section>

      <core-title>
        Full width
      </core-title>
      <core-section>
        <v-layout column>
          <v-time-picker
            value="9:41"
            class="mt-6"
            full-width
          />
          <v-time-picker
            value="9:41"
            class="mt-6"
            landscape
            full-width
          />
        </v-layout>
      </core-section>

      <sub-header>With seconds</sub-header>

      <core-title>
        Simple
      </core-title>
      <core-section center>
        <v-time-picker
          value="9:41:14"
          use-seconds
        />
      </core-section>

      <core-title>
        Allowed seconds
      </core-title>
      <core-section center>
        <v-time-picker
          value="9:41:14"
          use-seconds
          :allowed-seconds="v => v <= 40 && v >= 15"
        />
      </core-section>

      <sub-header>As popup</sub-header>

      <core-title>
        In dialog
      </core-title>
      <core-section center>
        <v-dialog
          ref="dialog"
          v-model="modal"
          :return-value.sync="time1"
          persistent
          full-width
          width="290px"
        >
          <template #activator>
            <v-text-field
              v-model="time1"
              label="Picker in dialog"
              prepend-icon="mdi-clock-outline"
              readonly
            />
          </template>
          <v-time-picker
            v-if="modal"
            v-model="time1"
            value="9:41"
            full-width
          >
            <v-spacer />
            <v-btn
              flat
              color="primary"
              @click="modal = false"
            >
              Cancel
            </v-btn>
            <v-btn
              flat
              color="primary"
              @click="$refs.dialog.save(time1)"
            >
              OK
            </v-btn>
          </v-time-picker>
        </v-dialog>
      </core-section>

      <core-title>
        In menu
      </core-title>
      <core-section center>
        <v-menu
          ref="menu"
          v-model="menu"
          :close-on-content-click="false"
          :nudge-right="40"
          :return-value.sync="time2"
          transition="scale-transition"
          offset-y
          full-width
          max-width="290px"
          min-width="290px"
        >
          <template #activator>
            <v-text-field
              v-model="time2"
              label="Picker in menu"
              prepend-icon="mdi-clock-outline"
              readonly
            />
          </template>
          <v-time-picker
            v-if="menu"
            v-model="time2"
            full-width
            @change="$refs.menu.save(time2)"
          />
        </v-menu>
      </core-section>
    </v-layout>
  </v-container>
</template>

<script>
  export default {
    name: 'TimePickers',

    data: () => ({
      modal: false,
      menu: false,
      time1: '9:41',
      time2: '9:41',
    }),
  }
</script>
