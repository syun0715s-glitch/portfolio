<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>TODOアプリ</title>

  <!-- アイコン -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

  <!-- CSS -->
  <link rel="stylesheet" href="style.css">
</head>

<style>
/* ===== リセット ===== */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:sans-serif;
    min-height:100vh;
    background:linear-gradient(135deg,#dbeafe,#eef2ff,#f8fafc);
    display:flex;
    justify-content:center;
    align-items:flex-start;
    padding:40px 20px;
}

/* ===== メインカード ===== */

.container{

    width:100%;
    max-width:1000px;

    background:rgba(255,255,255,.8);

    backdrop-filter:blur(18px);

    border-radius:30px;

    padding:40px;

    box-shadow:0 20px 60px rgba(0,0,0,.15);

}

/* ===== タイトル ===== */

header{

    text-align:center;

    margin-bottom:35px;

}

header h1{

    font-size:48px;

    color:#2563eb;

    margin-bottom:10px;

}

header p{

    font-size:20px;

    color:#555;

}

/* ===== 入力欄 ===== */

.input-area{

    display:flex;

    gap:15px;

    margin-bottom:25px;

}

.input-area input{

    flex:1;

    padding:18px;

    border:2px solid #d1d5db;

    border-radius:16px;

    font-size:20px;

    outline:none;

    transition:.3s;

}

.input-area input:focus{

    border-color:#2563eb;

    box-shadow:0 0 10px rgba(37,99,235,.3);

}

#addBtn{

    background:#2563eb;

    color:white;

}

button{

    border:none;

    border-radius:16px;

    cursor:pointer;

    padding:18px 24px;

    font-size:18px;

    transition:.25s;

}

button:hover{

    transform:translateY(-3px);

}

/* ===== ボタン列 ===== */

.menu{

    display:flex;

    gap:15px;

    margin-bottom:30px;

}

.menu button{

    flex:1;

    color:white;

}

.green{

    background:#22c55e;

}

.orange{

    background:#f59e0b;

}

.purple{

    background:#7c3aed;

}

/* ===== フィルター ===== */

.filters{
    display:flex;
    align-items:center;
    gap:12px;
    flex-wrap:wrap;
    margin-bottom:30px;
}

.filters button{
    background:#e5e7eb;
    color:#333;
    padding:12px 20px;
    border-radius:12px;
}

.filters button.active{
    background:#2563eb;
    color:#fff;
}

.count{
    margin-left:auto;
    font-size:18px;
    font-weight:bold;
    color:#444;
}

/* ===== タスクリスト ===== */

#taskList{
    list-style:none;
}

#taskList li{

    display:flex;
    align-items:center;
    gap:15px;

    background:white;

    margin-bottom:18px;

    padding:20px;

    border-radius:18px;

    box-shadow:0 8px 20px rgba(0,0,0,.08);

    transition:.3s;

}

#taskList li:hover{

    transform:translateY(-3px);

}

.task-text{

    flex:1;

    font-size:20px;

    word-break:break-word;

}

/* ===== 完了状態 ===== */

.done{

    text-decoration:line-through;

    color:#888;

    opacity:.7;

}

/* ===== ボタン ===== */

.done-btn{

    background:#22c55e;

    color:white;

}

.edit-btn{

    background:#3b82f6;

    color:white;

}

.delete-btn{

    background:#ef4444;

    color:white;

}

/* ===== アニメーション ===== */

@keyframes fadeIn{

    from{

        opacity:0;

        transform:translateY(20px);

    }

    to{

        opacity:1;

        transform:translateY(0);

    }

}

#taskList li{

    animation:fadeIn .3s ease;

}

/* ===== スマホ対応 ===== */

@media(max-width:768px){

.container{

padding:25px;

}

header h1{

font-size:34px;

}

header p{

font-size:16px;

}

.input-area{

flex-direction:column;

}

.input-area input{

width:100%;

font-size:18px;

}

#addBtn{

width:100%;

}

.menu{

flex-direction:column;

}

.filters{

flex-direction:column;

align-items:stretch;

}

.count{

margin-left:0;

text-align:center;

}

#taskList li{

flex-direction:column;

align-items:stretch;

}

.task-text{

text-align:center;

margin-bottom:10px;

}

.done-btn,
.edit-btn,
.delete-btn{

width:100%;

margin-top:8px;

}

}
</style>

<body>

<div class="container">

  <header>
    <h1><i class="fa-solid fa-clipboard-check"></i> TODOアプリ</h1>
    <p>タスクを管理して効率アップ！</p>
  </header>

  <div class="input-area">
    <input
      type="text"
      id="taskInput"
      placeholder="やることを入力してください..."
    >

    <button id="addBtn">
      <i class="fa-solid fa-plus"></i>
      追加
    </button>
  </div>

  <div class="menu">

    <button id="apiBtn" class="green">
      <i class="fa-solid fa-cloud-arrow-down"></i>
      API取得
    </button>

    <button id="weatherBtn" class="orange">
      <i class="fa-solid fa-sun"></i>
      天気
    </button>

    <button id="deleteAllBtn" class="purple">
      <i class="fa-solid fa-trash"></i>
      全削除
    </button>

  </div>

  <div class="filters">

    <button data-filter="all" class="active">
      すべて
    </button>

    <button data-filter="todo">
      未完了
    </button>

    <button data-filter="done">
      完了
    </button>

    <div class="count">
      タスク数：
      <span id="count">0</span>
    </div>

  </div>

  <ul id="taskList"></ul>

</div>

<script src="script.js"></script>

</body>

<script>

// ===== 要素取得 =====

const input = document.getElementById("taskInput");
const addBtn = document.getElementById("addBtn");
const taskList = document.getElementById("taskList");
const count = document.getElementById("count");

// ===== タスク配列 =====

let tasks = JSON.parse(localStorage.getItem("tasks")) || [];

// ===== 保存 =====

function saveTasks(){
    localStorage.setItem("tasks", JSON.stringify(tasks));
}

// ===== 件数更新 =====

function updateCount(){
    count.textContent = tasks.length;
}

// ===== 画面更新 =====

function renderTasks(){

    taskList.innerHTML = "";

    tasks.forEach((task,index)=>{

        const li = document.createElement("li");

        const span = document.createElement("span");
        span.className = "task-text";
        span.textContent = task.text;

        if(task.done){
            span.classList.add("done");
        }

        // 完了ボタン
        const doneBtn = document.createElement("button");
        doneBtn.textContent = "✓";
        doneBtn.className = "done-btn";

        doneBtn.addEventListener("click",()=>{

            tasks[index].done = !tasks[index].done;

            saveTasks();

            renderTasks();

        });

        // 削除ボタン
        const deleteBtn = document.createElement("button");
        deleteBtn.textContent = "削除";
        deleteBtn.className = "delete-btn";

        deleteBtn.addEventListener("click",()=>{

            tasks.splice(index,1);

            saveTasks();

            renderTasks();

        });

        li.appendChild(span);
        li.appendChild(doneBtn);
        li.appendChild(deleteBtn);

        taskList.appendChild(li);

    });

    updateCount();

}

// ===== タスク追加 =====

function addTask(){

    const text = input.value.trim();

    if(text===""){

        alert("入力してください");

        return;

    }

    tasks.push({

        text:text,

        done:false

    });

    saveTasks();

    renderTasks();

    input.value="";

    input.focus();

}

// ボタンクリック
addBtn.addEventListener("click",addTask);

// Enterキー
input.addEventListener("keydown",(e)=>{

    if(e.key==="Enter"){

        addTask();

    }

});

// 初回表示
renderTasks();

</script>

</body>
</html>
