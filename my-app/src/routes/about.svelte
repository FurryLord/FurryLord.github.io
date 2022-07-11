<!-- <script lang="ts">

</script> -->
<script context="module">
  import { browser, dev } from "$app/env";

  // we don't need any JS on this page, though we'll load
  // it in dev so that we get hot module replacement...
  export const hydrate = dev;

  // ...but if the client-side router is already loaded
  // (i.e. we came here from elsewhere in the app), use it
  export const router = browser;

  // since there's no dynamic data here, we can prerender
  // it so that it gets served as a static asset in prod
  export const prerender = true;
</script>

<main>
  <div class="wrapper">
    <div class="row">
      <div class="col span4 box">
        <h2>Education</h2>
        <ul>
          <li>
            School:
            <ul>
              <li>Lyceum №7, Kstovo, Nizhny Novgorod region, 2010-2021</li>
            </ul>
          </li>
          <br />
          <li>
            University:
            <ul>
              <li>
                Innopolis University, Innopolis, Republic of Tatarstan,
                2021-2025
              </li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col span4 box">
        <h2>Grades</h2>
        <ul>
          <li>
            First semester:
            <ul>
              <li>Philosophy - A</li>
              <li>Fundamentals of Computer Architecture - A</li>
              <li>Introduction to Programming I - B</li>
              <li>Analitical Geometry and Linear Algebra I - B</li>
              <li>Mathematical Analysis I - B</li>
              <li>Foreign Language - B</li>
            </ul>
          </li>
          <br />
          <li>
            Second semester:
            <ul>
              <li>Data Structures and Algorithms - A</li>
              <li>Software Systems Analysis and Design - A</li>
              <li>Foreign Language - A</li>
              <li>Mathematical Analysis II - A</li>
              <li>Theoretical Computer Science - B</li>
              <li>Analitical Geometry and Linear Algebra II - B</li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="col span4 box">
        <h2>Skills</h2>
        <ul>
          <li>
            Hard skills:
            <ul>
              <li>Basic knowledge of C++, Java, Python</li>
              <li>
                Knowledge of HTML&CSS&JS (it wll be higher after finishing FWD
                cource)
              </li>
              <li>Git, GitHub</li>
            </ul>
          </li>
          <br />
          <li>
            Soft skills:
            <ul>
              <li>Time management</li>
              <li>Focus</li>
              <li>Empathy</li>
              <li>Enthusiasm</li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </div>
</main>

<style>
  h2{
    margin-left: 5%;
  }
  li {
    margin-right: 5%;
    margin-left: 5%;
    list-style-type: square;
  }

  li li {
    list-style-type: circle;
  }
  .box {
    background-color: #7f55db;
    border-radius: 15px;
    word-break: break-word;
    max-height: 700px;
    padding-top: 1%;
    overflow: auto;
  }
  
</style> 
