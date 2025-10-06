CSS FOR COUNTER APP
===================
body {
  margin: 0;
  padding: 0;
  font-family: 'Poppins', sans-serif;
  background:linear-gradient(135deg, #6a11cb, #2575fc);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

/* Wrapper styling */
h1 {
  font-size: 2.5rem;
  color: #fff;
  text-align: center;
  margin-bottom: 1.5rem;
  letter-spacing: 1px;
  text-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
  background: rgba(255, 255, 255, 0.1);
  padding: 10px 25px;
  border-radius: 12px;
  display: inline-block;
  backdrop-filter: blur(10px);
}

/* Button styling */
button {
  margin: 0 10px;
  padding: 12px 25px;
  font-size: 1rem;
  font-weight: 600;
  border: none;
  border-radius: 30px;
  cursor: pointer;
  background: linear-gradient(135deg, #ffffff, #e0e0e0);
  color: #333;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
  transition: all 0.3s ease;
}

/* Hover effect */
button:hover {
  transform: translateY(-3px) scale(1.05);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
}

/* Individual button colors using nth-child */
button:nth-child(2) { /* increase */
  background: linear-gradient(135deg, #4caf50, #2e7d32);
  color: #fff;
}
button:nth-child(3) { /* decrease */
  background: linear-gradient(135deg, #f44336, #c62828);
  color: #fff;
}
button:nth-child(4) { /* reset */
  background: linear-gradient(135deg, #ff9800, #ef6c00);
  color: #fff;
}

/* Active effect */
button:active {
  transform: translateY(2px);



REACT DEVELOPING CODE FOR COUNTERAPP
===================================
import React, { useState } from 'react'
import './Counterapp.css'


let count;

const Counterapp = () => {
    let [count,setCount]=useState(0)
    
        function increase(){
         setCount(count+1)
        }
          function decrease(){
         setCount(count-1)
        }
          function reset(){
         setCount(0)
        }
    
  return (
    <>
    <h1>🧮countApp-{count}</h1>
    <button onClick={increase}>increase</button>
    <button onClick={decrease}>decrease</button>
    <button onClick={reset}>reset</button>
    </>
  )
}

export default Counterapp
  
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.2);
}
