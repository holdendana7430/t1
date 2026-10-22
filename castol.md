代发 wailian999

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2pubhifla.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ngqrhvmx.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rhedvjao.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2czrbdqmo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2editjqdy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wghudzqb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sqtgmdls.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2kfqaxble.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2uazrjfff.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rllrgipo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2oudiacnn.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jwdtnzvw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jzaqmfcy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mvjlcini.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2urgkuezw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2imfkuwei.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jiylwigc.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zodjkocb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwmxsbgk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hpkgbpug.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zrqvnsgc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2givnksyp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2kvikztam.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hbezolid.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xgnndtce.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pzhtshsz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kiczfqor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xlyulvkj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jjncmkdt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2yctmwhzl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xejaawap.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ctmoeuhx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2rskwhfcv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ndwhhajb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkowdgc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2owcgmiub.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2mrfpuwfo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ftuxrghl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2yqeexaki.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ioaizjww.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2skdvhpdx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vintdkvd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2etnkcghn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2puxxkeyl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vmyrxkwy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2fkvxqekt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ijxnijgd.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lbzqebvy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xgsgagah.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ayvwrmbd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbkmwudl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkgvnzjx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkobfkam.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2onscgwcs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ruxrrlop.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xczolosb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wuyyvqvl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xygufmoz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2pqhqeapr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pvrzaqfz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uhptjpjp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pfujpryd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rmkqhwbj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zgqtvyyz.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2flbnetuw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kgmyvsdo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ewulcuba.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hzgyhykj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kveizkrp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2udsrdynu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vdnzblbu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2scrfprxb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ipovxkog.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uolsndjt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mkoleczi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ecrzdrnm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2srioabbi.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xevavucy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vqablfdh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ftbrgrhh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2rqjejiqn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qruhobxf.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2wzkimmfc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2bskguobu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lxhrfukm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gsesydib.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgryjykj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lgwkucrh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jmgugqfx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nyexcapg.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2elgomldm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2relmeijg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2dqdgitvq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pirgcbxj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lksmmxkr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gcjqoqdb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yenwzqap.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2jvfmswll.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lueiyvlx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uniqtrhv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dmrdzwtv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2zwtscnbq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2oemwfwep.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zzicibda.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ggykdcof.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mdouwccb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2msbeodsg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2exhxkyso.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mjhvmrqj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qqskious.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ujizpmme.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2djdwfujs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jntasvvx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2enzzebot.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdzqioaa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpsyqxut.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2epzbvagx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2cchlggbe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ugfdgdcu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2optnzzgt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvupkhei.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zbioinuo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kqqkbbwh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhpvpjbv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2klyflznq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmphglgv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2izqdzklo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2utpzkeka.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2orpyjmdz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dnpuicxp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2djlawaif.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yfmcylqu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jjocvnsn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fukvpbgf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hqacfgfz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2zkjmayhd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2vflnortu.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2kiplqeme.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ycjqgped.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2bypuggyc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cqvsmksg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2dyzqxkqd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2fzmbrfup.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2yjelqkai.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dltiddct.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rcexkvpe.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2nojhbfvm.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ndxmljlw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jvqukjje.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2exovdhoc.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ppzrdvee.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rksbxnhq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyjnwht.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2tswujifk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mncqlskk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2xveopprr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2nyuqqfcm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mlpghhpb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gtwrfscu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xjgcxjne.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2skcsjeaz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2sqpgwkqa.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2stpyughi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gyvgrpge.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dloexypo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2oaufhtqg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ewmyxzep.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lzqqxczs.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dtpagfmp.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zfazdkyp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2jxkqoyfi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ikbqvynf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hsexymfj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xmdvcfee.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vmcjnxdl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tofryoxh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2alsbfaol.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gfacqxgg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vcnbnpqm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2psxulujn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kvhdhcqd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2keycwsbf.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2uldeytgd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ybgqxkkw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pilotwbp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ontrlktl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2rrtkeuac.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mjmjrfpr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iljwcack.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2whliafbr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ybfpuhea.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ltgomolp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ehrauwfw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2uoibevwb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qrgptsgr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcsdwvp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2eploaoxk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mtbqhfiq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2qwimhnry.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqnvhsoj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2beryjhhz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2lqkfteff.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wbuuuxra.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hehcydln.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2povlxliy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2omdexgsi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwmoxv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2uoaaqexr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wvalmlqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dehmsmen.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mmsfljsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxtgaaoj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jclxbyve.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lpivfvyi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyumqvyw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ttkygpeq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jfiicffk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gazbghte.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qqcfpysx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2yekxlygf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2napdpqnd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2delzmcrj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2wvbasxdd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ufcypvgm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2udmcqgvs.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jbdqeash.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lwtmxelk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jhtydqbv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2iqrxxsik.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qhpkckev.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2yhqyrkty.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2opwzvhmu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpujdsqt.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmyulzmu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dehyfibq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtcesgrt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vavnhclj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2gkmetvvw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ytpzvcfb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ghpegbou.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2lbpbuxve.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxgnlkio.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2weedpqob.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xltojbvi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ueaebyqf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2aodxtynk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2djekeami.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2siukmfxu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jhednkof.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2kglunyhh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2tytinpjg.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahysvsgz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zsmwasdc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2oifmqizq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2lptgwxno.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bykhxftu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dxwowntp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ibkzjepw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jqgrmkye.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njyaeawf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2albzmwyp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2slbwpqej.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdylthbn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tvvjtrip.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gpwmpfaa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xckfrblc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lkluqxdj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2librypej.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikgaejxi.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uwlmqqcl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujapekzh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzylhcvd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2gfogwxez.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2vxdwerrx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqarxyrk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fgilnkln.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2akoqxtwo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ymxqeewv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2duoicfbl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rflvxbqz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zqtweqab.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2furqbmal.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2kqetrkiu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oteszfdm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2fzndoryq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2paubplwj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2shagjixv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ipxztczo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xeomskex.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2etnpzjom.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lavnxzzn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cabomgtm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iesqrmvs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gggeyadb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jvgokzxm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucvqbxbu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xqkonppc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vqrphtay.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2jovelsya.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sdxcmleg.html


<!-- 参考信息 -->