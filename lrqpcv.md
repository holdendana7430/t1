代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ptfqkyys.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ptjogyvn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3noqbyqih.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3frwaqbxo.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3egxmeehl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cxxfqmoz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3dafvykjs.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pnnmyjjf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hyqhwvlo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3nancfdoe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wsvvghlq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tebusgbf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3olhliuka.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ulfhizyb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bgzktqbi.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3mdhxouwy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3acfpxmay.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vyjcnmzt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3mmlpkrdr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wpxeqcfs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bcyfmayr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3odzywblx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ejcsduyx.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3aihhyaca.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tyahwvuz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tyifzhpz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3cpovzsvi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3eqycuakp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eesrggth.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ginzfmmi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ribmludg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mdovzgry.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bppwjbfh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3dnyqldks.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3zlusgsmx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zgjlrnca.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3fzulokln.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fwxoshdc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wjgksgtv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uoskvsjh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3psguocxo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fxmvnyot.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tyjxidtu.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3obpkphof.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3klmnwvyy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uujgbclr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zkaafbqt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xxfvwhir.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3scxtcguc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jcmpclbs.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xzxnrhzt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3xuqsbgul.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kjyihoch.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3oeuwphsv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wuaiufff.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3oppimnze.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3prncsivg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3igvhxcfc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zxhylbnf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zkwjlqfp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3npvlnfex.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3gsuqfttq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3fltwzvnj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pncvedvc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3atfbvlgg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dnomfzdv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3oikksmrm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ittwpkhd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ottexhwi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3smwkhjrv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3solvtnfk.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3epbejhnt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpiztbz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qbmqpfnq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3topxampm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ydqxdgjr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3majofebg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3omrzuwrv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ypblayau.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ktqivfta.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3aniyuejj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ftwdeven.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3niyvusmm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3afhzlfjz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ybqmenjm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hwgskgkt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3rfnqlare.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wqaetfgj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3oippiqri.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wifwxrqx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3oiwqxjzk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pctyudrc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qlnwfcuz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3thhuwwip.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3znmocqrj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dthqulwe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3abmrplhx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yqhcjeag.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qylejdqw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3tetedezm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wqwcxgjm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fzrtnlug.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3opqfutna.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3snfcpbqn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wnguzfdk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3elsykfjk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hkdpbdxa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3jdmhjunm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dijsuwsm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gmfxusqi.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bnkzifdk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jmtvqqze.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kfdjevji.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mmkjsdbo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3assavetl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3owfvfjde.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rlxdhxro.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3wlwtgjgh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wevqhgat.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3udwknbxd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3buuzgody.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yyrdxlyr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3axkagmio.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lbgvgguw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3khpnxtwe.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cyiqdvri.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jhchxwoz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rioljozi.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dcntdnhf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mafgnsjb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fdspzbfy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmhrcguz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fietyzno.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ffxdznng.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zjxxhomw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3ajuqpqhz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3bsggsooi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3brydmoog.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3pxexeklj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3egjdyqay.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3sqjdaxhi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3twaktpay.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3garinnjh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3bclyfwmc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgxykani.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xjxqtkzy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rqeijljh.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tudiuqdz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ymexzgtd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hqskhowz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pkikssex.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qpuwnfys.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bulvxlti.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3okgaxbsq.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qricuyap.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3mgosbwes.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3xprpzeim.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3updhzdwr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zaemthig.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hhdzcmas.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3oivsmvzz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3arjmmbqe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wtzvlhpk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3atgisceq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kzlbgdxy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xwghiuai.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tpvfdjbh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hpdpwsxa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3itkyujud.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3yqpjircy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3crszrote.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qbujsvrp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ovzytrxh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kikyleof.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3vqvbajmd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ozwrcoor.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3qvdvfzrh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3tlefrsyg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3efoebxyv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ezscvqld.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vzjjenvz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jvvjkytp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dupxdmip.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ldwaayee.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3umkzsaoc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3grklqdcg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lvjqlqzd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xyiscyxg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3evcchcrt.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfvphtnm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3gdqzyzdf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3khnxjtvx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qsnanwqb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3pihwusne.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3vkuykxjo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3cszyuhth.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jlefdgfh.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lypkkprs.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3nuxjktaq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3joohgtdj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tyzipehe.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3obvtrlxk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mqqghgho.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxcvhog.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cjywijgz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ofthyqba.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3srqfnwpk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3sflazgiw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cucnrabq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qywgybpi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3etphlkre.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3triovedz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmypbhzu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3xkxpzzzc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bqalhwgb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kifcsnjs.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cvdppbzg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zyablnzk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pxdredtr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpotpov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3nevmckqy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rqzhsvnb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3xkkjiufb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3crpcnzsp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dssqgldb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3sicgygcm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wsfdphxl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uaxergcw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3gxqmkair.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fntvrpjh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3bgozauia.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3pwpmdpdo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3iwyxxcuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyrjgavz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qupvlqab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlcaycut.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3fguucqml.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vivipbqf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lktjpbbq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kdcdytpv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jyipylmv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3icmznreg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pwciqcfq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3dkumumox.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xgttollk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3eejehtum.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3yaqjyyua.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3llbuwmlo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gdlhythy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gneempfl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tqjcwyke.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3vsbnhgtl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3udczbykb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vfopldsw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yjmbpaom.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3xfnsdsry.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tvzcpeyz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcfnhnjz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gyvxrqpf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjvhslnr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qazzglph.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3vwbpcfkv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3itlgjgyv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rqndvtuk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mocucbug.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbqhhzrw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3advswktb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujnufdmb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3vzevzojp.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xdsirfoz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3guxmlcpn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsmgmrm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nmaruxrt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3najhrsyg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lnstzsuu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bacysfat.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3khedaibt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vuplngze.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3uzrvpclo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rllhhyir.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rktljtio.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ttgbocat.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xohkgxbr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3uetlmaso.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioauguni.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aqfmcrzp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gejeyeqy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zknznazh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3eskkiewm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3ficpzzyk.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vnjzodeq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pvbjdoah.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjycbeih.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zhtffcpg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fhyxjqvz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zihbvsyv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zoirwpof.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3tttpcwss.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3urlmkqaw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3anmuvgvb.html


<!-- 参考信息 -->