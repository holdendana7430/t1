代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tybqukcg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ecczgjen.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jitqdgat.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ytwlnlwg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mxvabwig.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2bsyvswpy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nrxssuuv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pkvsvoka.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rfhjxldq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xlfmuxri.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lgazchdh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ihxkceso.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wwhvztik.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ldahcolu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqzwjhpr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2asfnsorp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2jaywgwvt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2aywrxxho.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2apjorobg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2mybyvxjo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lpetsepw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rkgbwgcf.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2sfbtsyqe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ryzpgmtr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mmrouiot.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eycrcqru.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pgeyzkfe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vlequehv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmdloere.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2isyxpwhg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jgfwsxqb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iuzsebqk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ebroqdor.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ozjcgluh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ajacfkkm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hsfubigp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xhndhgkt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bwdbynfx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2csfhkwgi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2fvmrgyal.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ktlxhpmo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2frvkmrto.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2pfsxxnvz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mltkkkij.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2asrbtgvo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2njbcmoyf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rsifkzfv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gowomkea.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2sxctvsfx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2oebmgbyt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gzhxpnsc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ffqykoho.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2snufpkvw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrtipgc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2pmwalgkq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jxrqyurw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rokaaili.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2gwcwrvpk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ctenespk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ixrcvzfa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2akaklbbj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fwuyjkdm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2chxbiveo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yslxzrjt.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uxhuauay.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2uzjpbdnh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2sbiobwiy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ascmsxyl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2erekbjbt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hynukwqz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jlwouczx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ibgmkkaj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tsqhppsd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dbjtacow.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2untiycad.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2owiumobf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2amhsjlyu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2zdqrronu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xnvhlldj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2khyxrafq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bhwdlsub.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ozdeqvmq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qfdixknq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gomlqjrt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gisfwwye.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nwcmmppk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ghkucpfo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2aczqfnfp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2yifattbc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mrieakbp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lfdwqmpl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xcrcudjf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2phvgnxak.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2glozgdwu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gymetweo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2kxgqlkmt.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dqgkdtxn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2algrfogh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qisyenzg.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wdusadnh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yxjzptih.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2futwprfo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fdffeqpo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qapdnijg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mhseclus.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vuxdwzll.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lpgvaooq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cyuesmsq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2axiczdxf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vftklziv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uggslnmv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2twqpggde.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2utrwrikj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ouqdtkrr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pfyiztff.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lnjalokc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2atmtmwpv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2rjlvgtoi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zaivxzaz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2pjlqtdjg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2polxempr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mlqdbqrf.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2lkavrvke.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ueitmbzd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fqihcutf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2levpawkh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2fkaefsql.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2wndjssvt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2olmlpusn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xhzqxedx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2lqwvgoxl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2sqivyvfi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2egyqercv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xwzsmnbm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2szselpzf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tcmopfni.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yygiikld.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tjeygtwo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wrdxgtdq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uttkzete.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2fhirctvc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ztghpodu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bsfwdved.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hxlzirqy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2muqhmhka.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rgeeaigs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jjvwulnn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2bltzcvnd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2rdyaltmr.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2pifarbmh.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2boaizyco.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2asglrbzn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jfcgktsx.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bipejahr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2qtpbpmff.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2xlgbxdoa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ieijolym.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dnshylrh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ptzpcmpx.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ifbuclgl.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2skpgrjmm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ojamjqrq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2peykdtem.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pymheygf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2pbycddvd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2oqinptgw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2shjuagto.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2pqetswic.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mioxsumd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2glwzjppb.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlvhtoa.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjbwrjs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrlytid.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqxhpwy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ztzflazw.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ywqgsbsu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xjmvbokk.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2kkdhuayn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jbumbchz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gjacobtn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wkqzfksf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mjoqibgq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dyvxtbeg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2rnswalhy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2phldzvxh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ygxvyzoj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2grubbsss.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2onypqgqa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pfzpzzez.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wvdoxtgh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vmormwsy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2pwtexnct.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rzfairdp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jtinmmzp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2qsrktyjl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2jfdhgwun.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2xiafbert.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gjrftwcl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hxgydsup.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2vhiurznp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deyzftau.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xphkuvyr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zpxiisxq.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gztqarai.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2buzenjkn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fgibmucu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2egdktisz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ebpjoyal.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2orothcyk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmwtrdq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2urisraeo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrhnjyn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gxvwswmq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fvjvufsq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ybdeydkb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2lbuvvejx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ubbpewmx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kjzzocsj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fakgseed.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fgywwcaj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fqiyoqlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgfnwtne.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2rgdruqsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pliafsov.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qobgogmo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2uuwwsosq.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ecprjqbd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ezjeghbi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ymozyoea.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dyxoutac.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yqvoafrs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2jnsxisps.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ceuvzpyx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2naheewzh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cpqbinvg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvyezdh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hvptunto.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hstezxjt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cccrkfqe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2jqyrvlpo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2gkqkyytv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ewknsuax.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bngjrsvf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ufsibnur.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sojaeuqo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrogadde.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pgogfwjp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2poteuita.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2cmzgykng.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2oozwvorn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sexjmjzj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pdlrdfat.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2uuxejjhc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2lfmewxbe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhrvibws.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kjceepwx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ueicrnwx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2npbrnfkk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2atpaaior.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwlgozro.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2csaxlpmz.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2nibhdeyl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qxnsbboq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rffzvskg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxssigwa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbfpgxdm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fdssyxdn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2qnekcuqe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2afghimtf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2akzeoyhf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jqlkixpg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imddwbzw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtwmumia.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zprszwax.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qpnrychk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mcqczmsi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2lxojbjjm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2koaehqwt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfaidqbp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2indwfanj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivxqvyap.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxxptsgz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bgqpcgan.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2okyqdruy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2cmztcuuu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vkmzshin.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtslmhh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2lxvdqome.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2mqndigwr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nydcqyvh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oqgftpbr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pelbxfdc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zhuxsxmo.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kozubgtw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2prvvzwpb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2drxuecyk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zrhfmxci.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jnlasyiz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeaozrzk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hlnyuypu.html


<!-- 参考信息 -->