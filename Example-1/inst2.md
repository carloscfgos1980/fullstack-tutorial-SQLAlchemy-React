app.js:
11. Import 
import React, { useState, useEffect } from "react";

12. const that will handle the data
  const [data, setData] = useState([{}])

13. useEffect to fecth the data from the backend
  useEffect(() => {
    fetch("/members").then(
      res => res.json()
    ).then(
      data => {
        setData(data)
        console.log(data)
      }
    )
  }, [])


14. Loop thru the array feteched and unsing a binary comparison to display a message in case there is no data:

        {(typeof data.members === "undefined") ? (
        <p>loading...</p>
      ) : (
        data.members.map((member, i) => (
          <p key={i}>{member}</p>
        ))
      )
      }


# THE END