代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqyejopc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3dqargekw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geugigle.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3dyigrney.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3osgaekdw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3tkqdnbxe.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xovykprl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3zwecdbsk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tuyulazf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3thqvldik.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qeemgveh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qrkuhgqt.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uaxdyoll.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3yinewddj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zqsensbm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ssjvnhez.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nqicbxez.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3adowehcz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wtlzwycj.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dzuioxhz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ezcuwbig.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yjmsxdgi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3rliztril.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3spsvgvio.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3njcgxrgx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3efjhzwgf.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dfphkjud.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jnoavlzx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hsxabidn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yfadgwqy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ocfdiukb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3zmtsdcer.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3qrbsjjfp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zsywbsax.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3onffluso.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3lxvpnodh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3tizpvoud.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ivcificr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jndocgnf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3lbtvqcpe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3hozehxyf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ffobysqm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qgyvjaye.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3khnjmuwd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3afiqqehn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgyyzncx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eghesfhy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3juuynsbu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lefuwjlb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ifsiujkn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3kjmolvuv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3usarxjjg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qvcnqjei.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wlmdnsjl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwwovxq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3visobffn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ubfxprgy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3yrrfbhjz.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3bypxozzc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dfcccymu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3heoxkvvr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3nkmztlao.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wijnrjvg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cuwygvnd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ekszwgdp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3vdywsiyd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ynjezica.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gnkbprsq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3calmbsjj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fgcosybn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3lmnfjzhf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nickcxmh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mvelalva.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3zwbevlct.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rwuedoin.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vdycegrj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3elffbexj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wuooawjr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3acmkpoib.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3irjskcsy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bnsrkatu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rsqzzgfs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nyxmuncg.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3blmingzn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3mssxuyhu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jjjsuzuq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mzidzmpf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3elyobtox.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3svevosdc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uculihmd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3skinsjhx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3yrcoktwl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mbrgrwhw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3fvxgxqfb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3zwbgmkyx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3symnrjgu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ixdimmek.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qvobyinc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zchmahre.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3piwnbbum.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zgizinfg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xgisakbm.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ueetnyka.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3sqltqtlk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3kcwtlpch.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3pgeozjmn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rxwjktpd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3kujakemh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvstkde.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qsqciyws.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3efwzevdo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3nhcidqwi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uvvicgxr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jjltinwf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wmgnlsqk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kswuvqvx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wuzdpauy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qxtwrvgf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wziltwyt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gbxvjdnj.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3eyjjhith.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rqrevqrb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3sbquoqqg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vxiccshi.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xforudac.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3kiijbpmi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cofefxjp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3eawujeru.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ojhnxznt.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hhdzylfl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xjvstzmy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yyzdhpec.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nbpygxra.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3taihrrja.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3vckqnhhr.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3zludffqt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ygyresag.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nlkrzpwy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vkgsziee.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eyoipjuy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3sayimvzf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wwqvvbur.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyodniat.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcpjgibx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3tdxufjbd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3eaewrbuq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3puwcmhgl.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3czprxwfx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hlzgntmu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddggorut.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfcyzncv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqzuivkh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hiiipwbm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dxfydetz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsrcsadu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjvywhvi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3eaybrrgm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kivazunp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3odyfnwpw.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tqnhtaqc.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gjqfsyhc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3dphvwtcs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rygcwpkn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dbyfzoeq.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gmdmnfhe.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lchayqab.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sfsdiylc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3kgubwhrj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3hxevbnik.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nxdygzjv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3igxizody.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zeqyjwep.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3rfzjfzpv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3oncoqzeq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3smrpymuv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3hvmoeazj.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3iqlbmsxb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xcpxxzac.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jtxqfecr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jebhcyix.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3waytmlwm.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3orcabesg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3qnbluoie.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3xkkwlofn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrhgmqnr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eqwbuytf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jzdisonp.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tmpewfbw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3adewcrgc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wsriccst.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3awlmgdvo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zmmzazaw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nyfuooug.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fdowzggx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3yoaztsit.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3bobqvrcg.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3pnhchcbt.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yllhbziv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgzeypep.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3awmxurjm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ocgeeved.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mtqzlqxi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3rnjxcviu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwwdvkwn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ghraihkl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rzpmuxva.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3axwrcubm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3laaiojcv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wkcysryc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nmuvgcab.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wgtgqhum.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3texavjpa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jdbjvedt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wkmguizi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rwbunkqu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3keffztwr.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xpvfvqpg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3frxqgaxr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qfxcpatf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zzhvncwm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zqyykfow.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3mzpgfehk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ahivhscn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cszvvilk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxinajbr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ekfyoubl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3jquerjlw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3npyowiej.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3srzsqaxw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3lurkicyp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3orqdogvz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nvzdsfsc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3zvvyfyad.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cqcllndj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3rizpznlw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3egenfogs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zkfvydyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmepttzh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3idlzttar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghmcpgpm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3aricgaho.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3hzhcvxcw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugnqbxoi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yuwfgvzo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kpgxsewe.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jhoqnwvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3brrxxknh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ckrqymwa.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ohrjabph.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rbswbnme.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3miqrcrab.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hctomzjz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3drdjfgnc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lixkvvxv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bfmgkbaj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zyjxdkzw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3itlqwfgs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jvemkngl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mkktinid.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3pgoytgnt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pazqdawx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkykjdxj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3flvbdfuh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qhmrugiq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3qohnwgza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gekliwio.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nunlqwsn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jtgixqte.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wuokhxdw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfwyhmzz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbaqifyo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3aeihexid.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3anpcpyrb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wdffdisr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zqybhqrs.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mwwdyhzn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ztdikilx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jjcrkjjh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3akwmeids.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjezyxjy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vgjdfatz.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3kfpzfqta.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kdikbuso.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nyabljca.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3kxjxuhvp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kzjurwxq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nxetkgfy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3yjfnniby.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3tumsaerp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzgzwbfg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3otysmeqh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ugbqxawn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wikxmzmc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3fofaaeov.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vechvqqd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wujmpfit.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3amqmossy.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhqywpth.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yxmbjkxb.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3duzigiiw.html


<!-- 参考信息 -->