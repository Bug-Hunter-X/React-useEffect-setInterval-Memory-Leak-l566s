# React useEffect setInterval Memory Leak

This repository demonstrates a common mistake in React's `useEffect` hook: using `setInterval` without proper cleanup.  This leads to memory leaks, as the interval continues even after the component is unmounted.

The `bug.js` file shows the problematic code. The `bugSolution.js` file demonstrates the corrected code.

**Key Takeaway:** Always return a cleanup function from `useEffect` when using timers like `setInterval` or `setTimeout` to prevent memory leaks.