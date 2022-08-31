# m_flask_template
<p>This is a modularized flask template, ready to go.</p>
<p>Template credit and thanks to: rteet702</p>
<p>This template is used with bashrc code to clone the template into a new project directory. 
  To get the full benefit of this template, add the following code snippets to your bashrc file:</p>
  
  ```bash
  function pyi(){
      pipenv install flask PyMySQL flask-bcrypt && echo "-------------------FLASK PYMYSQL BCRYPT AND VIRTUAL ENVIRONMENT CREATED-------------------"
  }
  export -f pyi
  
  function gitmflasktemplate(){
      mkdir $1 && echo "------------------- CREATING NEW PROJECT DIRECTORY -------------------"
      cd $1 && echo "------------------- CHANGING INTO PROJECT DIRECTORY -------------------"
      git clone https://github.com/code-Brian/m_flask_template.git && echo "------------------- GIT REPO CLONED -------------------"
      rm -r .git && echo "------------------- GIT FILE DELETED -------------------"
      pyi
  }
  export -f gitmflasktemplate
  ```
<p> I hope this template is helpful. Please ping myself or Robert (https://github.com/rteet702) if there are any questions!</p>
