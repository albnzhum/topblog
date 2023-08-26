<template>
    <main class="page">
        <div class="page_main-block">
            <div class="main-block_body">
                <div class="main-block_header">
                    <h1>Загрузка завершена</h1>
                </div>
                <div class="content">
                    <div class="table">
                        <Table></Table>
                    </div>
                    <div class="information">
                        <div class="white-button">
                            <p class="info-label">Площадка</p>
                            <div class="social">ВКонтакте</div>
                        </div>
                        <div class="white-button">
                            <p class="info-label">Загружено всего</p>
                            <div class="count-uploaded">30 000 фото</div>
                        </div>
                        <div class="white-button">
                            <p class="info-label">Корректно обработано</p>
                            <div class="count-correctly">29 999 фото</div>
                        </div>
                        <div class="white-button">
                            <p class="info-label">Некорректно обработано</p>
                            <div class="count-incorrectly">1 фото</div>
                        </div>
                        <button class="download" type="button">Скачать таблицу</button>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import Table from '@/components/Table.vue';
export default {
    components: {
        Table
    },
}
</script>

<style>
.main-block_body {
    display: flex;
    flex-direction: column;
    justify-content: center;
    justify-items: center;
    padding-left: 30%;
    padding-right: 30%;
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


/*---TABLE + INFORMATION---- */

.content {
    display: flex;
    justify-content: center;
    justify-items: center;
    flex-direction: row;
    gap: 150px;
    padding-top: 10%;
}


.white-button {
    padding-bottom: 15%;
}

.info-label {
    color: rgba(42, 38, 38, 0.60);
    font-size: 13px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
}

/*---SOCIAL NETWORK--- */

.social {
    display: flex;
    padding: 12px 24px;
    justify-content: center;
    align-items: center;
    gap: 5px;
    border-radius: 4px;
    background: #4663AB;
    color: white;
}

/*---BUTTON TEXT--- */
.count-uploaded,
.count-correctly,
.count-incorrectly {
    display: flex;
    padding: 20px 40px;
    justify-content: center;
    align-items: center;
    border-radius: 15px;
    background: #FFF;
    box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.05);

    /*----TEXT----- */

    color: #4663AB;
    font-size: 20px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    white-space: nowrap;
}

/*---DOWNLOAD-BUTTON--- */
.download {
    display: inline-flex;
    padding: 18px 35px;
    justify-content: center;
    align-items: center;
    gap: 10px;
    border-radius: 8px;
    border: 1px solid rgba(0, 0, 0, 0.10);
    background: #4663AB;
    color: white;
    box-shadow: 0px 1px 1px 0px rgba(0, 0, 0, 0.16);

    font-size: 14px;
    font-style: normal;
    font-weight: 500;
    line-height: normal;
    text-transform: uppercase;
    white-space: nowrap;
}
</style>