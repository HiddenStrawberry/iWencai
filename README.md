

**iwencai一键诊股工具**
====================


----------

- 封装了iwencai的部分接口，提取出有价值的信息，从而为股票买卖提供参考。
- 提供【根据条件选股】函数，并可以将结果集输出为CSV格式以供使用
- 自动遍历所有买入/卖出信号3年内**指定时长内**的平均盈亏比/盈利率/成功率并计算出平均值，提供强而有力的历史数据分析。
- 封装GET,POST并全局加载代理，，支持IP池，可接入第三方代理获取接口获取IP从而实现IP封锁后的自动更换
- 提供了一个腾讯云自动更换弹性IP的小工具
- 暂时设计了一个简易的前端，输入一个list即可输出全部结果


----------

- 为避免不必要的麻烦，本工具还在测试阶段暂不开源，仅作展示，如有特殊需要请联系作者



  
----------

    return {'score': score,
                    'bull': bull,
                    'short': short,
                    'mid': mid,
                    'long': long,
                    'title': title,
                    'content': content,
                    'sell_result': sell_result,
                    'sell_num': len(sell_result),
                    'buy_result': buy_result,
                    'buy_num': len(buy_result),
                    'syl': syl,
                    'zycp': zycp,
                    'hy': hy,
                    'gn': gn,
                    'buy_cent_avg': str(buy_cent_avg * 100)[:4],
                    'buy_ratio_avg': str(buy_ratio_avg)[:4],
                    'buy_rate_avg': str(buy_rate_avg * 100)[:4]
                    }


![Based on Flask][1]

  [1]: http://chuantu.biz/t5/164/1502173210x1709684826.png

