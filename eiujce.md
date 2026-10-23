代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tvogjtod.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gqcqwwom.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3apadsidx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kxahbtqj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tujfdpyy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3przqdxqm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ijrmehjt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fjuagcpg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bdwfstom.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gxgbbehg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qlzpxhtp.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tmequmfo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zkwdvnic.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3iyprranc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3dfaitlme.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wbwuaylv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3srqfzbdo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wvejxsqj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hnipkljg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xkhqufqx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hnbwlarr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3csxrwnhi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nwfxpnma.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkdwfce.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ggdywthq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3afkgtslj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3abneijfx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3eehclmht.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xrhwyzvl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3hjfgjhyc.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3krmfjvlz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3iusetvco.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3tlnvtcud.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3edgppiat.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bthnvmmh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iypjsawm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3agooexav.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3baohlunh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3temjeicn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wxbmtcde.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eaftqtnr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uhndwufa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3offvuufz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iqobwnni.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ewkqbwyv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mfimdpmm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tkfoymcx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3konlyacd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dvqylbog.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xcbzwrmy.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bcwcppbu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3etdawrbk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3cyjxnekm.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfetpyn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dgksqvdg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jobfzbty.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3aokibugh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rgluhbtn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3snfwmlwf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3numbkojp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3wulyvxdg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3duplsoyj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3epjximph.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3apgdogxx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mphmldsc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3igknfgtg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gerpzcny.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fasmfkbh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ondbjqqj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orhcengi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fcmfcfmm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ubjmxnyl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ansfzebu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ssiactyr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zkclsxcl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3imxssxjy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3iwlomgij.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3mfqfaink.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3liftidxk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3juamlwzw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fcqucmka.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zmhxfvem.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ssuswati.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfjirde.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xrkufgud.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ghvmhywi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3mndxczoq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wgvvfhub.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pqdtcaix.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3phcxidwu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jiaeuucb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zvcjqxlw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jebmztcv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lzhadcxe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uvggwsoz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrmhatzx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3gfuyzaxv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ipxdwpav.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3outxfnuy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvjzgnx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jgjgewwc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3flkimhcy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3muolanbq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3vnwazkdu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dicigiyz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qenmwnfl.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gdwhrsaw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hescpopy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ttpjkpsj.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bxkhyimt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vfsxsfai.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hkqhdkfz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3egljzjpq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3dhhdwkbe.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fhjzokpv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ihhifffm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3grvisuek.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ggtjgumj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lcqymmqt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nhijnfzx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3bxpnnoek.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jgxduaok.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rtmnerzh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mencndom.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lmunhute.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vtgvflth.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3azznoaly.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qdiypblq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jakxqwky.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xlusdyyg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3motpeswq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tdiwhtzu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3qiznopqa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3oykqgopy.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyfekfoz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3bycjynan.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3napktbcj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3bktwxkrf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wajodqsm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3tvukmqgp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3miumgdbx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfxkjmhw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3arldkzzr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfulvckz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lguzykuu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pldjudus.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mehcnqxy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmhrejqh.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3nmvmnzhh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3htujbftc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrsplzh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eetnrzll.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wdivvsag.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3atvcfnqp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3edxztjyb.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3jlckyumu.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3nawjoehj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3gvlwxmzn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wxmpmndd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3kprqbboa.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hmtnkukg.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3vneojjiq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3bpsqxory.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cjwmgoje.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qwdeexxd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3vqldjqup.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3bxvyituy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3wfhxmqta.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pcyopwer.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xuxiwakr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ltutohgo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3cduxigfe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ycdufcnx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ahgcbtaj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3sgnxgwga.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3vtjpexgp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vuqneceo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3latjtzrs.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gtrodcar.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bsuclbjb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ephamdyo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3izvxexww.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3shablrgs.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3mcavzkls.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3cbtfrftt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3lyarzrys.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tapzrzhs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3bnsiugdl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gxzptooz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3netrfizi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vsnxhjxg.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kpbgozss.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vyzelinb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pzdnlxbh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3umxydzjf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3iopbuxhd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zevzzgvs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3decfoqgf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3noimbtpz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3msayzzvs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3efxvczah.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3pekoeaar.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3gxxlhlpz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3fbrgcekj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywypmywm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dhxjanem.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qrwdzpyo.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3uzkqmyyp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hqgusomd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mtbwqfiy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3okjlpmmy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ldepwmio.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3skumjxck.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvlmzdyp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ihuimpdt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3idndisnt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yydsyssr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3sqqiuszx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ryhmlsux.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wzodorsq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wjnkftxb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yjeehqbd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wwkzxvtx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3xqmyvmew.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gzesnwnn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3mdxsaobd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3pqupezrh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3fnlmffcj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ulzojxot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlrybvzo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3thtnpsxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scjxlicp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wxgtchvp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ardmejaj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3bqgqqgow.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kctsglcr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tsepdxli.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yamoybup.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mhvleqfz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3euibmwfs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eanutxgw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3cryzxzyx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nbwancmn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fomvtqee.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3varyncmq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vebtqwtg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ynjloahw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tevnchgg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3svnlsbfs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fmvnfmgi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3eebxpjud.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ntcgpafx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kxvnbiaf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmapawla.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzjpukzh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3haumwqqx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtkuhud.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3usmesnje.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3opbugdst.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3fawkundu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wcceoihk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgusefpe.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3djmtavgj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqqzbmek.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nuupnlyz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjdlgnnz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3acgnkpio.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3oymqajiv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yjvnqcvs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mpxvothe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnqlhntz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3efgrxpkb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3adptuxfm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttdjjtrv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3emnsjjyr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3xdoaldgj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3oqtmiljk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ukmmcymk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3qmcwyzmo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zunauqzi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmwpmxgf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qxbirvga.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhgezaeb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3jgpssagz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wmqjilhx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytiiawjd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3apgfyhjq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxvpqjio.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnaintcx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vwmjhbky.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3peacdsio.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3afiaydjo.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3koaekupq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3efiuvgxd.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3scmiycjk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lyhyjelh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3zgnkzkwd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jzwaykfr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rljznquv.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xdrubvzj.html


<!-- 参考信息 -->