代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dujojxmq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxedyior.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2myzdvkfe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uirgyvbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzuecsyg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2cauisdnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjikpyek.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ktsnradx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yvbmfmkg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xrjnxtld.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ayzyubrw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dpvcdlin.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ndzpcwbr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kkaricbw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2bswzizgm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2khpadhmh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2wiuclsbh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2tpdnguat.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rwgsqxwq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2valqlwgx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2xxtrliat.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hpvnqquj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2cpplhbur.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zjgsrsht.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iijgmpch.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2gbzdaxeh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2smzkimhd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rpdddunh.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hsoyihvw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mkfxowqn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vnvzokwo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gnvwduiw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2roypjcyt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uenpqejh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ojiafego.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfpclzz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtsjsdt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lgfmndrc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rezzrtwb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ddpgsjdo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2sectczyt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2frlkjdcp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2olpmxmuw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2sgjrpqvn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qymvfbal.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lejvaccs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2skmaewgv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2glprhkij.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2smaetgii.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2afmjlyjq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ojvcurwn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2djvvwdgz.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2evaiurhl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2czxqclxo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qgdungaj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wcdsktws.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2oefkfmop.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uqqqcuzk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vhombcat.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kgjaiiyc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uvnaeayf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kmoksasc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2svuktuwg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2imlsacya.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pwquxfbo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uzagdtpf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2mmbllbdp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gqklgykn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2lsxblzom.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fyyqphvb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2gfaytqsx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qvllhywo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2edxcnuuz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vvrrtage.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2wylvppkm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tbteblmg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2emizblqk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2utgdsbbe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sszucjgk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xzbtrliy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tudqqoxy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ppuynaus.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2filpcyqn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hudicogk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkrueldy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2lpwyzdzr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xypmeapc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sumlpbki.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eriuebnl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2rtomfnxd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2oswlqpcm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zkekarrv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbfamayl.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dscynxtf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hcanjdjp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2lpyevzsc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2vlfdoobd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2rwnpxdtp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wblxkdgz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jsygurys.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2urieyema.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fuvqtlng.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bneopfqi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2pbivhzwi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xjfzbqse.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pzqrltdj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ncezymsr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2dlcjhozz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xlbuqqic.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vpafnvic.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vvlrnjif.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vubwprem.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2myxfsvum.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ngvotmnn.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2eoccyxhp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qdztnfqr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tiszlakz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xnkamhqk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2apusxutc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2operakmo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ejzzikiw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ppoderld.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tmymczex.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fccnyumj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2jhhvjojt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zantpnvr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sollhjco.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kqamzxcf.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2otzidwmh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gfdkykqw.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2grgvibvr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2oaidlwiw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hnpkbqxg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2bawqyfcr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qczjyxnn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2arpxvnxn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zteqrizo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kllccyhm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ewlsufgc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ynrmpebr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wlsfzhyb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dnirgzaw.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2toluobxc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2raqnbjhh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2aaxtepjy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2iiqdhxwi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkkbppgm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2fyjmitwh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2aelauxah.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2svbtleds.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ttdfqvfl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2csbslgzf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxjsgbwz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yoqgcdbz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bnauolnu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2etqpjirf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nkbewtsc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gifydzdz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlelcqsv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zqwvbnen.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2alzdaxjd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bmwkhrrf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2bfgjmqrv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vgqaigju.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lnpunszl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2zaqsqnmz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2aokwjmme.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2cuoeypib.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2ufvquctz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2eiajqzkp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2uycmijig.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2gknpntyp.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2upsmcwap.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2awmeqlfr.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2exgbpxlp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2egbfprqa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tvoxzopc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uicizrnq.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2awkhgtiz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ubbmdktr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xnvrfazc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2wcczsxlb.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nhbgnyfk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2xyhxooag.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ksqxwqcu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2qgixryma.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2mfghiayw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2mskdygnr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kojbbkwg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2pnpnolbt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2dfwnxifp.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrbdndy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gffhzfqz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2olsrokhx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqrxzvf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qhhadrpv.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mwzdtqex.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvcirgme.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2uyggfcon.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2ejutfyrs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2owpaeczx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qimbcpzs.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lociwvgd.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2htghbjey.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tmzmbvuh.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qfxqptbl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2inmtidhq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahoyczea.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2esfnkufl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iobourwe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nsexgmjg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2dtlaqybp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bdzkulga.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zbshnapj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2nzimswel.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2fqflfnjt.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvgephx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2llgthnts.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rxckmpbw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2kceirmml.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fdffiyus.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2rcgitdqg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hhqrihpi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ejnmckdu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2bnpurnlw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2jgsoqzzt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgxqdco.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2phyhqsud.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2cuupkcwj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ymvderpn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pjtpmfkx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvnnerfo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vjvdrata.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kqvrhbwq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2raxxzgge.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2oakzwali.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fdramkuv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tldvhpek.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2baiaqokv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bcqlcxeb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ysyrvnwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jascknts.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2mscywcxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swrqjyff.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2ublzfflr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tizdyjyu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bjzxlmeb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tqmerbjd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2axrnzqln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kaugiogw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ffozgjbj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qloyioln.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gdukmfpq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ueibryif.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cyvseatq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2bkmjgdbf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wwhtdaac.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bydvuxej.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vhgbnnmd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2juwvxrsm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dfuvtrwi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vlkgwfgt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ptpzjniz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yoanmcie.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pcxatthr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yqyrdecf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2svskpywy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sgszbqmf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rofjsvoe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2owqfpegv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ntpzrdqv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cjyftfdz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhkgsem.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2deqgedsl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2boqlrqeh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2suindmtf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqiypajh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ygaytdol.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ftgcthot.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2apoxoior.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xwktfaxx.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ghzcsivi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2abptvkdb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kvvixllu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bfncnivs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oewubkyq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nagbrvue.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bifidddd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxdejlxx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2jzcjgruv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xpvahqny.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2expkmztg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gtdvtfqt.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqvjntlw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpkafskt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2kezcqtdu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ecworyur.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2brmbhats.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jqvkzruy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2sojmvsyq.html


<!-- 参考信息 -->