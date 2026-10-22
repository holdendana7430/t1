代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byxzhcub.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2pavwfqgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqmcfual.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jtrewoxi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ajyfymcn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qbxqbbul.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wffrrlrt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2goanhgnf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uxjbwelx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jdfykjny.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fdkgwkqo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2obldfgqb.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2yijzrkdm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2nzekybax.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jxgzsfnk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nvdesyae.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iftqfguo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wsthnhtp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2rusygwkd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hswifzor.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ficrehuy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2fgefbtwk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wepbqhzf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uskynilo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oybvbtmg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vqjpdawo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lsgtcntg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2auegcepc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sdjivtrq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hoavwmeb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yyonakfv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2otuiutgi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnrzvyot.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fnafrsau.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ythfvopm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2wcqfinin.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cypmwhva.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2zqlvmeju.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2qadobhvh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dphuyofo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlslaiou.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kiqbqnxt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xjlizskm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2omynwwjt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ozuhylfx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fxubhuoc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wlweyczg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmnqyxmp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ijotwwdd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2abtjgrma.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hsqslxik.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eufkoixh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ugwronuy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2alkdozho.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bsifcjrb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2akdwxvcu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zzasbujk.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2glzeglox.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2uznhgpwk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2gjbhgnfo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2oqkolsbi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qcmnzglp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mzreyanq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2oizzevlj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2cxzdgbyr.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2fyxemxfy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2puhldaag.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nvizjncr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qgsazaof.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bwmaonul.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcxjmsv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aykpizna.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2xyxjvfxt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qrlrmavj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lkahtnbb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2faefxjjr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2byibimgv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vauhechs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmqbxate.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tppfyqve.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jpuwlpnv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fygdztxo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wirlhgga.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmhslgp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vdflamtw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2pwyddoos.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mytoccft.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2efvprvzx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vwerpgcb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lwiwssms.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rlfjsmaw.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zscyrntf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ipcwuzls.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nopjbspw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2mwneoigv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cftniure.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rnpewvkk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2orxccugf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2laoabqpm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2jttlvygk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fhngbppy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2swbsbpsa.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ghyvtjze.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zhtvefba.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2anmotjeb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yxqwyzwr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yuuwgzhk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oaqmmqne.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wobbvhbs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hjqwvyal.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2bpomcgua.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2kqhnbdzr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2trythlqt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aqbedgps.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yiydkboe.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2njqtftje.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zkuoazgt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vrpzegdo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2njsquuyj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fnwlbgmx.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ltpotsun.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2tpqschas.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2trjcxpio.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rjbsdrmk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2guoqrmdh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2ipwowfhz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vqbbohxk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kewcagxp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kyrvdued.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ngakgyix.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uvvetgoe.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2youskbhw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qsvarpxf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2thurigke.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2tmtvfgzd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zgvqfpos.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xmebqlgm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qmclpido.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2chhwdkbw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2jxpabhvi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ubwcvjci.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wmfewgxr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pgerdool.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2osutsent.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jlsjokwz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2mzcgmdqd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cqizptqq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rkbyovig.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qhtzkuws.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gtivhtad.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wnwmmqkj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ekuhubhe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dfkfgdji.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pygvrmow.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2goutuvah.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bisjgxse.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2qraidugz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ilpcesuw.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2dnhupjiv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2revlawtu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rkyzfxug.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gvyvlpiz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2qnwbtckx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2keevhact.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zvxlpffl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qtjuujxw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2urkwubbt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2feaqsavh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2juwstnjl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2vjjyylkn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2vfchjqus.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dyrypbbz.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aznskjnl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2mhlbdcgr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2shufwugy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2qekpzxbo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2dvfbpiql.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2glqtfcal.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2gwhvyerg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2uflaxoal.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2flpjjndz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2yrkgsich.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kgmilofe.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2zlsmlcgv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2echawgok.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fjpgrlzc.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qyydtdaj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kovmizda.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ikdjlqgq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ssrvbwyh.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xlbywato.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2rmmbtsag.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2apalfgdm.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pafummaa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ievhylhh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mtkxgyiw.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wxeeolgu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tjgrvqgl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2estpqsaf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ldnokfhy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ivfgwcbe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfoxpuhb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xghxjtuq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvwmndyx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qigcepkd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2djuyuyfa.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hmwtxwuq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfbkscvq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2apulqpxk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jzfpgqct.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2dwhmljrt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2mfhiftal.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2hemzejty.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ecxvjypg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2byjsosqq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2csqpyxgk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2kppbjumh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xnaskrjq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yntmwcsi.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2woghjlis.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xurlyxcr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kkzhabwr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xecvdvhf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvkbmcox.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwxajqh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rujlvxjh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2lcoigqtm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2asivuxsj.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2asqffiwh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2pprxvcob.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2pufqjhde.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ucbqfkcs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2cetcmktj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2mcysmkrh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2opdrzzxj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lcbtghwq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2cfzgeyyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbtkblxv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2lgfuqdlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nsdstadu.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2uivihhxn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bzzofhbp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wltyeguk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tyazvnkk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xhqikyny.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2umntxygl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2scioqqff.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sbgrmgqz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hwnbdyhp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ypdfruvo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2rpaaxslt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2imulaphs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qpsgpphg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wbwrtbpy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mrpofrsv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qdpcjvxm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rmlvysdl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rjabuswk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ltwuomtp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hnwkaxrq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wsrwadrp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egmwwemb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htvgfcdm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmkkpxpa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hcohdvpa.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2kuiylttr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2btruougb.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bfacpceo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xrtgdheb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cweziqcd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qiuvclpd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkqyraj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkecpgbe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2rgbwytid.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2nxvrnvnj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxpeiisw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2clipnyut.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2sbpaivtf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2miavbmyl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qxykknzu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2axcpvfql.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2swfcfhez.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2cusofisd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmjfqim.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrelbjoy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2epbijzdb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2efmqccgi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nodlusia.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fzejvkkb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xxzirbcf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ouvhsxyr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2qkdzhqzl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2oujoridf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2igbjilro.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tgcjtovw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fyavhywv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bufdebbt.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxyqnwcz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2prhvhlvn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nrhlodrh.html


<!-- 参考信息 -->