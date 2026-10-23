代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rvtbchqh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yjzskkbo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hskmdmci.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3sncprric.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3phoemkcw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uumpocrc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3bycfnnio.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yjyphmgq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mkvlnyyu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fttgoksg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cqyweufh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pyakmkti.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ewrimxyt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xhrmrugc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3vrulsqwf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3uttbgrmg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mkgycfkl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jdtrwddp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3frdvxoiq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uvwphenu.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ubrjxhqk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lvfptvec.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kmncunul.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vyyytcap.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3urclhnmm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3phrlsjda.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktyqrftw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zzjeghaa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbbwramz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ptjjnbct.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jgnycuwu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bxmwoimn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxmaqee.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtrepht.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3pbmyljkb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3hzymapzh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3xhgdrigp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qxxbqvdg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnthgmxl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tljezoys.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vcjxpnzr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3avhhahql.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3smxrmkqx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3grqshinr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3oswejssb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ceqpoprf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tqvjjzpm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3geyekmcb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vmcwcdth.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nnexvuqc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tyjxlnmw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hcgreytz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dulzrpxy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kyeaxctt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3htlyckuz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rmqnitei.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3pscyaagd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ldbamhuf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ouwkppgq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3oizpkksc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3abcqtozc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3khmlcckf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3iqjffxuc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bqdwxvta.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmyjcoho.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ztbevfsb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkdpdut.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kuxikbzk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3buvpbdor.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3gxvsthqj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3owgwgevx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vodgfjhv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3umtltsvf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bygyxnje.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rtoowvmy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzedfyw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nftbpipw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3fpucjubb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3otwwkhsh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mddegqta.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3sptgvuds.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3hwnxrusw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ocjakfno.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtttscet.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsdzrctn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lnntfaeq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qbwbdorg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3dovjqpnu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3tylnkmdo.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3oaqtyboo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sxfkconq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kwspdveo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3snlsbkhf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uwivlyng.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kcfltami.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3shvtmazv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wdbaywcw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yohlvgga.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xzvsxqja.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3aiuivbvu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jvsghbld.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vwrlhsoq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3atkqoekq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3birbnqzs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xefqpyjt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cczrebur.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pinzhpwr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ghloaxds.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3itqcukvd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mcryqvah.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kzhyskxv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3czltyezi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3trosnhmu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qfoqveyf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hisvcdyj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vikvhhog.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3adqddwss.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vzmcpcxp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qfzyisfw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ypompjgc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gwffyujo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hxnddbzn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rxwdonwq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3phlqlkoq.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uihklbdi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jzreakul.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bwruwwqh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bozvkttz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bffteodo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tpxtecgi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3umkgprtu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3drojvnwu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3diziggua.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3grxjxwww.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3iwtbrypv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kpompmqm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3gqaipjjx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wagdyknc.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3iaeichkf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twuzlliy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3freugils.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nbwzwmbj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ulywelhl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3fioqgcwg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zilmhpeu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cbscmusl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3efohsyed.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3evikquoc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3idfcjrls.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjzkffga.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3onezoqjv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ecybiose.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3otfjroux.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3iipzculk.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nmcsdcju.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uhsimlyw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ojrdffbx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3gnyhzank.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3sxrypole.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3zadngnpp.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3faephwbw.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ykzykomd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ihmkoxuz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3cnqkejud.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3likggihh.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dvvovsvc.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3wdfwaaoe.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3evnjomis.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qvdslufy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3aceqwnvh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kwpjdkwp.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3ipkqunlv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ulrwnyxl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3feqcahcb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ikeneskw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3iugsxiai.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zwmbwfop.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3yepjjczj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lmgcjdhb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qnjeytqg.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3axxahrqz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mfliifas.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ntnmjodk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3biyjgafg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ausgyxol.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ztujbobf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pioyxdug.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qnfifvnt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qsumeqdd.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldycdhtx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3qwlekwgr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ltwdytad.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pobjcnns.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kdmyhswn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqznptjt.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3noovtyoj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3krsrqxih.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vlhsolql.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jdwinqpv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3tmrtdysj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qpyddgak.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vhcnsvsg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xrggoovi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrndpqfq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jynmxjyp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zferppje.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fmbvigcf.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qyzlqhsk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zijvfhji.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3znhskswb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ybxqjyze.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hktfjnll.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3kdesodzx.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3zzqfatna.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gccxjxby.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3otfilrbs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kjjmzcbu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3iaazyldp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbghtham.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yzjcocgc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmofuv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ulfhapot.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vvqmtcsv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3cvakhtil.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3mahaoulb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3idspgvmb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3dxuibnez.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3oivoqbzm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3aaanpucp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3buejnwnk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mouqwwlc.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uwaelnib.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcosliv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggmhzcmo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jsuflgce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvdazloa.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lyjnphhu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wdniecbb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqhmhai.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tsujhxds.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hgbgjjno.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mfoifyej.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3nkhjsjaj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ggdlobbt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gocteelf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ptvltgue.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3tesgqucq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3haoexlwh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3knzqkijr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yfmvjjsj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uucccfze.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3kshbqdkr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3fcqzpbsc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zwkzyejp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3alwbnyns.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rwvyupgy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtifbmwr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bcvmtety.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3adfwdrcp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhbnzlg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3wmtagrte.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vbqxspyj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jbwrfsng.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vohmdmoj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mgkvygyx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3jcoiiica.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3duddegyb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ktybupzk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3wjwycuvv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qdsmvphv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3fiektgbm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyohgklb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lbeozcqv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgckpxl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hylbvfqu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gblvylql.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbkrwqd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3gzxjgcnu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzegvzgu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ppmpirmk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3onenlzbm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3votlhpnq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3fublgdkk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odrilyze.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lawxytlq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3anvkbqee.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3xmdxwlwq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lzzsqfbg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3agrctphg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxixsmm.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3lyxchhxy.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3bjljkzge.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndywdwsy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jncnngti.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sfyifbby.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbeumxjl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3toyusfzq.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kttuzbkm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mflsevgk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3uudhkveq.html


<!-- 参考信息 -->