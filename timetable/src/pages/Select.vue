<template>
<form style="width: 500px; margin: 5px">
  <q-select
    :display-value="text"
    v-model="select"
    float-label="Факультет:"
    :options="selectFacultyOptions"
  />
  <q-select
    v-model="select"
    float-label="Курс:"
    :options="selectCourseOptions"
  />
  <q-select
    v-model="select"
    float-label="Специальность:"
    :options="selectSpecialtyOptions"
  />
  <q-select
    v-model="select"
    float-label="Группа:"
    :options="selectGroupOptions"
  />
  <q-btn class="but" label="Показать" />
</form>
</template>

<script>
export default {
  data () {
    return {
      selectFacultyOptions: [
        {
          label: 'Биологический',
          value: 'bio'
        },
        {
          label: 'Геолого-географический факультет',
          value: 'geo'
        },
        {
          label: 'Исторический факультет',
          value: 'his'
        },
        {
          label: 'Факультет иностранных языков',
          value: 'for'
        },
        {
          label: 'Факультет математики и технологий программирования',
          value: 'mat'
        },
        {
          label: 'Факультет психологии и педагогики',
          value: 'psy'
        },
        {
          label: 'Факультет физики и информационных технологий',
          value: 'phy'
        },
        {
          label: 'Факультет физической культуры',
          value: 'cul'
        },
        {
          label: 'Филологический факультет',
          value: 'phi'
        },
        {
          label: 'Экономический факультет',
          value: 'eco'
        },
        {
          label: 'Юридический факультет',
          value: 'law'
        }
      ],
      selectCourseOptions: [
        {
          label: '1',
          value: 'first'
        },
        {
          label: '2',
          value: 'second'
        },
        {
          label: '3',
          value: 'third'
        },
        {
          label: '4',
          value: 'fourth'
        },
        {
          label: '5',
          value: 'fifth'
        }
      ],
      selectSpecialtyOptions: [
        {
          label: '1',
          value: 'first'
        },
        {
          label: '2',
          value: 'second'
        },
        {
          label: '3',
          value: 'third'
        },
        {
          label: '4',
          value: 'fourth'
        },
        {
          label: '5',
          value: 'fifth'
        }
      ],
      selectGroupOptions: [
        {
          label: '1',
          value: 'first'
        },
        {
          label: '2',
          value: 'second'
        },
        {
          label: '3',
          value: 'third'
        },
        {
          label: '4',
          value: 'fourth'
        },
        {
          label: '5',
          value: 'fifth'
        }
      ]
    }
  }
}
</script>
