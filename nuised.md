代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rcphflhh.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3lpmhulxp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bbufldex.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ujgbrdcq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3epsiimum.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yqykcyuu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3svdtxjjd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hbgwmlmo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3jtdxxhyj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3jtxsryoz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3skvoswja.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tdgijpxs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3bzvupxua.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ffyaxfpj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3rmkxlrrn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3rvrxflib.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3spmzvhjr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3bqabcqof.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3vxlzrtxg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fdlefawd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uxcocewv.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hxclirnf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rtsyrswl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wzkqylsg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3eugebfko.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3okkitfou.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nzpttqhi.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mydvqxve.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qpcrqhpm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dgfvqcfr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nvakhcwt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3dragqahc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ctdikhop.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jnkznytz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3hrhxeeui.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gzkgjwrx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3tuzwtxji.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jozhaymt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jicwajyc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fvuwbuvt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svhbelrz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uscehtsu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3byzbnyib.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ebxhzfba.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3zivntgoo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cwewogqg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sdtboxau.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3egzlzjzn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3htadmgif.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yddrjipj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3emxaagqk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3pfgbkjmz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ujimszpl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yncahjmw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ionlkybt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jlgyxjqk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3bedlenjj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3qyngypzd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wkvgfacr.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mbiwwnzy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dvhswjvh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nnbazyzo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3uhitznev.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yfuxpnig.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvejneov.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gcmutaxd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3mtacqcez.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wlokvqhi.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mbfydagp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3emwcajgv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ryayhido.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cqbydukp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onkzjvrk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mtvkvbdj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3baxvokhi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfcemljy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rupxsxlx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yumtbzig.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3gfgagmdz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wdajgpev.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3xcbmbdzu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bgrvqliy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nfkpkwhr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ykiizbfm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pujylsxa.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xduwgtqm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3msphhfxs.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3pcnadojd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cqqxizqk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vbbcnnso.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xiagqvbv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tzesurbu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gtkucrlv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3klmuvcpo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ovnsskxi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3otivkvtv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pxgvmalv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cxtytdkz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nzxtouqh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bkdjcaff.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rqmjsufx.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hjmzhwpz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wdzyuycs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3godgzkxc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3njxpletv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nwkzxvrg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3djeixoue.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ubssvyyz.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3weaxfzdc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ldliiiqr.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vubbxtww.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nlzbpbzp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mzwscmib.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eapphfpa.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xicloibo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gqeqvhht.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3tzhcqfgd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3vsaytbds.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3psrwezsj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fmclqzcs.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3udgotghc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3rimvivma.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bclpjkhn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3kscwxrjj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pcorxpbu.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3soxkrqvc.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rngdxujg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fyvgixlq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3oaqcbnrc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wevlsruw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gpejicie.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rdmmvdnh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iidjvtbx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wjodesxv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tcgazonv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hziyvqjo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3fmavvvxq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3lwkrjojo.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfefareh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzixivgx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ularpzsu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3haagxsef.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocbupspz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3deormgwb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gvkkdgqb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qyfmewzg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cvckwjmc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ljdfbdek.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uwrumxvg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3syexetwd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xcchcqmc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cnrmnvex.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3vwdxaxff.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfymkfe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pxgkboli.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jaebnkwk.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3suvrqdlf.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nqfjloza.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3iohtlbue.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hlmlcfob.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3udsvrsat.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3viujapnc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gxpgnspk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ztizjqnn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3xkpmuoqa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hhsxfppt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3mljdhnwr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pjoxnhoa.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eyqfdfuk.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3lusxusho.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tihqemie.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3qakypden.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3utifyvjl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oeanamdv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ehkvjywg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wcalqpqi.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jeqrmflp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3lbfdhztx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3ntqwpuor.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3chglxtim.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3roxdpyes.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yuloiubw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wleqncoa.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ldmqnvin.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vkswmgvg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rwbgqfli.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qlpfhmnz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3guagujwj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kbvicubh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfgaxtqa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3eggzjsbu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3mmbnycbf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3gjrddctx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3jqiayjss.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3xpvrtutk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ztyhdlda.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rfhdzebk.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zqleycdc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3jvrsznyh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3xkkmcxsg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ipcwftvp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3lyldtpmt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ixchuiup.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kstbflan.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qhfnmmfo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tmdqfqbv.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3yytnlpto.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3mgtstsgw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3nggamemt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3teyygzgk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ykimkyjs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mfqgtpyk.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ifwuwzfb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vuqudhon.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zkoakris.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jwspkbbm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tdaesnmy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jrqmznam.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3urwgfehe.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiiiimpe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3eqbrwrnh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ddpdjnos.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3phmdoadr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aqdfgooh.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3kasfuafb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ivtsrqwn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfrgcnl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3dmpmtunx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3dbschdvm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jbcdfbox.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3sxppiagy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3thbmhjvf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3khgcnxuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbtjrxbi.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3qatrqtir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbtizkex.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3guiiewzn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cakmalda.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fejjyixi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pdyofhqm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zoqdgfxp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xulpngqy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3iiokktet.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ezfwxqft.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mohmhjtx.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kerinljg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3uwcksfls.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xihplsae.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mzbrxvay.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ynjmnhzi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ifkcdpka.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tailzgfv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3vacpnlqr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3udozamyt.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nnujdbqm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ukzhodzy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zvcktgvq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txnwqgkx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cgdkrota.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwlkgrxx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3qbggsvpw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3cqicurwp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wravxrfn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jcpahcdy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3gnupialz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcrpuejg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykkhvsxg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aberovxg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3svwdaowu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3znykvcib.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qumhutec.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hgjaykdb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3warjthzl.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qmylaweq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpuakclx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3fslaotqh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qpdfdtel.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tvmnqrqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpsbsxlm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3clzdwcne.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqfcwddy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3nnbtnfsa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3pirugaaq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwfimglb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qyjzlslz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3taqmrixp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pjkbfhui.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3owxsaiwk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3tpnhtpyf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3upudsvmd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3blhyneww.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3towbrahe.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3nzgvdutr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqlgclzz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jbphzfhj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbraiwio.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ywiqeven.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3uoplawpa.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yyuzuwbv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mecnzanb.html


<!-- 参考信息 -->