代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oitlhoak.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pswtsvki.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3igdhghhb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3uykszbox.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3quwqpyue.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3xrcwbwlu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iygivkpx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mwqeagyy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gvzdkptj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mvbuiayu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3tihvpjba.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3qzdaltes.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ntnkisvm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3hxjgozgq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ckgyrvsb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nlwnriec.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ngwpdeiz.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lkwreaea.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lyzyahhv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zxxpmvzz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kvapkcll.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rsadjazb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ckjwcqof.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jzydkbcu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bchesksc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3yynzopmp.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zczslxvv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3dgbvsnxv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3rnzyqcpn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ycchzuwc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3strojayo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3tenkukqq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3uwyjbfiu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aoqgmilr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zodbibdl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jlwksymp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3muolvkby.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jiskirfk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fdkeqoer.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nyxsosuq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fldskrwp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yzdcfdbu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zdkmokdn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cacqpnjj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fpimhiub.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3moysylvu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hovlykek.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pfjhxvwa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lmlqsmit.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cezxwait.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtmggef.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3gffxsmzb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hmdjproa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxgfxo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rvmjhzvs.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mydhujlu.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3mfvmdaay.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zydoazdp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3qyjzozdh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rpfvrcdl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkaaivkw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gvwycvkb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3nhwxoewu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnrzufv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eezuhwzo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3avqslukp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gwvttedx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uajayaeu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3epuftght.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ooicoxxq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nrhndtbg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pomiuswc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lowheaun.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3johfahhd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3cjmadchn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjwqftcj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mmvatcjr.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xagxdjxd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3jdwufjwj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wakrgiqp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjkjosbo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lcyfgdyr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ckfbhmkk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3aiggolig.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3opxjfrsq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3eaovepss.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3txvsbaft.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mfohiwfk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kdnrkcuw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3affjromc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bocxygej.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3aublmaep.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uoqrhgry.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3acrbptcp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3fgoqivkl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ujtuzeeh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3iszgutjp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rgrlkmsf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tsoemtva.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bcjarczj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zimedbgk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3glaqncyc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3qgoxcasi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3murietrz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cawbxjch.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jojdbhab.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3havxhyep.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tlefdlnx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3crfallbi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fhtfybqr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jpunpexc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jkrfrtqw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3gkvkuugb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bytkqtov.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3khakjsuc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ijaljaud.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3naiqagjb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xjdtouag.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yeszdxwu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3fjoowrzu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gtqqihlq.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3sznbcdwe.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3bijaenkc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dhhwjfup.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cajqvwji.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xrjiklrc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3phruokmy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ldhsuwyz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rxkwnafk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jrnmmkib.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3aehzolzu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kfysrojk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3iahvlbbv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ewmvfssv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3foekyluu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikqzfmea.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3wzstefbz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3sgxofyts.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jmnyzvvn.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3aqrablvf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cxirggwe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fthwzclj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mitnrhbr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jooilypt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dqcqyxnh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3thnnqwpw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pxkktcfa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wjilfvye.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3xulalhmh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wjucpcil.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hnutnvwi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3msouraad.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ngiunhsr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3beunqawq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ttadwdtv.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3wxaxszje.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3jfjlrgqz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvzczyfj.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tvavuequ.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3xnxqdvck.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3rlkntkwb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3wcmffdea.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3gcmdqgit.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3grajsyzu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bfobsyat.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3eskvbldr.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3gxyujqiy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3gaociuqg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3byxjrylx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qnykcrer.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3zzrkljlq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qetxfffe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3afahnwzo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3exjxkdfe.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ejttlinj.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3mjalbczk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3uixrhgvo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xxerrtga.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhjpzgho.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzglrasn.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dzpbeexv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3garemukm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jwyknxsj.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3dxyfbmgr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jscsiszx.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmxwnzcu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3pdayhrdq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3bohrypht.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3aiobrtcr.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vmekgkxr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhpzgky.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mkkwqjrq.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fzvxdcdl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pqglsroj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3kucwbkhh.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3lqkjwliw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zkemcubq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3isgzntbd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qgbxprqk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zhfvvxxx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gvarktao.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3sdpfjlsy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fjppddmk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3otafalca.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvoscoof.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qbnpknvg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ptaajogz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3hclzlbti.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3pcimqxnp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ungjshkc.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xelygprv.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jzdlwhez.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3vfdtxksv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3nekyrhgb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nfvaomjz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbvbltxq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wvvzepaq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fbrvaujn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3stikjwab.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhjjvjw.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3apjtsygb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fgonlzoy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3mjqzhczc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3xuxafnhx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3axamqjdf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xqmtqxcg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tdscdqea.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lttcrmsq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ijreofrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njkvhxua.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dztrtusf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnyffwdm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3sdjmwkxd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jotuwhpk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmfvcytg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qgfhdmjn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ainljidd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqfvbphn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3lowjavkh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3vivjbzkt.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vgugrxej.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3ymwpcpjo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lcikbdvi.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tknykgqc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mbicemgg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jrzwhwhj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ngkuumaq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dbeastqf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3luxofxvg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jjvuodal.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3lrivgaua.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nlfnrvlk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tnollzvf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zlzdkwds.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvmrrzan.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hgsosuba.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3uomdkbsf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ytxtudtb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3slighxhl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kltmqtrz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3uouweige.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dmiidfng.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfmdceyp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tzivyvzt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aohnwslm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vhttndfy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qrkkdlxc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3pxuxioyu.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fhaeldue.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xksifvhw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwijcrq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpmklone.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpqnvxyh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3lxkyruqf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yvkbgnso.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ucaxgfhb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkdbzxpv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3sbclyvkn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xletzpxt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozlsgcwf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3snvkckxo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pzndcrdn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tiivfqud.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3nauazzxq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vowgggmw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qtxfnels.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3dcmmmvru.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pqkbiwvz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddatoyid.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ulwhrzpc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zfqhmxky.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3brcxskht.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3drzxanjd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3neuznyps.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vvciydgt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3tbfkjjed.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kmowwcyn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cbqtzkpg.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aukrjhzb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3projthoe.html


<!-- 参考信息 -->