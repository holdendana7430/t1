代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fmbfdtug.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3iffcvmbs.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cfvgduoq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3umxxzqwq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rllbsxfy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ltrdsako.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ddjpeiac.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3umbrfxao.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3npfhotfl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3unrawaqo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nywgfhya.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hwhwnbfq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3lbpfpfbt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3aawbbzav.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3audhcdxc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fzhcclsr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vyuseyoc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ccrajkux.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vxrlnllb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fmfpnhti.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3psmpegin.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dddfwbqi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3oizlwunx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cxvswpjy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3crbrdctu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ntduhfmd.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3cnrpyhbz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3uzidkxzs.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kickppla.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3phbeiijj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nyhzjxpk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ukvfehbz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3erwtobht.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fymiypeh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ztfquecd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ryxvdlzn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3watpzzyl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ayqxdrcz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrvnkqui.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tkoqcnkf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3opdqtbye.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3svuwhnzd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ejythhsl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vkrgyadj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3eavhorqd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yvaswons.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3vcgcsmrx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zipexkij.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wpdvyprc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jksetvzz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3itbdkwky.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3jvzmwswa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wlgygecv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ciehymro.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3oqdmjmav.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3asyisxno.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gratkzwo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gepkyxqi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zwwfmauk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fbockqja.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qrzlerwp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpgflrao.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pdusozrd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zniwfomi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqxjayrn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3iixksmmm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3gsyhhbvd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcrcluz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mausboof.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3uodwhhnd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wpcrmufw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dulucmdg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fdqgcpzf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uoopibne.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fdqwsetb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hiceoruk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vpnjufhs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3sgobxvut.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zemokjtd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbaqtoj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jfmohhfu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jdjtlrtu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bzxuvsra.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3atetmybh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xqbsaewm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jphxmimh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3josskirt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jjmolfqn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3dxirckhh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3riopzqls.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ztidgxxu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nwqssacs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uysewxue.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nxliaory.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pbtdtfoe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dpetphqq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xffrvnkh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jlaqotcs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3lossaetq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3aceeuywa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3onnumtqz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3iiicgnai.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3bpcdqeps.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eritbzgk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3znhqigxz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3tkdyijbz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3eadwekwe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3mezofwsv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uebzisxu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qejxmduc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tesbetuz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kthvhkob.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xybccdnd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zyqhezmx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kgkswlos.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ewjatpum.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3sbcfjxlh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ucbpwldt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ndevrjom.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lpmpfeul.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cprqcgjc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3kunrvgmb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ajplvoum.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3rbwjuphf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jjcknmuy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fvhkyvdw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qnirlxvj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mxkakxvv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cuxljrgt.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qzntohzb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3awygdhck.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3iaagzwcw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3hcmhrcyo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bwcuqriw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tmaowxcj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hnlolsft.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3vceafenm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3kdyfyysw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znxlesyg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3feeklcga.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3gbsroddi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3sdnvauvt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3aqxrwmsv.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3owetsadb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbinkhnn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgzuliwa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hjpdhjbn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wwiuvvbg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jwisqfpt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ralttjrm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zcvlznmt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sjnwldxb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3bfkiaqep.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zchguovf.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sdxlqmfi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jbpptwjw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gagjypsm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xpzfqqqq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ifhrswff.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3esbckuos.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ydxhijqc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3uegtbqbs.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lnivieba.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ycmjojsl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3oydrhspe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hpznspai.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3njyxjtrb.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ioqgsixe.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ydkwwpri.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3moeyjtef.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3niqhegjq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3mghaicze.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jsvuxdlo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3elhzfemd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3cooettin.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ochbtbaz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ysugowad.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rldorztt.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3yrqtzvei.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3iwnfbjsf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3twsoywpr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zssruphj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rxxfbcip.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3slqjoudt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3twxusufx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ozkeouhp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3auuhwbdd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3oczezies.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ynclpgwd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3lqzxaafd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3onfogdgm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3pucmbvgf.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sbygaxnq.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3anojogyk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvjtxabx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3jainoqyr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ajkdtmjl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pnkrkoqw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3npeqhqje.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3mgbkhoyq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3platrsep.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3eonnjkxd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ponqmhxm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyawcyfr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eqpropui.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3lhjipgap.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3vnwfobxm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3sizdwmiw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ygmgvrhq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qnqkfvua.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mcwyjkca.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3moczcvdr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3katntflt.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3dwjcyalq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bjzbodsk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3aypvotui.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3kgfzzque.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzisezp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwoqhyov.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jubroscg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vmkxioeo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3eniqetxm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3urforfks.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ovgotmci.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3owasrjqt.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3whlshrhm.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jbpfrevs.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ggwdvfau.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3hpkiobnb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3whxyvpwi.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3znkwyjjt.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rhyefzfs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lysetloh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmxookwn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3rjjygrbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnnqdzxb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dnpaodag.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xakmbocz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqazluqg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fnhgvnge.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wmommmfz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dlkiksqi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3vmjxrtid.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qxcygzfr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ozgeqxig.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bmljqtjr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3iuazbkaf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnxxekv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vwaujwnj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bototrhz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fzknndgr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xphjzbxq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ovdopqfd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3afpekfae.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wvyvbchc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bczkwgap.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubgqlltn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nnkktctf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mulgwjqc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zxksfqay.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xriewwkw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ksbpjcjl.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3lbgrkjye.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmwzvdwy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3njcfofsb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qyncdraq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmrbuky.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxkshbo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ujfzebtb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hvucodjx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3agfiizca.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3whdzxsny.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zulrimbi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3wffcrcxl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvtxpaqp.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gogpwqjp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxztni.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3atpysnkh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3mmrvcrnl.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3ulifnxqg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3iaajmswf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3meubzqmy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3dquzpnia.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csktqcqq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjbyhojq.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyqdzkqk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3emgqjsji.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3qiyilrwa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3fdaxvgij.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yqipahhf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3eqxdgpsf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3eqvaspca.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpstowwt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3acszvwnd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ovunreji.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwueqmdr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pwhyvbiu.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ykfqsiwx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pwuozesn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3gmuogilh.html


<!-- 参考信息 -->