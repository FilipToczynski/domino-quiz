<script>
  export let count;
  export let answers;

  // COUNTER AND WILL STOP AFTER 21
  function AddToCount() {
    function stopCount() {
      count = 0;
    }
    count += 1;
    if (count === 22) {
      stopCount();
    }
  }

  // WIPE CLEAN ALL THE ANSWERS AFTER CLICKING NEXT BUTTON
  function clearAnswers(e) {
    e.preventDefault();

    document.getElementById("firstAnswer").style.backgroundColor =
      "transparent";
    document.getElementById("secondAnswer").style.backgroundColor =
      "transparent";
    document.getElementById("thirdAnswer").style.backgroundColor =
      "transparent";
    document.getElementById("fourthAnswer").style.backgroundColor =
      "transparent";
  }

  // VALIDATE ANWSER AND COLOR ACCORDINGLY
  function checkAnswer(e) {
    e.preventDefault();

    function correctAnswer(e) {
      e.preventDefault();
      document.getElementById(e.target.id).style.backgroundColor =
        "rgba(151,255,132,1)";
    }

    function wrongAnswer(e) {
      e.preventDefault();
      document.getElementById(e.target.id).style.backgroundColor = "#ff0800";
    }

    // ANSWERS
    count === 0 && e.target.value == answers.A[1] // MARGHERITA
      ? correctAnswer(e)
      : count === 0 && e.target.value == answers.B[1]
      ? wrongAnswer(e)
      : count === 0 && e.target.value == answers.C[1]
      ? wrongAnswer(e)
      : count === 0 && e.target.value == answers.D[1]
      ? wrongAnswer(e)
      : count === 1 && e.target.value == answers.A[2] // PEPPERONI
      ? wrongAnswer(e)
      : count === 1 && e.target.value == answers.B[2]
      ? wrongAnswer(e)
      : count === 1 && e.target.value == answers.C[2]
      ? wrongAnswer(e)
      : count === 1 && e.target.value == answers.D[2]
      ? correctAnswer(e)
      : count === 2 && e.target.value == answers.A[3] // FARMHOUSE
      ? wrongAnswer(e)
      : count === 2 && e.target.value == answers.B[3]
      ? correctAnswer(e)
      : count === 2 && e.target.value == answers.C[3]
      ? wrongAnswer(e)
      : count === 2 && e.target.value == answers.D[3]
      ? wrongAnswer(e)
      : count === 3 && e.target.value == answers.A[4] // HAWAJSKA
      ? wrongAnswer(e)
      : count === 3 && e.target.value == answers.B[4]
      ? wrongAnswer(e)
      : count === 3 && e.target.value == answers.C[4]
      ? correctAnswer(e)
      : count === 3 && e.target.value == answers.D[4]
      ? wrongAnswer(e)
      : count === 4 && e.target.value == answers.A[5] // CARBONARA
      ? correctAnswer(e)
      : count === 4 && e.target.value == answers.B[5]
      ? wrongAnswer(e)
      : count === 4 && e.target.value == answers.C[5]
      ? wrongAnswer(e)
      : count === 4 && e.target.value == answers.D[5]
      ? wrongAnswer(e)
      : count === 5 && e.target.value == answers.A[6] // VESUVIO
      ? wrongAnswer(e)
      : count === 5 && e.target.value == answers.B[6]
      ? correctAnswer(e)
      : count === 5 && e.target.value == answers.C[6]
      ? wrongAnswer(e)
      : count === 5 && e.target.value == answers.D[6]
      ? wrongAnswer(e)
      : count === 6 && e.target.value == answers.A[7] // DOUBLE BACON BURGER
      ? wrongAnswer(e)
      : count === 6 && e.target.value == answers.B[7]
      ? wrongAnswer(e)
      : count === 6 && e.target.value == answers.C[7]
      ? correctAnswer(e)
      : count === 6 && e.target.value == answers.D[7]
      ? wrongAnswer(e)
      : count === 7 && e.target.value == answers.A[8] // CAPRICCIOSA
      ? wrongAnswer(e)
      : count === 7 && e.target.value == answers.B[8]
      ? correctAnswer(e)
      : count === 7 && e.target.value == answers.C[8]
      ? wrongAnswer(e)
      : count === 7 && e.target.value == answers.D[8]
      ? wrongAnswer(e)
      : count === 8 && e.target.value == answers.A[9] // VEGETARIANA
      ? correctAnswer(e)
      : count === 8 && e.target.value == answers.B[9]
      ? wrongAnswer(e)
      : count === 8 && e.target.value == answers.C[9]
      ? wrongAnswer(e)
      : count === 8 && e.target.value == answers.D[9]
      ? wrongAnswer(e)
      : count === 9 && e.target.value == answers.A[10] // DIAVOLA
      ? wrongAnswer(e)
      : count === 9 && e.target.value == answers.B[10]
      ? wrongAnswer(e)
      : count === 9 && e.target.value == answers.C[10]
      ? wrongAnswer(e)
      : count === 9 && e.target.value == answers.D[10]
      ? correctAnswer(e)
      : count === 10 && e.target.value == answers.A[11] // NEW YORKER
      ? correctAnswer(e)
      : count === 10 && e.target.value == answers.B[11]
      ? wrongAnswer(e)
      : count === 10 && e.target.value == answers.C[11]
      ? wrongAnswer(e)
      : count === 10 && e.target.value == answers.D[11]
      ? wrongAnswer(e)
      : count === 11 && e.target.value == answers.A[12] // AMERICANA
      ? wrongAnswer(e)
      : count === 11 && e.target.value == answers.B[12]
      ? correctAnswer(e)
      : count === 11 && e.target.value == answers.C[12]
      ? wrongAnswer(e)
      : count === 11 && e.target.value == answers.D[12]
      ? wrongAnswer(e)
      : count === 12 && e.target.value == answers.A[13] // KEBAB
      ? wrongAnswer(e)
      : count === 12 && e.target.value == answers.B[13]
      ? wrongAnswer(e)
      : count === 12 && e.target.value == answers.C[13]
      ? correctAnswer(e)
      : count === 12 && e.target.value == answers.D[13]
      ? wrongAnswer(e)
      : count === 13 && e.target.value == answers.A[14] // CONTADINA
      ? correctAnswer(e)
      : count === 13 && e.target.value == answers.B[14]
      ? wrongAnswer(e)
      : count === 13 && e.target.value == answers.C[14]
      ? wrongAnswer(e)
      : count === 13 && e.target.value == answers.D[14]
      ? wrongAnswer(e)
      : count === 14 && e.target.value == answers.A[15] // QUATRO CARNI
      ? wrongAnswer(e)
      : count === 14 && e.target.value == answers.B[15]
      ? wrongAnswer(e)
      : count === 14 && e.target.value == answers.C[15]
      ? wrongAnswer(e)
      : count === 14 && e.target.value == answers.D[15]
      ? correctAnswer(e)
      : count === 15 && e.target.value == answers.A[16] // VEGGIE SUPREME
      ? wrongAnswer(e)
      : count === 15 && e.target.value == answers.B[16]
      ? correctAnswer(e)
      : count === 15 && e.target.value == answers.C[16]
      ? wrongAnswer(e)
      : count === 15 && e.target.value == answers.D[16]
      ? wrongAnswer(e)
      : count === 16 && e.target.value == answers.A[17] // TEXAS BBQ
      ? wrongAnswer(e)
      : count === 16 && e.target.value == answers.B[17]
      ? wrongAnswer(e)
      : count === 16 && e.target.value == answers.C[17]
      ? wrongAnswer(e)
      : count === 16 && e.target.value == answers.D[17]
      ? correctAnswer(e)
      : count === 17 && e.target.value == answers.A[18] // QUATRO CHEESE
      ? correctAnswer(e)
      : count === 17 && e.target.value == answers.B[18]
      ? wrongAnswer(e)
      : count === 17 && e.target.value == answers.C[18]
      ? wrongAnswer(e)
      : count === 17 && e.target.value == answers.D[18]
      ? wrongAnswer(e)
      : count === 18 && e.target.value == answers.A[19] // TOSCANA
      ? wrongAnswer(e)
      : count === 18 && e.target.value == answers.B[19]
      ? wrongAnswer(e)
      : count === 18 && e.target.value == answers.C[19]
      ? correctAnswer(e)
      : count === 18 && e.target.value == answers.D[19]
      ? wrongAnswer(e)
      : count === 19 && e.target.value == answers.A[20] // PARADISO PIMONTESE
      ? wrongAnswer(e)
      : count === 19 && e.target.value == answers.B[20]
      ? wrongAnswer(e)
      : count === 19 && e.target.value == answers.C[20]
      ? correctAnswer(e)
      : count === 19 && e.target.value == answers.D[20]
      ? wrongAnswer(e)
      : count === 20 && e.target.value == answers.A[21] // EXTRAVAGANZZA
      ? correctAnswer(e)
      : count === 20 && e.target.value == answers.B[21]
      ? wrongAnswer(e)
      : count === 20 && e.target.value == answers.C[21]
      ? wrongAnswer(e)
      : count === 20 && e.target.value == answers.D[21]
      ? wrongAnswer(e)
      : count === 21 && e.target.value == answers.A[22] // BIANCO VERDE
      ? wrongAnswer(e)
      : count === 21 && e.target.value == answers.B[22]
      ? wrongAnswer(e)
      : count === 21 && e.target.value == answers.C[22]
      ? wrongAnswer(e)
      : count === 21 && e.target.value == answers.D[22]
      ? correctAnswer(e)
      : "";
  }
</script>

<main>
  <div class="container">
    <div class="counter">
      <h2>{count} / 21</h2>
      <h1>
        {count === 0
          ? "Margherita"
          : count === 1
          ? "Pepperoni"
          : count === 2
          ? "Farmhouse"
          : count === 3
          ? "Hawajska"
          : count === 4
          ? "Carbonara"
          : count == 5
          ? "Vesuvio"
          : count === 6
          ? "Bacon Burger"
          : count === 7
          ? "Capricciosa"
          : count === 8
          ? "Vegetariana"
          : count === 9
          ? "Diavola"
          : count === 9
          ? "Montanara"
          : count === 10
          ? "New Yorker"
          : count === 11
          ? "Americana"
          : count === 12
          ? "Kebab"
          : count === 13
          ? "Contadina"
          : count === 14
          ? "Quatro Carni"
          : count === 15
          ? "Veggie Supreme"
          : count === 16
          ? "Texas BBQ"
          : count === 17
          ? "Quatro Cheese"
          : count === 18
          ? "Toscana"
          : count === 19
          ? "Paradiso"
          : count === 20
          ? "Extravaganzza"
          : count === 21
          ? "Bianco Verde"
          : ""}
      </h1>
    </div>
    <div class="answers">
      <div class="answers__check">
        <input
          id="firstAnswer"
          class="button"
          type="button"
          value={count === 0
            ? answers.A[1]
            : count === 1
            ? answers.A[2]
            : count === 2
            ? answers.A[3]
            : count === 3
            ? answers.A[4]
            : count === 4
            ? answers.A[5]
            : count === 5
            ? answers.A[6]
            : count === 6
            ? answers.A[7]
            : count === 7
            ? answers.A[8]
            : count === 8
            ? answers.A[9]
            : count === 9
            ? answers.A[10]
            : count === 10
            ? answers.A[11]
            : count === 11
            ? answers.A[12]
            : count === 12
            ? answers.A[13]
            : count === 13
            ? answers.A[14]
            : count === 14
            ? answers.A[15]
            : count === 15
            ? answers.A[16]
            : count === 16
            ? answers.A[17]
            : count === 17
            ? answers.A[18]
            : count === 18
            ? answers.A[19]
            : count === 19
            ? answers.A[20]
            : count === 20
            ? answers.A[21]
            : count === 21
            ? answers.A[22]
            : ""}
          on:click={checkAnswer}
        />
      </div>

      <div class="answers__check">
        <input
          id="secondAnswer"
          class="button"
          type="button"
          value={count === 0
            ? answers.B[1]
            : count === 1
            ? answers.B[2]
            : count === 2
            ? answers.B[3]
            : count === 3
            ? answers.B[4]
            : count === 4
            ? answers.B[5]
            : count === 5
            ? answers.B[6]
            : count === 6
            ? answers.B[7]
            : count === 7
            ? answers.B[8]
            : count === 8
            ? answers.B[9]
            : count === 9
            ? answers.B[10]
            : count === 10
            ? answers.B[11]
            : count === 11
            ? answers.B[12]
            : count === 12
            ? answers.B[13]
            : count === 13
            ? answers.B[14]
            : count === 14
            ? answers.B[15]
            : count === 15
            ? answers.B[16]
            : count === 16
            ? answers.B[17]
            : count === 17
            ? answers.B[18]
            : count === 18
            ? answers.B[19]
            : count === 19
            ? answers.B[20]
            : count === 20
            ? answers.B[21]
            : count === 21
            ? answers.B[22]
            : ""}
          on:click={checkAnswer}
        />
      </div>

      <div class="answers__check">
        <input
          id="thirdAnswer"
          class="button"
          type="button"
          value={count === 0
            ? answers.C[1]
            : count === 1
            ? answers.C[2]
            : count === 2
            ? answers.C[3]
            : count === 3
            ? answers.C[4]
            : count === 4
            ? answers.C[5]
            : count === 5
            ? answers.C[6]
            : count === 6
            ? answers.C[7]
            : count === 7
            ? answers.C[8]
            : count === 8
            ? answers.C[9]
            : count === 9
            ? answers.C[10]
            : count === 10
            ? answers.C[11]
            : count === 11
            ? answers.C[12]
            : count === 12
            ? answers.C[13]
            : count === 13
            ? answers.C[14]
            : count === 14
            ? answers.C[15]
            : count === 15
            ? answers.C[16]
            : count === 16
            ? answers.C[17]
            : count === 17
            ? answers.C[18]
            : count === 18
            ? answers.C[19]
            : count === 19
            ? answers.C[20]
            : count === 20
            ? answers.C[21]
            : count === 21
            ? answers.C[22]
            : ""}
          on:click={checkAnswer}
        />
      </div>

      <div class="answers__check">
        <input
          id="fourthAnswer"
          class="button"
          type="button"
          value={count === 0
            ? answers.D[1]
            : count === 1
            ? answers.D[2]
            : count === 2
            ? answers.D[3]
            : count === 3
            ? answers.D[4]
            : count === 4
            ? answers.D[5]
            : count === 5
            ? answers.D[6]
            : count === 6
            ? answers.D[7]
            : count === 7
            ? answers.D[8]
            : count === 8
            ? answers.D[9]
            : count === 9
            ? answers.D[10]
            : count === 10
            ? answers.D[11]
            : count === 11
            ? answers.D[12]
            : count === 12
            ? answers.D[13]
            : count === 13
            ? answers.D[14]
            : count === 14
            ? answers.D[15]
            : count === 15
            ? answers.D[16]
            : count === 16
            ? answers.D[17]
            : count === 17
            ? answers.D[18]
            : count === 18
            ? answers.D[19]
            : count === 19
            ? answers.D[20]
            : count === 20
            ? answers.D[21]
            : count === 21
            ? answers.D[22]
            : ""}
          on:click={checkAnswer}
        />
      </div>
      <div class="container" />
      <button
        class="submitAnswer"
        id="ClearAll"
        type="submit"
        on:click={AddToCount}
        on:click={checkAnswer}
        on:click={clearAnswers}>NEXT</button
      >
    </div>
  </div>
</main>

<style>
  #fourthAnswer {
    word-break: break-all;
  }
  .counter {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    grid-row: first / second;
  }
  .submitAnswer {
    margin-top: 2rem;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
    grid-column: third / sixth;
    width: 100%;
    height: 2.5rem;
    border-radius: 3px;
    background: #d2d0ff15;
    animation: all 3s ease-in-out;
  }
  .submitAnswer:hover {
    box-shadow: .2px .2px 0px 0px #000;
    transform: scale(1.01);
  }
  .submitAnswer:active {
    transform: scale(1);
  }
  .button {
    font-family: "Montserrat", sans-serif;
    height: 100%;
    width: 100%;
    cursor: pointer;
    border: 1px solid black;
    border-radius: 3px;
    background-color: transparent;
    padding: 0;
    white-space: normal;
  }

  .button:hover {
    background-color: #f1f1f1;
  }

  .button:active {
    background-color: #e4e4e4;
  }
  .counter {
    font-family: "Montserrat", sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    grid-column: first / eight;
    width: 100%;
    top: 0;
  }
  .answers {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    grid-column: second / seventh;
    grid-row: second / fourth;
    width: 100%;
  }

  .answers__check {
    display: flex;
    align-items: center;
    justify-content: center;
    grid-column: first / eight;
    width: 100%;
    margin-top: 1rem;
    height: 3rem;
    cursor: pointer;
    font-size: 0.6rem;
  }
  
  .container {
    display: grid;
    grid-template-columns: [first] 1fr [second] 1fr [third] 1fr [fourth] 1fr [fifth] 1fr [sixth] 1fr [seventh] 1fr [eight];
    grid-template-rows: [first] 1fr [second] 1fr [third] 1fr [fourth] 1fr;
    grid-auto-columns: 12fr;
    grid-auto-rows: 1fr;
    gap: 0px 0px;
    grid-auto-flow: column;
    justify-items: center;
    align-items: center;
  }

  @media only screen and (max-width: 950px) {
    .answers__check {
      grid-column: second / seventh;
      font-size: 0.2rem;
    }
    .answers__check input {
      font-size: 0.6rem;
    }
    .answers {
      grid-column: second / seventh;
    }

    .counter {
      grid-row: first / second;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }
    .counter h1 {
      margin: 2rem;
    }
    .answers {
      grid-row: second / fourth;
    }
  }
  /* @media only screen and (max-width: 1800px) {
    .answers__check {
      font-size: 0.6rem;
    }
  } */
</style>
