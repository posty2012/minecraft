# minecraft
Command /fly:
    Permission: yourperm.here
    Trigger:
        If {fly.%player%} is not set:
            Send "&bFlight mode is now &3enabled&b." to player
            set player's flight mode to true
            Set {fly.%player%} to true
            Stop
        Send "&bFlight mode is now &3disabled&b." to player
        set player's flight mode to false
        Delete {fly.%player%}
        Stop
       <img>
