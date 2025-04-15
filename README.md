# PowerPath Typescript

Please refer to the official documentation here: https://1edtech-alpha.stoplight.io/docs/1edtech/awfxqyww6zbmu-power-path

## Usage

The PowerPath Typescript client is directly modelled off the official PowerPath API, with operations tied to the specification.

### Creating the client:

```js
import { DefaultApi as PowerPathAPI} from '@powerpath/ts'
import { CoursesAPI } from '@powerpath/ts'
```

### Using operations:
```js
const course = await CoursesAPI.coursesControllerFindAll();
const lesson = await PowerPathAPI.getNextLessonByCourseAndUser(103123, courses[0].id)
```