# 蓝桥杯

## 1.学期计算

### 问题描述：已知今天是星期六，请问 20 ^{22} 天后是星期几？注意用数字 1 到 7 表示星期一到星期日（看到题第一感觉就是暴力！！！ 但是转念一想Java不是有BigInteger，太好了，看代码）

```
public class Main {

	public static void main(String[] args) {
		BigInteger bigInteger = BigInteger.valueOf(20).pow(22).mod(BigInteger.valueOf(7));
		int result = (6 + bigInteger.intValue()) % 7;
		System.out.println(result == 0 ? 7 : result);
	}

}
```




