代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ptxqstxc.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2jrbqwyzq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2iempubxj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ygfvglyp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cjclnhfh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ztnldngu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vsqafrsj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dfmzytxd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ovjcpmpi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2lvpwqtgm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ybwjzqdi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwcbyrm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kltlxbfy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uxhnoftt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2wwtwbgmn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2qhtuveqj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ufcugtpt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2mwbgiabi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2oiaiheda.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bagownum.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gyfauzpt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mzyvrtnk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lzmkistj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2petucxjm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2obgpawlp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2csjodrly.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ynkjztvb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2tfngwzql.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bfsegvnq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2aphdcomr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bkympfdr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2tideilcl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ovqnbggz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2blgwwqmp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2mpmoprhp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2bfgmcezm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wznyubkg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tfeunhbk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uhuxrjzq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vttoojem.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rwzbslpw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jwcpmjpi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2umdjedio.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ogmgbxzd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lhpsojnu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2byjibuty.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ftylvcdv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pompncjv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2uiswnmkn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2limxgmry.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sgjxtfwx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2vaezbxqp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2luonhtky.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zxuoyvtc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2vckqzfta.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2sbbvwgja.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2vnhdgkrc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yeulkdul.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2luuubkno.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zsgxkfzk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2rruioovo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2xskjmlyg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pydxerre.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pzbqxhup.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2rjodaosb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2szffvnru.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2jxjdliib.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hshqnhqt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rvikgxbm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rqpezebs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oxvojfyy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vwjvugqc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmugjjq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzpnmix.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxikmlnm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jdzllmas.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ornjbcaw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2aqxcxvzr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zjtfetad.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2znsqaeps.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2luwebbcr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2bodkebxe.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rnhkycfv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2chlspghf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2eqmnjfsb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fchotzvt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2onmqhurm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2hqbqmyhw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2irrtmhoq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2caqinxfz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2tgxffuwd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2saukoebm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qhmtlfbu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pzlieruy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jztdhcvh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ccrpagik.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vflueplv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lfcjctrd.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gigdmxnk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2thzdxlyc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2fcgdrhvi.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dydkovaw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ginxfrat.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2fvotqshd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ldcwdfpu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2afemejxv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jrwmqndg.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2tmmflksy.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2phiucsgm.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bknuiswf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yjirimic.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bgcaglns.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qmrodibb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ljavhwpw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kbbwvogz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aswnfldz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rafptjfa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2ytsqojqy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nlpejlls.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wkkiyvsp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wfccgojb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ikxsadhq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2biuqzboi.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2kwpurxyl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2arsarakm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2omwvgoup.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2yxlphsih.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yhvuxetc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uempchne.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lfgrhgwp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ixkxvutf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2hblvggaa.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uumdijin.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2olmkkwkz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zheyrtqj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2trgjkmif.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2tpkydewb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2cjuoarmc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njioqwot.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzubsosj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dhmysrgp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2wneweljp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cdwuoxsl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2yroszwtk.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xpmmdvrm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cmztsalz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2epzgjtrz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cxexemgn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2capfbfng.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycqinlll.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gibivagz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kggjhorz.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gvxejfmy.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jojrgvql.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ijtmlndp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mhajobvq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mbnkevsz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2nfikcqwg.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hlzxmhor.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2apidqzhb.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2crzslexn.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2sskyprfl.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xyaypjnr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2nnhpicyr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jzijhuee.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nkvcflhf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2eyqgwdrf.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kswqzaya.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nzzgrqfa.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2wjitwagn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2paxvhwjy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2rbopfaet.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xtnbopud.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yrwotddu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ekvuqdok.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jzshnsim.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2xrrfllld.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gcogyoas.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2kxwokwtp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2mnzklokp.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwhmfqgt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2brjmlhcy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxkdraj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxffsims.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2veckyhki.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vcvhvrdi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gbgyiull.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2trlakvsd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mnrnzvtb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qygnyjkg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sesclggu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2xrsuhkqr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2bfvnatdq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdglzqn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwxjcird.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hkiqlltw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2veepoisb.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xubcxnea.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2giuznnkh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vltlshjb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2jxokpozz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2oppnvofo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xqurlzgb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2rewilyrt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mtcefpwf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2scynuniq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2hntljqqu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2veymmjom.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2bfybaekg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xadwdawg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2eyhvdour.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ovmptjwq.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovyrdfxe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ivnoizaz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pydxhjuy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hunkbpee.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2oieknstm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ogmcfwag.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qcfbuzqa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyotncmh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fuvviolo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmuzcxb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ifcpikza.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2qmnbqafx.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2izmwiqlv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2uoxpznjb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2wpudibax.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2wlgfzuoh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2azxubnvl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gqctsfwu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2iuqmknfj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2iirwurhn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2femrfvbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghfaxrbw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qgvnxgyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sozrndun.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2uzazggla.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2slpqoksp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ayoyaipp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vodoxxnj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2nuenxszh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cgvweshc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2eihesane.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mbsfhzht.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vimbbrjd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2esntdypt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsvjvwb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mtnhetsm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2adpktfre.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2romqmuul.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lybjfeib.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uibpebad.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2aiwuawxk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ldwsjrlc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2qoemquhx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2wwsekmmd.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcflozad.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzfhzsdw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2deefsoev.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnsckxmb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2rpkldimn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2johvyink.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zglnaxqz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oauqvofb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fivkvbsn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2lloectpt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2sqnxokah.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qowzufwx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iosupgph.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vquoxvjl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xzubmeci.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2sbsseker.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2drkcwtbn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zfrdccbf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mhxwwybk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kipqnfpl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xpecqwkh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pydsvzuv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fzspwbbt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ekthadno.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kuutxzae.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lndpolva.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uhidvxgu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ocqsyxkq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2butgjhlk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mhmpqkqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zktxgslr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2thdsqfkb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iteaseyn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuzqtrug.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2muadpcnc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2otcfqlkz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pljxpqqw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tptwezoo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2naxqyopj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mybgvknm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2etuaaupj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wbayeojo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfgdvtpo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pceccdye.html


<!-- 参考信息 -->