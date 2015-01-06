The goal is to read in an array of questions. Those questions will have a key, text (actual question) and an array of answers. Those answers will have values, and next question key.

If someone answers with a specific answer, it will send you to the question specified by the answer.

Example:

```javascript

{
  survey: {
    key: 'Example survey',
    questions: [
      {
        key: 'which color do you like',
        text: 'Which color do you like? (Check all that apply)',
        answers: [
          {
            text: 'Red',
            nextQuestion: 'do you like fire trucks',
            type: 'checkbox'
          },
          {
            text: 'Blue',
            nextQuestion: 'do you like the sky',
            type: 'checkbox'
          },
          {
            text: 'Green',
            nextQuestion: 'do you like snot',
            type: 'checkbox'
          },
          {
            text: 'Brown',
            nextQuestion: 'do you like new jersey beach water',
            type: 'checkbox'
          }
        ]
      },
      {
        key: 'do you like fire trucks',
        text: 'Aren\'t fire trucks the best?',
        answers: [
          {
            text: 'Yes',
            type: 'radio'
          },
          {
            text: 'No',
            type: 'radio'
          }
        ]
      },
      {...}
    ]
  }
}