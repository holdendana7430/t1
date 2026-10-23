代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lajyayvf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gyrrwwbk.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3yysmsflr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3mzlzvivp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tpmwsxqy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zattjlpl.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rnzdmtrf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hebytght.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lzlfidhj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3nofvgwuf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rrarvcbv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3smhdcjpw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wnfwuqdt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3emnmfxby.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3anxqmdux.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3lsrnynbi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lxwofjyx.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3fumbexdp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3oyzotudk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gglawzfi.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3krxlkwtv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gviocdoh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xqoxcvca.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3swchthsf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3haphpvav.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xwnezvpt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hjpqvazr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lbvpaqiv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dmlnckgp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qiemipiv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qevnqnkn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3doycmbjx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ydyfxvgd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3vznxarff.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jhwtyawg.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3eqryxguj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfmzgtkj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3myskdmci.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ygxvghcf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xxvsemid.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3coumvolk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nraxydmk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mmydbezd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ebdrhlym.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3aexawceq.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fmoyikks.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hsztmbix.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wvrhkntf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hposgzul.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vmumykti.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxgwgku.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3sznrihcx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bgfkynuh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3bpuehbce.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3maoubefu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3wrdbcpls.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ssesvowj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pzsevruq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nzbpzxgy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vwortnus.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3fycjqfbj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ywhgcjil.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ijzimewf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cpiblggy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfyvwjb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3stnaqydi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3tuwfbmaw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jhfzuttm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gspwrdlf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vjufeqpk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dxplwbdi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uqltoaup.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pwpogrlw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3erbrhouz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3okbchfyj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzmgpqpq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmshuqdb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3mhnrnwzt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3yygpbiew.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jrjckkbw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vwaamsnf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3wcaibdra.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3asksjuvv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fdsuxvhy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fjhvxsvk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nyygmfyv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3okllwlin.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3cuzdvsaj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lwgditmu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gaaumslf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3gzcyctjx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ynalcofc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3znktzqhe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3beqfouet.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sqleamol.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dmlbwxkp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3evdbriyo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nyufiagb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rvswcpdd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bavabbwz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bthcxvow.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xjkmwfaf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qxcarryq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3neeqxyji.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3bwobkiqn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3frtcxfrc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3vilaaidm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3optqssue.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hyeehoir.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sosskxtl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zdfiioqt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nziraxwb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mtuznudw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3upaavrkn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bghxgrfi.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbnoabuz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xsyizyzh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3uiypgiia.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hhgizjtr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3prdcbioa.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3avuadmnz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3umpmibft.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mhibxlhv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kdjqkyva.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ktdidxcz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ikhijtiu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3adeybvlp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kqqxskbs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lrhzbcby.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3izwbtxif.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hyhhawad.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovkagumc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3aqplapky.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gsdegcdr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3oyazfypn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uhcmrjgj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3miegyffd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3kghyiehd.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oequmgfu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehjlggsg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3cubswxcf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rmxhnkgr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgielipb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3llodzqur.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vkrjpska.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pdfxkjcb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3grtbmpaf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fhhcfcld.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqxolrsq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgxcyzed.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wylqjzxd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kmpdgond.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3oykbkhah.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qwjfglun.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mtwospuh.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uokkgmii.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qprdpudl.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3pnuetoes.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xtwdeqik.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ezsnrqqt.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xhhbzczo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rvtkykwk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dmbepsyb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3vhwlbdpl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kdvyxvjp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ljwsehkf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3nunefgff.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3iwdszuyr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gmuhcjyy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3govvcnpj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3lbxvvxzj.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hboxgeqe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ayeqnuxj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zazhzhkg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hinrgwry.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3ruywpaum.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3iopcwvpu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3awtcgoce.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3udfrtsxk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3fjinwooy.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3svdujggv.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ayymdlnz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3znhoetqo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjgmdhl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tctbqlko.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vomsaixq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3uhnlgiif.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3pfdsswuu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ajmhhvqz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tqdkewye.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3dwtjmegb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hwyzjztr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ancizoly.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vqbkxmll.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhuyhhu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3plmnahvv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3watobfit.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fiysxurm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ykubwjom.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ybdenqed.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ceygwzpk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vzujmzxh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3birzoajf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xlptgwdf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3iuciaaze.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ynwazlhj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jwretjeb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3dbburtfl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nozfhgfl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3hmajsimh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3utbcgthi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wkiajntl.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ftksjksy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3nhwvbwga.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gephmknu.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ewkdyffw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3uibsaokp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3arvgkmfl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3zepsiskw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ifdrnwey.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpeitrny.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dwgkglel.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3udrybhhz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3jwfoaaeh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3veaodwrv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3eetzmvgr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ngckvusv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pksytdxi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3xznjwgou.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3nvhmaynq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3mycczdbs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3wggikdbv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lfqinhvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfrjrjkn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3pifjthci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlvkeuea.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zxhtljfo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3shcjjzzs.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkqytxyz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zfkolskn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ocllrpsv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kyfonoxp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ztfhokzh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3yrssoimo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kxoqnfpo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3onavkcta.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wsdvjdal.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iacinkzi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gsyrdxqq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hyhuhsvo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3yktigfam.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3glmoozmg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zfriejrz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zfjqgnzm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3atgnzwyh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3bsljemut.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qpybbgyh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ftrlgvxd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xcshaofd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhwnviny.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3dzhhrcvi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ojcdaznz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3xwbhtrzp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nkehuaue.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ekzuhgej.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ykvyzxrh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sewziexh.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3djvjxpcp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qhpbcamq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3zgdydxff.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hhkejntm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3waelqvsb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ykptrdym.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3znewddqv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxknkpdn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkvrxdji.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lhvxjvyj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzjdqgiu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vcojixja.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mpyoqhwa.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3tgvfucip.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jysdaumq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qhwhajcc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3lbjwvtdr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qzbvunlp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3zoffgsxr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3iipxrncy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rxrjlfai.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3uigwhocx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsdzowcu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vuzimclh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mgmifgfd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3fwmwgshh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sltjsvus.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kuixoiof.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldygzmpa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vejjtuys.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yightdve.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3sqbqiegs.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3sbeotryx.html


<!-- 参考信息 -->