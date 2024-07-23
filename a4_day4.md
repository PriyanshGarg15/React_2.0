![image](https://github.com/user-attachments/assets/057dd0c4-8fc5-4283-985a-5e4973abde28)
![image](https://github.com/user-attachments/assets/121f7c1e-5d6a-48bd-9800-1e10d79e85f0)
![image](https://github.com/user-attachments/assets/b9d36f26-589c-48a0-8897-6109b9bc121f)
![image](https://github.com/user-attachments/assets/ad93e134-3ad8-495d-b59b-046c2788202f)
![image](https://github.com/user-attachments/assets/6e2e1ffa-d9d2-4e23-9e70-a3648194556e)

import React from 'react';
import { Link } from 'react-router-dom';

function App() {
  var x = 100;

  return (
    <div>
      <nav style={{
        width: "100%",
        backgroundColor: "red"
      }}>
        <ul style={{
          padding: 0,
          margin: 0,
          display: 'flex',
          listStyle: 'none',
          justifyContent: 'space-evenly'
        }}>
          <li>
            <Link to="/" style={{
              textDecoration: 'none',
              color: 'white',
              padding: '8px',
              display: 'block',
              fontSize: 18
            }}>Home ({x + 200})</Link>
          </li>
          <li>
            <Link to="/images" style={{
              textDecoration: 'none',
              color: 'white',
              padding: '8px',
              display: 'block',
              fontSize: 18
            }}>Images {x}</Link>
          </li>
          <li>
            <Link to="/videos" style={{
              textDecoration: 'none',
              color: 'white',
              padding: '8px',
              display: 'block',
              fontSize: 18
            }}>Videos ({new Date().toString()})</Link>
          </li>
          <li>
            <Link to="/movies" style={{
              textDecoration: 'none',
              color: 'white',
              padding: '8px',
              display: 'block',
              fontSize: 18
            }}>Movies</Link>
          </li>
          <li>
            <Link to="/contact" style={{
              textDecoration: 'none',
              color: 'white',
              padding: '8px',
              display: 'block',
              fontSize: 18
            }}>Contact us</Link>
          </li>
        </ul>
      </nav>

      <section style={{
        width: '75%',
        padding: 34,
        background: '#f5f5f5',
        margin: '48px auto'
      }}>
        <h1>This is section</h1>
      </section>

      <footer style={{
        background: '#323232',
        textAlign: 'center',
        color: 'white',
        padding: 100
      }}>
        <h1>This is footer</h1>
      </footer>
    </div>
  );
}

export default App;
