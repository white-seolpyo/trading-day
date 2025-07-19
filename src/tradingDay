from datetime import datetime

import yfinance as yf


def get_trading_day():
    ticker = yf.Ticker('^KS11')

    df = ticker.history(start='1990-01-01', end=None, interval="1d")

    indexs: list[datetime] = df.index
    item_list = [i.date() for i in indexs]

    return item_list


if __name__ == '__main__':
    date_list = get_trading_day()
    print(f'{date_list[0]=}')
    print(f'{date_list[-1]=}')
    print(f'{len(date_list)=:,}')

