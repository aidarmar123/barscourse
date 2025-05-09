<template>
    <main class="main">
        <Breadcrumbs/>
        <div class="culture">
            <div class="container">
                <div class="culture__inner">
                    <h5 class="culture__title">Культура совместной работы</h5>
                    <div class="culture-content">
                        <p class="culture-content__text"><b>Культура совместной работы</b> — это культура, в которой взаимодействие друг с другом происходит постоянно и целенаправленно.</p>
                        <h6 class="culture-content__title">Принципы формирования культуры совместной работы:</h6>
                        <p class="culture-content__text">1. Открытость и обмен знаниями. Чтобы эффективно работать вместе, вашей команде требуется согласовать общие цели и четко представлять порядок работы по их достижению.</p>
                        <p class="culture-content__text">В рамках культуры совместной работы руководители открыто делятся информацией и новостями вне зависимости от того, хорошие они или плохие. Замалчивание неудач или проблем способствует распространению слухов и заставляет сотрудников чувствовать, что им не доверяют.
                            Организации, в которых не обсуждают допущенные ошибки, упускают возможность учиться на них. В культуре совместной работы самое главное заключается не в том, чтобы всегда достигать успеха, а в том, чтобы извлекать уроки из любого опыта и улучшать работу своей организации, делясь полученными знаниями.
                        </p>
                        <p class="culture-content__text">2. Доверительные отношения. Решив наладить более тесное взаимодействие между сотрудниками, организация не добьется успеха, если просто велит им больше работать вместе. Это особенно касается сотрудников, которые привыкли самостоятельно принимать решения или вырабатывать идеи. </p>
                        <p class="culture-content__text">Совместная работа строится на основе доверительных отношений. Они не возникают сами по себе, однако есть несколько способов, которые могут помочь.</p>
                        <ul class="culture-content__list">
                            <li>Площадки для совместной работы. Построению взаимоотношений способствует создание в рабочем пространстве привлекательных площадок, где сотрудники смогут работать вместе. Разве не лучше это делать в удобном и вдохновляющем месте, чем в тесном и унылом конференц-зале?</li>
                            <li>Хорошие инструменты. Для эффективной совместной работы участникам команды необязательно находиться в одном офисе. При нахождении сотрудников в разных местах наличие правильных инструментов может значительно влиять на то, насколько хорошо они могут общаться, строить отношения и становиться надежными партнерами. Например, Confluence обеспечит более удобный доступ к информации всем участникам команды, независимо от их местонахождения.</li>
                            <li>Стратегии совместной работы. Нужна стратегия удаленного взаимодействия, отвечающая потребностям вашей команды. И тут вы можете дать волю своей творческой фантазии. Например, можно создать внутренний блог/чат, чтобы поспособствовать знакомствам и обмену знаниями между сотрудниками из разных мест.</li>
                            <li>Личные встречи. Даже если участники вашей распределенной команды в полной мере используют инструменты для удаленной совместной работы, важно дать им возможность встречаться лично. Например, можно организовать совместную поездку на конференцию или предложить удаленным сотрудникам периодически приходить в офис.</li>
                        </ul>
                        <p class="culture-content__text">3. Тимлид, подающий пример совместной работы. Помимо содействия открытости и построению взаимоотношений, руководителям отведена еще одна важная роль в формировании культуры совместной работы. Для того чтобы совместная работа действительно стала ценностью команды, тимлид должен стать примером для подражания.  Участники их команд обращают внимание, на то, что они говорят о совместной работе.  Но еще больше внимания участники уделяют тому, как ведет себя тимлид в этом вопросе.</p>
                        <!-- тут должно быть аудио -->
                    </div>
                    <div class="time__btns">
                        <light-button 
                            class="time__btns-light"
                            @click="router.push('/block-4')"
                            >вернуться
                        </light-button>
                        <my-button 
                            class="time__btns-dark"
                            @click="router.push('/roles')"
                            >продолжить
                        </my-button>
                    </div>
                </div>
            </div>
        </div>
        <Navbar/>
    </main>
</template>

<script setup>
import Navbar from '@/components/Navbar.vue';
import Breadcrumbs from '@/components/Breadcrumbs.vue';
import { useRouter } from 'vue-router';

const router = useRouter();
</script>

<style lang="scss" scoped>
.culture{
    padding: 14px 0 80px;
    background-color: #fff;

    &__inner{
        display: flex;
        flex-direction: column;
        gap: 30px;
    }

    &__title{
        text-align: center;
        font-weight: 500;
        font-size: 16px;
    }

}

.culture-content{
    display: flex;
    flex-direction: column;
    gap: 8px;

    &__text{
        font-weight: 400;
        font-size: 14px;
    }

    &__title{
        font-weight: 500;
    }

    &__img{
        width: 100%;
    }

    &__list{
        display: flex;
        flex-direction: column;
        gap: 5px;
        padding-left: 40px;

        li{
            font-weight: 400;
            font-size: 14px;
        }
    }
}
</style>