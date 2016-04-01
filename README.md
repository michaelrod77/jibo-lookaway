# Jibo: Look Away

This is a simple skill for the Jibo robot. It allows Jibo to respond to requests to "look away" or "turn around" for a specified amount of time.

This skill was built to solve a simple privacy issue by giving the user direct control to have Jibo hide his cameras for any length of time. This is important for when you need physical privacy or just don't want Jibo staring at you.

## Requirements:

1. Atom Editor
2. Jibo SDK package

## Installation:

Download this package into any folder and open the root in Atom.

## Usage

Run the skill in the Jibo Simulator ( or on the robot if you're lucky enough). Type (or say) "Hey Jibo", then "Look Away" to begin the skill.

Following is a complete breakdown of the skill in action:

1. Jibo starts in idle and listens for "Hey Jibo".
2. After hearing "Hey Jibo", Jibo listens for "Could you look away", "Please turn around for a bit", "Stop looking at me for 5 minutes", "Close your eyes please", or other variations of these requests.
3. After hearing a "look away" request, Jibo will immediately turn around and look away from you.
4. If you didn't supply an amount of time in your request, Jibo then asks "For how long?". Jibo will wait up to 10 seconds for an answer, then turn around for 1 minute if not given a specific amount of time to look away for.
5. Jibo will look away for the time you asked for. After around 30 seconds, he gets border and starts looking around, still keeping his gaze away from you. Occassionally he'll let out a little "chirp" out of pure boredom, unless you said the word "quietly" when asking him to turn around or if you say "be quiet", "quietly please", or "shut up".
6. After he hits the amount of time you asked him to look away for, he turns back around and jumps into idle again waiting for your next request.
