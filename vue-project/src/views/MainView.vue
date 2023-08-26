<template>
    <main class="page">
        <div class="page_main-block">
            <div class="main-block_body">
                <div class="main-block_header">
                    <h1>Загрузка скриншотов участников</h1>
                    <p>Выберите площадку для расчета ключевых цифровых показателей</p>
                </div>
                <div class="main-block_buttons">
                    <button class="button" type="button">ВКонтакте</button>
                    <button class="button" type="button">Telegram</button>
                    <button class="button" type="button">YouTube</button>
                    <button class="button" type="button">Дзен</button>
                </div>
                <div class="main-block_upload">
                    <img src="../assets/upload-cloud-icon.svg">
                    <div class="upload-content">
                        <h2>Выберите файл или перетащите его </h2>
                        <p>JPG, PNG or PDF, размер не более 10Мб</p>
                        <button class="upload-button" type="button">Выбрать файл</button>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
.main-block_body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    justify-items: center;
    padding-left: 30%;
    padding-right: 30%;
    padding-top: 5%;
    border: 0;
}

/*---TEXT----*/

.main-block_header {
    display: inline-flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

.main-block_header h1 {
    color: #2A2626;
    font-size: 30px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
}

.main-block_header p {
    color: rgba(42, 38, 38, 0.60);
    text-align: center;
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

/*---BUTTONS----*/

.main-block_buttons {
    display: inline-flex;
    align-items: flex-start;
    justify-content: center;
    gap: 16px;
}

.button {
    border-radius: 4px;
    border: none;
    background-color: #FBFDFE;
    color: #D6E0EA;
    display: flex;
    padding: 12px 24px;
    justify-content: center;
    align-items: center;
    gap: 5px;

    /*-----button text styles-------*/
    font-size: 16px;
    font-style: normal;
    font-weight: 600;
    line-height: 100%;
    text-transform: capitalize;
}

.button:focus {
    background-color: #4663AB;
    color: white;
    display: flex;
}

/*---UPLOAD-FILE----*/

.main-block_upload {
    display: flex;
    width: 784px;
    height: 425px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 36px;
    flex-shrink: 0;

    /*----styles------ */
    border-radius: 15px;
    border: 1px dashed rgba(42, 38, 38, 0.25);
}

.main-block_upload img {
    width: 70px;
    height: 70px;
    flex-shrink: 0;
}

.upload-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 18px;
}

.upload-content h2 {
    color: #2A2626;
    font-size: 20px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.upload-content p {
    color: rgba(42, 38, 38, 0.60);
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    margin-block: 0;
    margin-bottom: 35px;
}

.upload-button {
    display: flex;
    padding: 18px 24px;
    align-items: center;
    gap: 15px;

    /*----styles----- */
    border-radius: 8px;
    border: 1px solid #4663AB;
    background: #FBFDFE;

    /*-----text styles----- */
    color: #4663AB;
    font-size: 15px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
    text-transform: uppercase;
}
</style>