代发 wailian999

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3sybvpbxa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dqjprlof.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oyirgyzt.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3oxvdjbgz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gwpiwszm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tmfnmhet.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3oeevxbzc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yqjgaonw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ipsszzor.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yadeurfj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3nohapgzf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lhqhnqyj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vnnqnnet.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nfasaikk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwtteivq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3xdaxocjq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kwquubeg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pkrafvry.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3cflfbsie.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dmewidml.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtvafhm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qdpyhahu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lyjyequy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jdqefitn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3byimnhyu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlcctrt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3rvhudnyh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mtebcuab.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3gjkxcmzq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3faajusln.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aoenzwaj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zmevgkzj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bulhiupb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlfrsqnz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dyqlvyzj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bfmzerzn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wcilrqet.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rlqwxbeq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3zfxqvgdi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3umbnqtjn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3twfnljyo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tgfebtak.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3thdkkjfd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3yleusssz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aluywqfo.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3gcsaktja.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fypkqdbe.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kbupvydb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ytzhxudy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xczrnxsd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3boqqrjxr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3htnyvnji.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3tyexwxqu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3pkrzolax.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hwhmizbb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bntfakdt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3poaxmcql.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pdhbjmtv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dmlpwchs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yxqpbagk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3huklpvfv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3iakhletr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vozhzajy.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lrmvuopy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3knjvlqxz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3esdahhbn.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqcmzuov.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lhwgxqcg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rushsdoa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3saphgdnm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qqyarhmp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oekvfrol.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cvepbeae.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuguidc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3sphxqhkb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pulnknhv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3osvhzlzq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3njppagqx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3lvqzobze.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3cjvpmmxw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3kxdzplzx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nqfgymuq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hegqmpxd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mogyljww.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uoeuelnq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tmuofapn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sjfhtsia.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3mmznjsli.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zmvughen.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dxtsiifc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3biecoyfn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3gvablurl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vtxxawph.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ppqrhwgh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3cbmfmrpl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rsiaffma.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3akfhdtkl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3guyrtcvs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3oqznnprg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3iuguzdks.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3upnulqgv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hsncrzfl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3btyzhlni.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ccvxzwyz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ihtrokof.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ryjffkgt.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ebkcawzd.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mgnjzzpf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gpaeijhg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3huttawaq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kbgzuuxu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3njxvlqzb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qllajpro.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3lmpmsxnm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dhbdsyyn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ytqnnxwh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ltmlomkt.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rhygjync.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bvvevijc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ovsflgop.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xnulvxlj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dgwbivai.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vmfiujwu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3uneovsda.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rukewcoc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yhrcdxkw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3gjucvvmd.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zvfdiiwt.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tnihhxgq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3regqpvak.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbynkgsv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3focfziyx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3oxghywwq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mebhyxez.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xadypdhn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3srjkhfgp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ftjpmknv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3khayiuwu.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wufoawig.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qmirleoi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vjjywbuf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3afjfedla.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xixvkdso.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtwnonuu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3dehsxzic.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3utzqwswe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hrajubeh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rykjyaid.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmvvrzs.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3zeictiwn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3lrgbwwoz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3egsygtva.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3emifezai.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dkcfrhup.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rutpqqjc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lqcrgrke.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wfrqpnci.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xigkfkzi.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ilqprwwr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bgaazphz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yetahagg.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jmjpyhye.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3wsjkynac.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3rmzaylca.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mygqraie.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zccusrvk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rwbajnfv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3vtcygqmq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmxopii.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3bdswcvan.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uyuesfls.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ehawkoym.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohjckalx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dcoxfftc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jgtovtrr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ppcinhtw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3orspokut.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ioulxvrj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3isvftaxh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lxpmjpzn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bvohcgbj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndsyhkat.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3lhhupiqw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3qvejjjun.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jzsmkgtw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ksewfqeg.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqnlxuv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3itwklcny.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hfwhdtrl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rxvankri.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3lregsryd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3osiaylgn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ctepflaj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3nwfqymxu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wwdyuwok.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3uckmiazd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qgmvqzhb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3dighglem.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3dzfsvutk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3bhrlytkg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3skduwoqe.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rjvdhdvw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3deqnbtww.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3zkontegf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3kpevpchz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3knskjdsd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cbgcfxmt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ozvbejxg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jqcvxkba.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rjeobqoo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cjjclsqh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pofdcewf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xiitenst.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3npmjjdmf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jrjwwwxx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3oxejpnbu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3zfjjdcva.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3zpdbzpjc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3hvpfljqz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dkbwecne.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zagfjqkp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yvrxmcye.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xaadycwa.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3baubsmbp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tohecvdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jonndcos.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3emcjmebc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eolzgnmg.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3xltebgec.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fywdwgyc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddduqcsi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ufjvykby.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hwcmlizv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3unyhpbns.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3mxsolmqt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ltlphjrp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3amzgbsza.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ihmbvvve.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwdtbjp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3extwxbbb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vqhnofrm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jofnffic.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdcgmusa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3zeowciaw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3gdrujsyn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3skelpidi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3npwuwqiq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3icdkgizn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zagnooez.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmpxlzbb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dywhhbav.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lgaljbzv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3vkuzfhqx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yrwwhhoz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3vmmorgjf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3luurbxzb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqnxtvt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybbntlyu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzfsfvmf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3twofxsvm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3aarwydyw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3butumjal.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tynxjimw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3dtxokpgd.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tucjvqjv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rbfluwkb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3nzulhgkf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zstruvda.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3isdjkzqj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3geiaosaz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3lbtndwfe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kdkwcxpr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxztryks.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nqcgqnzc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3rghhrent.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpejvxhn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3krahvtta.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jnbccgjr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwdzkur.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zhatfvys.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3dncsntai.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ajxcpsug.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3blsgvrbg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xykycrxk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sngmfimj.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvjomyno.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uhfcdwbd.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ptvgrnve.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3shuyoste.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3obkgnmcw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbjzgdac.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3ixhugfby.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qxclzfnj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bfhunict.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nycjzezt.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rjafszwh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3heobohap.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujjschwb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3frsqmnbc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xascvjjy.html


<!-- 参考信息 -->