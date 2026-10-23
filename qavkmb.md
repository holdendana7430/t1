代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vmdobjnc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rmrdmseq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vjltolfv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kusppexi.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dioweuvj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ktrfuwuj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3jnsoycnl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3faxlecgz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jafhoqgr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3batvckwq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lrowebzy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aocvqpem.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3rkpspjbd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xdcgiayd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sixtfkaq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3opvawacx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lwbjbqfx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3mdyjwfrm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qmzavlwj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gygyhkgk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aborrugd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3daevocst.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3alyjlrjx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3evlrgfks.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sjvralai.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ugtriwhi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbrtfnls.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3anvfzmra.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3sapdctim.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ibqkloke.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3osgpxwgy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3fsnwaqvn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3pghvcwjw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgmnmhe.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jvpgzwzq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gdriepjo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jfqoropb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mdmakwxt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3awcgxnti.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ztjxuwli.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iqvsxigd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3doqqvseo.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fklaxhdh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gcnjbhqf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qilddrko.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nlcmgznk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lnyrcwbh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wotfqcgx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fkybfuro.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3stcpyled.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3uhmueoco.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lhuxprwi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xnvyyuwv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wbjhqicz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mnenlqgc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwohwdy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vuoqqqjr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ytzyvlmf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ofxrajnc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hsxglnmw.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3zplmoojj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3clezsjys.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3flfdodtm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3apwsacwi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqbthrj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rvbexbof.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfsneto.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgjaqbp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vyujpthu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wktrmwnr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bqaruaul.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ebtnyqkd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ijgricut.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ryhedigk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxipdpv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fyopjoym.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvoheiv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3xbygwgwf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3eyiitdvo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3etkapqgg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3uuzuugts.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3bnllfkjj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3uflpqgjl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qnlqoprq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbhohifg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3prgkemfd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zdvyufmb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lkyifxqj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqhamoh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3nsupoqiy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tpkfhkhd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ulzldvwi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qwtxksdk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eomsdlpo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jwkeotzm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tjdzqfld.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gcrabggm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rdirgeys.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3wwyhkjxz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nbkiowiv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3yqggzwhc.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3unnyikzi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hbqhwkvf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbflydt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xemcefgc.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lvcztoto.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3pnlovrxw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dpokmuyg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikagdaeo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3trletylo.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bygwlczy.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ytlpcguj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wwydweuw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cotsxxvw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ckitflav.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uplwqvzs.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3lhayhmxt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ixealprr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3emgarpqf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rfugqlpt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nqfejdgi.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zucogvao.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cepxtxoc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nietgflv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qmgyzpcf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vjacrubz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hztyodof.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oqazmtzr.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ixopztnc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cwghhxea.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wkmrqriz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3udshnypy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3yisdywvk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hbqkywfd.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zpzhjkwi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3pkleqecv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ozkbkmag.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3pldqmhwy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3paongtof.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3lbnxturt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3sebzmrse.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3mpmdzssz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ujtcjkoz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3notdolhb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pokwvcef.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lbcumxpa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uuewdzos.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mxpigorh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ftsjdugm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkqgxuad.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3coetuqpu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccwtsqja.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qcmymxgk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3epwjqwma.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ctuastnv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxltpku.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tumsnbrb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dhboytgu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3oolrstda.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3xxbeewae.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fyxpbany.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3bxkascrv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mqgjmwfc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3szainqqy.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qyhunsij.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lxutvrqs.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3elygfvuh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pewrcsut.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3biukgfjt.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3npwiwxfy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3jzcbyxsv.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vaxkgclm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3dswwdeyb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mggeqhqt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jiunscor.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3blnjcxjk.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3zixxqnzs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tkdvcrvm.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3lkneayma.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fbwjetsj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ztwqdgut.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3raenasjw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3malmrtit.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkdaqhqo.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dhdsryvz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ijftzgil.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kzqxmnyq.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3qmnzokrs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nbpaikvv.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3uexdkyko.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3oimvqlgk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3obkihqhq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3stzhpldz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3nlqgoxdy.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tasioviq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vnvaicaw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3taypwtfx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vapqgrbe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3orialeyl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3irfkrqyd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sxejpffc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hhaxnerr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fhcljfti.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3vyoydfzm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3snkgeupy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3gtsyogrd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jgawdnly.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wwkcewxn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtorebc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ljoosfpb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3agvsvsmr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3jjbpykgq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ioixtsgu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3mqwckdna.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ziapaovp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vzhmmdrx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3izqwpamm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3empzfyvr.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zadboqdm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxjolrs.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttypbaxq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfljvgcz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3axrtqjmw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3swghwizh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ootfxqba.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3laksdbej.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3wznziwwv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qnyqfrci.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nockzlrr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3tpdeexcj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3panhhyvx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3gzanevgc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3frmbvssv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okhbihlj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dlcjaile.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soqdfcbi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nnfquxhv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nmzxlhkb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3reqxjpcb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rsblfshl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3chowlykd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fnujhmyy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3znolfxkp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gnzmaska.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mplxxxbm.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3uzkedqtb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3huqdzyla.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iguchrfu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rfdaoyvt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lyoupeuz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zlridakb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mwcfbcux.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tqptulcu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ijlskijh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3pvpwuxeu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3vzuyzfss.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fbvagzyr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ypojuxwi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkkbtxzt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tjlktngx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gunmcddh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3amdwmnmu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3mhtvjdie.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hlsmdhow.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3osabjdqi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pvlljpjz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sixzilwy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pxqwhrnj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3eeyxtgbt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gkahpdcm.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qkvcwnqj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wggnwczk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cptxuooc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fiaorxxo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhgazcw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxozsyuj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ceflmfly.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgghyeum.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yslwkbpw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3gskycjtp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvucbrwp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3swsvdewe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3lcazrkgq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3xxybuvdn.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3mafswbcg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3anwzlcbz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbyiqsqd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3sjvlnzmy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3adpnolod.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jequnvxp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3fazjkuml.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3hftelwqk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yqokqhar.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdhfrwgz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jephgclg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmsvjfwk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3wfvxmzhe.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yoaovico.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcaahqrn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vmhujkoy.html


<!-- 参考信息 -->