代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nnhhftxv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3puxcuykm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tgetlmmg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jfqekqpa.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wsydpjhw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hnbipmeh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cimlmtso.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3oxoucxmg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vrmmrskc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mukjekbl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3zwqnstyr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqcsbcu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hsaczubg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rjqfnhnw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wuggztne.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wuqkusho.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dmkrsqrz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3huvqbknm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jmcqdeod.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ypcapope.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3blthaoql.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3blzxtkvp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wxzsnady.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pypqvvkv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zejvhxwi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fmwpdvgh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gibdqjcz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fgtwioqd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pmhgrhwx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wuemwdkc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dydgryhy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rfhgupct.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ubtyzqdb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yafbttbc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3pppjzxzr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3upamfbmy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sazdokgr.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3mrvmppij.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rminhfdk.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zexfrwsk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3gromeffo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nzaqpifq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mveizgby.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dcteacgy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3bzliqchl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ehezgdyy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nkghhlfk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sokxovvh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjsyndlp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gtjbtfta.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3wufdkxgb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bzhkzktb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jlmtoehp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3czmxpins.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wxwwugbb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jsiyptxo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zmcafuuj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzhsbqzy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkjpklpl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhqlbcg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qlkentfl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3dglvvdrz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rxvwjiba.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qasnbntt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hdhgzmtg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3uipexfik.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3pijkznfs.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bhgqwsuv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ovtdbkyh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yxofxuwg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3mweebosz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcslhhy.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vewjviot.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3eunrpqty.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3kawdsvjg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3liqxqwyp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bjcoxilj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mummgohf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3evgpjxzv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dnnuuyla.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jdrwlgxi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ekdpqawv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rsdcyxdz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ennobzgi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3szbhcmov.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3difunvrc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3iiwbmxxz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vuimcfyc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xelyzefs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3frtvvfol.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hbnduerw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mryaijvm.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oorurwrd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mxkjhpds.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jldkskiq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pcbjnhgl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ejtzxarg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ldlqcomx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3etnvoacq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qdatgilr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kevvcgxa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gfithmac.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bmrprpyn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ixxrmtkw.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zcviblvr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xhpxnokn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wsihulhe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3uwqmlrox.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nhazzhfa.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3alphnvmw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mtylluis.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ztwufymv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yvktlgmh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dreddfkv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3arkhksao.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3fwsnejkf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hqqdxcec.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ahcuzpio.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3xycfzbgl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3qhddxrwl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3phdbcoij.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3bxtugabj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3iakuesiy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtlchdmk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3esxqtnqo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3anxbacgk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adizfwtx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3psppdslb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwylewix.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ivxxliif.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfubcyub.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3camaftgl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vccuyhsc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhrdpetb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rdcdcpjw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3iydosznj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3umkbjlhv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3crtnnbee.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3axfzjwdl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ckqmswkk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mgjjvvmm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3slkqtrdk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3cargenmv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xmougvao.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3sdqwnqrd.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3mymzwqxs.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wopmznyd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kcexyhld.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wiqakqsn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3lfmlcnqo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3afnrsotw.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oioxzseh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3fndkvqcd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3twhpuhde.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3bgsubcwo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3onnoxpvr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mfgxkyqc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xullrjvg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cofcvpoi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3sdrnwpga.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ykexobfj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yiacjggz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3zqeanhtb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3wrncfmul.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3zcmbuyhv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3edracnir.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3dyuirssk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3loalnyrq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pqqzplaf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hzzxxdra.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hwbqudop.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3davevsxh.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqjsmzrc.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3irlarhas.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qryeuvey.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3lleucatn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wvpcwwox.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3qbapcbbx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3maiqpcrk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jmevmizf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3eoqbeetg.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zasgmzer.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bghidnak.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pmbdpslv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hstonypw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ptldlmep.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wabzadsw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcvyuth.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vjtcfhbc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3akggvtgj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jbrlbkpw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3eierteyg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tbleldud.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jfurouvl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jggyudje.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ibuusrmo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kxudiuaj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bzecoxoj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3opnihrgm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3idkfknqp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zvpshnoe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3awvrnhqx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yezwuojy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bpglikdp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3qrzwkkwl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3puzjtcbb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vhwuqvxf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmnlvetw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3issskyfy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wwiitmjt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rxpkjzsw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3adykdorc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zftxtdmy.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qdiygebd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3axlcdzgg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3stomlxfs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfspjbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujgagiby.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3hclvejbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arjkqspf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3trqdphje.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3bklovwmr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ptydtgqe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3quvqinow.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ntfysxvx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hjaumfib.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3gvexwdto.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fmvioqqs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dguldqux.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uhudjthb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yjqchoql.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3plqlgysa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jjgvverr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jjislptm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zfjvjzjj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fydgzkfc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ilygcnhb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bjrvxhel.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ufdkmytg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ydbxilwv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qjkvyxgi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwtyvdhw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3khsmagpq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rjuelqkg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hachiisb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gsivgwte.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ggfntggt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rtzdfyyy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kqjgqlle.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wzbtavvt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgnlewns.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lwufhjxk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvqrpomg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fqgyrtll.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cjddlola.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3spvcmjfo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uhtsokow.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wegqycqm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibhctiqd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3msnbbzlv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3chzglrbk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3syvdnnod.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mremxoor.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zkwggnjy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhnrbck.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pkhjfanu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xstfauio.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvipemd.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uvginlkn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlrpfiwy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mofsuajh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3pbfwujje.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cdeloklo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ikrumuyx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xbkwbsoj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgzubmar.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3blqxwmco.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cybvxxlk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeajcavj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lqqmssgr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3uxfczysl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qxgkhlwx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmaztuup.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3yhrfyrkl.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3oapgbewk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qtadpkfa.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvunspgh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mafunbwl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jafkyqde.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iqehzxnc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3kgzweqvc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bafkdxki.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3dbfrnyxl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kopdbfdz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3kszxwaaz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwxdupak.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvxqhnav.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lcoianlh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgldnopa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ejnnwguu.html


<!-- 参考信息 -->