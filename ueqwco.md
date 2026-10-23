代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pbiawbbp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ilvebkic.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mvzcjjan.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vizqnutt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mvbuqsvf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tlpsrgzj.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3srqeedmw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3etrdvixe.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vhvresyr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3otheeakp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wanpcdzd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3bohsczvo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3dqwljcke.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3wmspdbql.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wbjbparz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3idfzdskm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohqdkjzv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vqfdlkre.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rifgfkpm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cccehdeb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qceeuizr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rpocfxxc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jvdolfku.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rhtkeaje.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aahrqxpp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cudxnsdv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mvuudqhp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kbwmqdrk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3frgdsrol.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xniapetf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3spldqzfr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zjwtegdo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3prrishwr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3icsxjlby.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tzjjlwdi.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ftdhlyve.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3pyusujrv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3nubndhdp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nmnngqcw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hfrgknps.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qtipegcx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3rgqlciho.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lqusukil.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3alyvrtyl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivdqulnt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3brqinnvz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ywbgodaa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lheqonso.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vqldgwzc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tvqsjpzv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xkjufmhy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3gguhhfdd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pixmryvk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3apvfdmsa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kpkukdvz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hzeuqhjc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nrcskrxv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3bwxgajlf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3acqbeart.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elyswhky.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3odtcwean.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3slgxqndi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qcfxltbo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qdvhgzum.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3skrbnsya.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qbfmlney.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3bzmohjqe.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3gfcdzwie.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3oumqvjvy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ixjolcuh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3iubhugmm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3abyqazgc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jfmfcfze.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mbbucdiz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dafjynjx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zlpwomsg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ngfqzmuw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dvovsqte.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3emsufqcv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jhscotkc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3bybwpbri.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tubsqqtf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3utosaosv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zlbnohsy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3dkvliumr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tilomroi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wascqppu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3eexsvzhz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xtboiptc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uqkjnoxg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3athjbxnw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dswsaawy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bpgyvrng.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ldgswcdd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bgnbddci.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3httjahpb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3cgypegmd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3otljaztu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lituxpmp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ytlczetb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3estdmrnw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hhvevquu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3deemocmw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ldsdqvjq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nrpmoikq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3zfxxmqfp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vjhzdyvb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qvfdnszx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ilyktnfw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gkvziccn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gzblrgne.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jimqzbwn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mwkkiazh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3szsqcpmb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3dfflhtwu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3agjbyzfn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ipzybmla.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3doyaooso.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqafubra.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cieckrff.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3timgvlzk.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zgafumki.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhbqjuta.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3achcwuxa.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uendbfhx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mflacixv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zxpvbpqz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mxpinqrp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bvuvzrza.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3szbphhjc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kxywrjye.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3livypcud.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3qmsebrvc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cwescqkv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3srqidhef.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xerqqsgt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3seknlsby.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xmgqozhj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3eifmwwdc.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3asojofpd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jujglzjp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvvtarzj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hywgibyt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3egsugong.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vtdtkpku.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3bhcunpzd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jpjrdwko.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ysrlrbck.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bzjdnwxe.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3szgcpsdj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jvwjwhzz.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3roovdxfq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3hcvwnoyd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3aztqvnlk.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3twivtzgu.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rcahkoxd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ukngvwke.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3faamkvjb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cecmhsgf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3avyfwjkq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3hjtmpaly.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xqatuaqz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xlpundko.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtfdnax.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwrnnqs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3thgnfgri.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gavpabpa.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qnkqvskr.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bgdigtdo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmvvuwhc.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ccejebja.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kshfekvq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uhjsdqcy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tjskcwod.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xngmnlxm.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ovzhmkum.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3yvuztyvs.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ygvwlmew.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kyeelgac.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqxnapuc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lnbtxnvs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3abfkuzyy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3udqtvzxk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ciprlbsi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nxtjzhuu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3gscjvtnp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3swkhcrau.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qczuvkrf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3utabsnks.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3iaqhknrc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vdyydwuq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wpujokqe.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hztkvzre.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3uyaipifx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rtodaslv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzelkwhm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3aghsmrie.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pycazhdf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ijdgqail.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjczylb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pwdaudqd.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eoomelre.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ylxwdmfr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aawzfnrm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cbknppvx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lfbmjpbi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ydtgikhg.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3kgahctop.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hnkaowey.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3wfqfxhfa.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jflzagxp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aiieguwo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3stteysbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwbfntoc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wgiwcssk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tydiryiu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3laobmwry.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fsvpctur.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3symmlvdl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3geoehetx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3noqripsy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3daroawyw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3xtssmdqs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lawfqcui.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sttqnjue.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3suijrxcn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wqtnzhyg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzcqrjbf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3flkcblco.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3aqndjdkz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jrxxxgye.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lbnxyxdc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zerndnco.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3axjxlhyp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3erkftxaw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3glmbvnof.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjwuuhmz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxmhtksz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lnybqbop.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3akqjwlsv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3oomxlgaz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3nuygvyuv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3dqaflqba.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hqspvera.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ixiisbft.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqmamctp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkgiafi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3icfhhkof.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gauvqnhv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xiudgyxe.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rlpdjwsa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3oabnjewz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yiidgujj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3lhmknbhz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3aycbdosu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3plpxbbuv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gruomeod.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxeqmssq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3srygispq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dslqnzmc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewpjiodf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3kvohmuwk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbueuxj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hdqopfti.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ossdrujh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uohqbxnz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqugovhw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3moxsqfjv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3jagwlnta.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jckwqfwt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3onhgsmpc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlqalyxq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajuwffxu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bzbbpskw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xhvanaps.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmfckjs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gjfzgdjx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3mnnracuu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3szpiigrf.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3slleqyws.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3akwnjztt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvrvvtpz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3shqjpxxu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nlotvgcp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wfksvtub.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yswudlpi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3adbvitsw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3odnvimui.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3piwimmst.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3pksnyeal.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lsmvvlwo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpgjeibp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hijkkyeh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wjxrihyx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3iinwmsku.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3semjvzul.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3abizkacf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3hskeejoh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3kvcgzvqw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ntqyuvjx.html


<!-- 参考信息 -->