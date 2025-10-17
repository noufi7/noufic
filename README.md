import React from 'react';
import styled from 'styled-components';

const Card = () => {
  return (
    <StyledWrapper>
      <div className="card">
        <div className="top-section">
          <div className="border" />
          <div className="icons">
            <div className="logo">
              <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 94 94" className="svg">
                <path fill="white" d="M38.0481 4.82927C38.0481 2.16214 40.018 0 42.4481 0H51.2391C53.6692 0 55.6391 2.16214 55.6391 4.82927V40.1401C55.6391 48.8912 53.2343 55.6657 48.4248 60.4636C43.6153 65.2277 36.7304 67.6098 27.7701 67.6098C18.8099 67.6098 11.925 65.2953 7.11548 60.6663C2.37183 56.0036 0 49.2967 0 40.5456V4.82927C0 2.16213 1.96995 0 4.4 0H13.2405C15.6705 0 17.6405 2.16214 17.6405 4.82927V39.1265C17.6405 43.7892 18.4805 47.2018 20.1605 49.3642C21.8735 51.5267 24.4759 52.6079 27.9678 52.6079C31.4596 52.6079 34.0127 51.5436 35.6268 49.4149C37.241 47.2863 38.0481 43.8399 38.0481 39.0758V4.82927Z" />
                <path fill="white" d="M86.9 61.8682C86.9 64.5353 84.9301 66.6975 82.5 66.6975H73.6595C71.2295 66.6975 69.2595 64.5353 69.2595 61.8682V4.82927C69.2595 2.16214 71.2295 0 73.6595 0H82.5C84.9301 0 86.9 2.16214 86.9 4.82927V61.8682Z" />
                <path fill="white" d="M0 83.2195C0 80.5524 1.96995 78.3902 4.4 78.3902H83.6C86.0301 78.3902 88 80.5524 88 83.2195V89.1707C88 91.8379 86.0301 94 83.6 94H4.4C1.96995 94 0 91.8379 0 89.1707V83.2195Z" />
              </svg>
            </div>
            <div className="social-media">
              {/* Instagram */}
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30" className="svg">
                <path d="M10 3C6.14 3 3 6.14 3 10v10c0 3.86 3.14 7 7 7h10c3.86 0 7-3.14 7-7V10c0-3.86-3.14-7-7-7H10zM22 7a1 1 0 110 2 1 1 0 010-2zm-7 2a6 6 0 100 12 6 6 0 000-12z" />
              </svg>
              {/* Twitter */}
              <svg className="svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
                <path d="M459.37 151.716a202.1 202.1 0 01-60.426 16.243 104.934 104.934 0 0046.132-57.827 207.91 207.91 0 01-66.599 25.34 104.934 104.934 0 00-76.67-33.137c-58.152 0-104.934 47.106-104.934 104.934a108.32 108.32 0 002.599 24.04C133.8 222.878 73.27 190.294 30.642 133.933a104.934 104.934 0 00-14.294 52.954c0 36.386 18.517 68.548 46.781 87.391a108.22 108.22 0 01-47.431-13.319v1.299c0 51.005 36.062 93.238 84.143 102.985a104.934 104.934 0 01-27.614 3.573 108.22 108.22 0 01-19.818-1.624c34.12 55.716 95.163 89.843 161.137 89.843 129.755 0 200.41-107.448 200.41-200.41 0-3.548-.081-7.097-.325-10.645z" />
              </svg>
              {/* Discord */}
              <svg className="svg" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512">
                <path d="M524.531,69.836a1.5,1.5,0,0,0-.764-.7A485.065,485.065,0,0,0,404.081,32.03a1.816,1.816,0,0,0-1.923.91,337.461,337.461,0,0,0-14.9,30.6,447.848,447.848,0,0,0-134.426,0,309.541,309.541,0,0,0-15.135-30.6,1.89,1.89,0,0,0-1.924-.91A483.689,483.689,0,0,0,116.085,69.137a1.712,1.712,0,0,0-.788.676C39.068,183.651,18.186,294.69,28.43,404.354a2.016,2.016,0,0,0,.765,1.375A487.666,487.666,0,0,0,176.02,479.918a1.9,1.9,0,0,0,2.063-.676A348.2,348.2,0,0,0,208.12,430.4a1.86,1.86,0,0,0-1.019-2.588,321.173,321.173,0,0,1-45.868-21.853,1.885,1.885,0,0,1-.185-3.126c3.082-2.309,6.166-4.711,9.109-7.137a1.819,1.819,0,0,1,1.9-.256c96.229,43.917,200.41,43.917,295.5,0a1.812,1.812,0,0,1,1.924.233c2.944,2.426,6.027,4.851,9.132,7.16a1.884,1.884,0,0,1-.162,3.126,301.407,301.407,0,0,1-45.89,21.83,1.875,1.875,0,0,0-1,2.611,391.055,391.055,0,0,0,30.014,48.815,1.864,1.864,0,0,0,2.063.7A486.048,486.048,0,0,0,610.7,405.729a1.882,1.882,0,0,0,.765-1.352C623.729,277.594,590.933,167.465,524.531,69.836Z" />
              </svg>
            </div>
          </div>
        </div>
        <div className="bottom-section">
          <span className="title">UNIVERSE OF UI</span>
          <div className="row">
            <div className="item">
              <span className="big-text">2626</span>
              <span className="regular-text">UI elements</span>
            </div>
            <div className="item">
              <span className="big-text">100%</span>
              <span className="regular-text">Free for use</span>
            </div>
            <div className="item">
              <span className="big-text">38,631</span>
              <span className="regular-text">Contributors</span>
            </div>
          </div>
        </div>
      </div>
    </StyledWrapper>
  );
};

const StyledWrapper = styled.div`
  .card {
    width: 230px;
    border-radius: 20px;
    background: #1b233d;
    padding: 5px;
    overflow: hidden;
    box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 20px 0px;
    transition: transform 0.5s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  }
  .card:hover {
    transform: scale(1.05);
  }
  .top-section {
    height: 150px;
    border-radius: 15px;
    display: flex;
    flex-direction: column;
    background: linear-gradient(45deg, rgb(4, 159, 187) 0%, rgb(80, 246, 255) 100%);
    position: relative;
  }
  .border {
    border-bottom-right-radius: 10px;
    height: 30px;
    width: 130px;
    background: #1b233d;
    position: relative;
    transform: skew(-40deg);
    box-shadow: -10px -10px 0 0 #1b233d;
  }
  .bottom-section {
    margin-top: 15px;
    padding: 10px 5px;
  }
  .title {
    display: block;
    font-size: 17px;
    font-weight: bolder;
    color: white;
    text-align: center;
    letter-spacing: 2px;
  }
  .row {
    display: flex;
    justify-content: space-between;
    margin-top: 20px;
  }
  .item {
    flex: 30%;
    text-align: center;
    color: rgba(170, 222, 243, 0.721);
  }
  .big-text {
    font-size: 12px;
    display: block;
  }
  .regular-text {
    font-size: 9px;
  }
`;

export default Card;
