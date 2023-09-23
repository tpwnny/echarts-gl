
```bash
npm install echarts
npm install echarts-gl
```

#### all
```js
import * as echarts from 'echarts';
import 'echarts-gl';
```

## Minimal Import
```js
import * as echarts from 'echarts/core';
import { Scatter3DChart } from 'echarts-gl/charts';
import { Grid3DComponent } from 'echarts-gl/components';

echarts.use([Scatter3DChart, Grid3DComponent]);
```

## scripts
```html
<script src="https://cdn.jsdelivr.net/npm/echarts/dist/echarts.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/echarts-gl/dist/echarts-gl.min.js"></script>
```

NOTE:

ECharts GL 2.x is compatible with ECharts 5.x.
ECharts GL 1.x is compatible with ECharts 4.x.



```js
var chart = echarts.init(document.getElementById('main'));
chart.setOption({
    grid3D: {},
    xAxis3D: {},
    yAxis3D: {},
    zAxis3D: {},
    series: [{
        type: 'scatter3D',
        symbolSize: 50,
        data: [[-1, -1, -1], [0, 0, 0], [1, 1, 1]],
        itemStyle: {
            opacity: 1
        }
    }]
})
```

.
