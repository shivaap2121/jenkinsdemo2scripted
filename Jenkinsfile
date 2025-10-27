node{
    try{
        stage("Checkout code"){
            checkout scm
        }
        stage("Extract Pipeline"){
            bat "C:\\Users\\shivr\\AppData\\Local\\Programs\\Python\\Python314\\python.exe extract_etl.py"
        }
    }
    catch(err){
        echo "Pipeline error: ${err}"
    }
    finally{
        echo "Pipeline completed"
    }
}