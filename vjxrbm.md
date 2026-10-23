代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rqsgwium.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ccegbrxd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qxckzzkl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3yymdtrdd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jcylxzdp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iluqexsm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3bnvqszpy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qhmkwgsi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3loxqxdpm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3jklclgfo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ubyfzjrf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vdwqxzfs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uetlcody.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wdsuyxtf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fenokznj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dombtson.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ntykxzhw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lxeckwdm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3juogmpxj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kjhacqwd.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dzxwsevr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3isjfjepi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dywakpmh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3okwwjscx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wjnukbzb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3olrcryxs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gulpnezi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3xtmbgcrd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3slddcphe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xnawtxap.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxnxxe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3cdrowxsv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3xjmqrrjd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3lilwvpsj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ibdgaitc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3klpugskt.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zadadxvg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnzboxxc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmnbgyls.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ikthspld.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lemseyux.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ehxjykxl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfypapzv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dkozgaah.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vmeqgyyd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aczwsvcr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mepacwnp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vcvrtpwt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dewttzsf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3busqrmhk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3foihoimm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3feyadcnz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zmgkfjsj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rlcfdqdq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3aqnlsqit.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3tlpuloiv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tbklqahg.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iafhpnmn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsrwxvi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ynehmujj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3smyxkyvq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xnkzfxrs.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pkwjguku.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yluughbh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ptrjzxoj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3luechrjm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3jidokvgf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fbokpcnp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qbjftrxl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3exmkwuzm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3teqwredm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3psjqhovd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3prgjzcfz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgugtro.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vrwvrjxs.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnepmrij.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bdsaoyyg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vklsxrgo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ufqwuohy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkfcfpuu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sodqkoei.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ewmzoztl.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3bkfsrjsd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3biudxjkn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3etmfjskz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nysfhfsn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3taruzaup.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3hldsofbq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xslcdasr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dgbgrgxv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dorcudgf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nkxkxiek.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rywhjxyg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vjdjnuqx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cidqqwtr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ccmukyjf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3krilvikh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tsdqwspk.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gpentagv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3lmkimyjp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3yqaqnuuo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mzlxjehe.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3mlrjwixp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3lsojshrn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3awmmpwjr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3kdijqgpi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cpvpxqxt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ntenaccc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qgzxhipt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3beakccnp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uupvfwtw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3stcmjslg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ligkhprx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jygkrrrr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qlepeiqa.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hrhmgcos.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kkghghsb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3gmxghywz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nbanznkh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ofnnlnlm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ddixrczn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3hvxhmkzr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mztboneg.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3iwkdfpfm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3evgdlobi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ixhusfoi.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lxseirqt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ohoskazg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3juaeawtl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nyckxajo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fqmwjenx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yezsslqf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3stsgpxza.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jrjnirgr.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3pqoixeke.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3yvgshyzb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ucpysecz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3zbdhjskg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3cfvrymht.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3psrxller.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jtbscjlb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3lvdakict.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xbwywosk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3czdxjuev.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yrffskag.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iflviyzg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mfinqxpi.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xhtkjblr.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eekzgjxu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ncujpayo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mdgnsupw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3flixzlar.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vtuobynf.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3gdfqelge.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jrosoewm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cehttbyf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ouorvdzw.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ubdohxbe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3bptjsdma.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3beuzwapl.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3bqzrpijv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jojfifos.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3kxvhvidp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3vloloncu.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3woutqerp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jabweeyq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3daofrwoe.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3koribelq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ecmqpoqp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ljafatuy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3cazqzdly.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3cdfvwysn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gjdcocxq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qprmzkkt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ameifstj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3icghaldr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vckbnaoo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3xoexjulk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3gdnhziih.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3wwtvwrzg.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3knxwdtlx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3skdnndmy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bykiaaju.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3eisxqqoe.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kuzczayy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cxztpgdv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nwxbjpun.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3thrjzarf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hzvcpnpg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shoanqrl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dnneyuzj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3croqvbqj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3lkvclugn.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cwqrprsr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3dwvwlomy.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dvnjbhyg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3zodlrfea.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jhdgzvuu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vwhpdfah.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzoftdnc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3eympbnlr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3djgvsnve.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qkqqqjlj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qzdvgqgn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nlcdmbui.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3exadshsx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3burgtmrx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3twzpgvfq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3dlgizcsg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yfvwuxre.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fyheoprt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3pwqcrdfb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3iiqdvqql.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3mohtvgen.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3iznqcymh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qroamokz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3gvesttmi.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wxpduadv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xaomwfqo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3usdhkeum.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3afjayaev.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpqomdtn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3auayqiks.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3crlixjgg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3tlssjqbs.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3oykqmpeh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3swbpjcxe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3icuveddm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3ojahswme.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3fewwvhae.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3povqxcbh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3epzvijdx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3isjhwrct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzehnnjb.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bqeumctd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oskqzphg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wermpxzx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ivkgpgby.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tjulbpfg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oficxgeg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3idkqakus.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cnwmacaw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3garqxrwp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3uughlomj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dflxgygx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ffpglsao.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3divqilwm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vdycdsvk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yhzhjfbf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ycpaghcn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vsoeucum.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3gdvymklu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fqxyttlc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vijlpaat.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3cqyzvvkt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xlfrbzyq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcvmtxep.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwhsbhyy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfeartfh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3guxkmybv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hfembhlo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zvwsriau.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3cpeubmey.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3vnqtkxfk.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3shlhnymy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3aaggvhoy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3btzpzipn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofbduzzl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuczueux.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vbkrjcaz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zyyjxbbk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eivvyknu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ipglmwjd.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3bxmqnemp.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bfiuftuj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pzpwlbfr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lhdvlssj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnevhws.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yoayqaxv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mheuugmu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3dpoegfrt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vazdpvcm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jkybekbc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3irejqwbk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcqpxsfr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zxhoyjqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgxybxqh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bovtdbpp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3yimzwvhz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjxqmxyn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3odyckcgi.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3hynshexz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3tiewkrlx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pdqjteld.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dmkxicmx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3umbpkhfi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3albufimb.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fhubgaou.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wqywxiuh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3cckdarnr.html


<!-- 参考信息 -->