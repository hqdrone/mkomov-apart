<template>
  <div>
    <section class="hero">
      <div class="container">
        <div class="hero__body">
          <div class="hero__title">Приложение для решения текущих вопросов по дому онлайн</div>
          <div class="hero__text">Поможет решить проблемы жителей дома в режиме реального времени, без дополнительных
            визитов и звонков в управляющую организацию
          </div>
          <div class="hero__button button">
            <nuxt-link
              to="/registration"
            >Попробовать бесплатно</nuxt-link>
          </div>
          <div class="hero__stores">
            <div class="hero__store"><a href=""><img src="img/gplay.svg" alt=""/><span>APP STORE</span></a></div>
            <div class="hero__store"><a href=""><img src="img/apple.svg" alt=""/><span>GOOGLE PLAY</span></a></div>
          </div>
        </div>
      </div>
    </section>
    <div class="pluses">
      <div class="container">
        <div class="pluses__grid">
          <div class="pluses__item pluses-item">
            <div class="pluses-item__icon"><img src="img/icon1.svg" alt=""/></div>
            <div class="pluses-item__title">Информационная система</div>
            <div class="pluses-item__text">для улучшения коммуникации между жителями МКД и управляющей организацией
            </div>
          </div>
          <div class="pluses__item pluses-item">
            <div class="pluses-item__icon"><img src="img/icon2.svg" alt=""/></div>
            <div class="pluses-item__title">Обменивайтесь</div>
            <div class="pluses-item__text">с жителями МКД информацией и оперативно решайте вопросы управления МКД</div>
          </div>
          <div class="pluses__item pluses-item">
            <div class="pluses-item__icon"><img src="img/icon3.svg" alt=""/></div>
            <div class="pluses-item__title">Общайтесь</div>
            <div class="pluses-item__text">с управляющей организацией и ТСЖ, участвуйте в управлении своим домом</div>
          </div>
        </div>
      </div>
    </div>
    <section class="use">
      <div class="container">
        <h2 class="use__h2 h2">Кто может пользоваться</h2>
        <div class="use__blocks">
          <div class="use__block use-block">
            <div class="use-block__image"><img src="img/use1.svg" alt=""/></div>
            <div class="use-block__body">
              <h3 class="use-block__h3 h3">Жители многоквартирных домов</h3>
              <div class="use-block__ul">
                <ul>
                  <li>Получение сведений о квартире, доме, лицевом счёте и управляющей организации</li>
                  <li>Отправка обращений или вопроса в управляющую организацию, ТСЖ или ЖСК</li>
                  <li>Передача показаний счётчиков</li>
                  <li>Вызов аварийной службы</li>
                  <li>Запись на приём к руководителю управляющей организации</li>
                  <li>Новости дома и района</li>
                  <li>Публикация объявлений для жителей вашего дома</li>
                  <li>Отправка заявок на устранение проблемы и оценка качества её выполнения</li>
                  <li>Организация совместных мероприятий с управляющей организацией</li>
                </ul>
              </div>
              <div class="use-block__button button"><a href="">Зарегистрировать личный кабинет</a></div>
            </div>
          </div>
          <div class="use__block use-block">
            <div class="use-block__body">
              <h3 class="use-block__h3 h3">Управляющие организации и ТСЖ</h3>
              <div class="use-block__ul">
                <ul>
                  <li>Быстрое и надёжное информирование жителей МКД</li>
                  <li>Работа с обращениями</li>
                  <li>Возможность прикрепления фото- и видеоматериалов</li>
                  <li>Получение заявок на выполнение работ</li>
                  <li>Обратная связь от жителей МКД</li>
                  <li>Контроль потребления коммуналных ресурсов</li>
                  <li>Предложение дополнительных платных услуг УО</li>
                  <li>Размещение новостей и отчётов</li>
                  <li>Автоматическая синхронизация вашего сайта с ГИС ЖКХ</li>
                  <li>Приём оплаты за ЖКУ</li>
                </ul>
              </div>
              <div class="use-block__button button"><a href="">Зарегистрироваться</a></div>
            </div>
            <div class="use-block__image"><img src="img/use2.svg" alt=""/></div>
          </div>
        </div>
      </div>
    </section>
  </div>

</template>

