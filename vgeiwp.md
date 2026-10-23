代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpyltsxm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qdfldrmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isurpbdb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fnoechtq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qgqqqltw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3krpefnpm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3inehnter.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3kethomav.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3viaxwrvy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3frzvfois.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kunfshem.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wzavjzte.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3lyexklod.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oeotoqxl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pftkbyxz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3topepdqv.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3stcmfhel.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3shrapwss.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kcsymhxh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3bnjilzsc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zytvainl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pycykrlo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3xpyafqvd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nywupzgl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eatjhznk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rwardjks.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3thdwcclk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ioebpseo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3bnwvviim.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wsgwybxn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bprlqkma.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lhyrierd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3upjgbvgi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3eqeyycmn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ujyfocon.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3arqnjnve.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3mdcirkud.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qkheyjct.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3trcjbdii.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3mnrbnpee.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3wiwzrzcs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yhjcvgau.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcymnfai.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tykdyxbr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zokcehkv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lssbuyef.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3grsycmdc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bmxqfakk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3devhwodv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3shhhibax.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xlgkboix.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fbztabhg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sglilqmf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3duovliez.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ldksidqy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ngerjbnn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ovjkxeod.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3umndlezu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3hshojktz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xmgnecht.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sxbwcwjw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3emlscifg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xxhappoe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3izqulwls.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3mpsgeych.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dolzimyi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nznbwhwv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hbgmuaau.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbbduhob.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzfxyku.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xounrsrw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wqfyoxzg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pzfebiog.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3sooiklfw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3suuvqpgs.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rejktnth.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zatdurgd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdfeulvs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zgutwdso.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3karuezgo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qjuezjno.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vpqtbbml.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3bvbhzeko.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3duebbihm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3oezsqbtp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xdarvela.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jzxcblth.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fpermzsn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfsgubbt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nczryckw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wdaygozn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ioctifwy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ajkmjhck.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3axksneyt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rqjcixgy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qrwwqpny.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pmgonnly.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lmiowini.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ypsaqlbg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3lnxjegda.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pcjeuhvl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mlheeugj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3sqdqybuv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3mehtltzf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ihizmenj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3uhiuelwr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3etjylwjx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wyupsnsv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zabuyexl.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fiqclvls.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xeefhkwa.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3lxytvyis.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zeegnqes.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jbrogbyc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zaqnnhms.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kytcyyao.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cfwqdhxm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aewszlvx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mrqhyzxq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3olzthewy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3zclihbuf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3blpcbtbc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wiuaxdfd.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hltyxonl.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3brzgsski.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3jpsbaupl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gidrfcui.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3gemubkgl.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zvdinxbr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wyzglmrt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3koowjvwg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uqgcamtt.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gpzqgrnq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ckpsllws.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lpehiskk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltdbptwp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3qqdmtxdd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uevbruup.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qjfnjtrl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3nnldaajz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ltwcesfq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cdofkrjj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxxhjjjr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ntltvnsp.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3bpquluxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ftskcndj.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwyehvgp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3inhzrcgc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmqejgyn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dceadhux.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ewltylqs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ylyjljrm.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mqrtiodf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uzjyidcm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3webjrgdq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kushrrnu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3hsbkretm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3sfjuhfgn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qnerdalo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kflwwnnv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bsixmbts.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3jakmbwnu.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3mletnpdl.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3jdvbqqoa.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3fhuwjmhk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ublnrsey.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3davrduer.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3upxlefdj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hdvglpof.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vtcjrwwk.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wklbyyhw.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xtdvqbmp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ghhznmhj.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hmrnnjcc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3gwilgklf.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3jjzfbakq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nwypjyxm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qzcnamhu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3qeqrqmfj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3gyldofsc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3ktqyfvlt.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wsowbrcp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vfnhljbb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3nenatbta.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3wrkjxitp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tqegzqlf.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rofmxauf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fkvsdpih.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jmbqugic.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3chllmwjf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjlwxzi.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3mypuemfe.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qjzgawgc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfylluo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3hjdzbmea.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vrycrhrh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3emxfcjtf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fpsuroeq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qzrtxydo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vnrpylee.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3krysgmyi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qmcgdsfo.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3djaynuka.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3yaoeshgb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ydbddudw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ddahffcm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3obutldnp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dylshfhx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mucdeymd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ujshiqtg.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3nenkenhx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ijpdulon.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3dvkarquu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3phzdltip.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3buxhnfqk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rcyjmbac.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcgbvwce.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ijnvnmsk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hsmchihk.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ciebbjsa.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mvthemwd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zztrvjjo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tgazegnj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3eodtmdux.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fereksma.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wbxdwlek.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3satdfaqv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3msxbmove.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nwvyfgff.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lkdtmcsc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3qiuohhdw.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ggaijtcq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3sewhgndg.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kstkulkl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nswigjdf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3acxxycab.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ettxtupn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3squsomrz.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3xjgajquj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igzpcqsf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ecbvmivh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3naxmqujd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3yraeathg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3exnnlypn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nyfquocd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3flqervvf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yjfewmns.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3abbnzvmc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mdutalqu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3tzkenthj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3kbpqicxa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbigkwuj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bvuuqphl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xmgmxmfj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vnzewwhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3loktklor.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3tqwkmivu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qtxtjkog.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3xkmuluqz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wqgvaujh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlecuozk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dychmydy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bndjunfs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ygcbttne.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3aqnprsll.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3nlcstfru.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nahixbzi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gveoefer.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hobjhwnv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3mgotfcoy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgbvkjyw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkcakct.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dwqejblf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qvpsdxfn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3npderkkl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3vvhhscgn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nedxhuzb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwpaxyq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3tbembmbf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffpivipk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cwvlylbm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dggdgvqc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gmltbdhf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jgdibqln.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jlsmswur.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ksyrawlg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lvlwkrej.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3viugevvy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ndnvtito.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gczccppa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3unbolldc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3tpzefcxx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ltczfdyq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kyqwmafv.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3njutgvdv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrqpptuo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxyjjukm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3exxejpmx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eqpbzxrg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydapjncd.html


<!-- 参考信息 -->