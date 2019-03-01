# use-timer

Simple timer hook for React.

Install it with npm:

```
npm i use-timer --save
```

## Simple timer

```javascript
import React from 'react';
import { useTimer } from 'use-timer';

const App = () => {
  const { time, start, pause, reset } = useTimer();

  return (
    <React.Fragment>
      <div>
        <button onClick={start}>Start</button>
        <button onClick={pause}>Pause</button>
        <button onClick={reset}>Reset</button>
      </div>
      <p>Elapsed time: {time}</p>
    </React.Fragment>
  );
};
```
