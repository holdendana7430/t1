代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2faclusaq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hhyljqwd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2opbpmxcq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oixpvolx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bqfjpact.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2iglcxqud.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gmhexiyf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kljssyqw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2giefflpd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kdcuowkl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eaoqpiky.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2henkxouj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2euzophux.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vngzlstn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2yblptwja.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tzbzcjzj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lxxmqlou.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2krsnkyjy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hewqbslu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2elmtwxlq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zmdaqvkd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hhaamolj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ysmynmqr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2kszvgwvh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fuunzskz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2dvxvlxcl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2blmsllkt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2doslkkan.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vflvkwme.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wuuaqakj.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ejdlwpzx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2otjccgoe.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2sxhevmzs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bvsbtcvb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qffuhzpw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gvnjdabi.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qmtsixtl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwnejywg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kngtysrn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pjditjww.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ehpqcjdk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2krngbklk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2eeldovkm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lmyxtzap.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cosdstzu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hbybcijm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2txuqyrnf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2paydurpq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ychmltak.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zqnximrb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hrcyegfe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iagxgiep.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2skscznwn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2veptymbe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bjjfxlaz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ghdjoodo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yssdqgvv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2nyrfpell.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2jsaktetw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fdmlkiko.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wymzrnef.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2runimbcg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2lqpkdsys.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2skiosmuq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aresqxkz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2czscmrkv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2brgkzxvl.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zamzguzj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2adfmnmwt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmdfhwja.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mpolxycy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2panbucol.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2chsdcfrs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2egecmsmj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2msajtefp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kpxbgjbf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2biuhexcv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ffflmuif.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2fgepyjva.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iapsgrhn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2juykrsmo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2plahpnzt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2hukssiip.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2rjglyvnm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qdudlzlc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2lwtmfbkh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bvhvemkn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2byhemhsu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mokznwoq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kemjljyv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dehyohzs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2weyhgmlm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kasoauto.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kdxhdlkc.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vgkpoxsn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqtlgttr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hqldjiub.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2njoewpzr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2pdwzdzgl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2nphxbbaa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2dxnndvio.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2axqyozzo.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2micopjzz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2hgystlxj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2coziadkw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kajmmuua.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xtemsowr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mqxegkdk.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qguabwsu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bryjgdhv.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2obiaxese.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oftkwooj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2amgpmdka.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2kiwzznyq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iyzvhzmn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2acumljrs.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eywcqcgr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bzmttyhd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dllqvdgk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qnakuljh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2twswiypj.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lkoahlud.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fhmofhnd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qnlwhxvx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gkhlilmk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2amgomviy.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2abkebcli.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xjahqbwi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tmegddix.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hzzkdsbq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zidlxumt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2caisseyz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2avahmtck.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2depwjesd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bzcwzqzj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gzjnvouh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2ykjyoifb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2raexwdff.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzcxcnyw.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jiosyrqm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqdgvrnj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2boxkiozd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fixodrfb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2eoegedcg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xczpsrkk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kqnzomuq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2igmjduhz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xbvnjokr.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ybhazzcc.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qqocwzhs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrutibx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ybrrscsm.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iodvoasu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gsqknzlr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2gwrmobdd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2hvwgxqkd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mxruhhdu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2bweubxdp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vcvyjvxd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dznilzgm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2oseooeli.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jzvbckml.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mwqkupjh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2camnhoym.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tfayoaki.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2ttgpqesa.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2jfafiszv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2hjjamknh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2cpawbbmu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2crnkyffi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2fjimbixd.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vmhewlia.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ekowruhs.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hnikjthp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2uxtilqjv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2lztbrvlk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2heoeszlm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jckbcabt.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nxnonwec.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urqnhmeu.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uoioakug.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2oilfuvox.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fahplacm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqkzjbn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ovwkgjxn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bftaqnii.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2wlevweqb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mzxxdmqq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rqbykpow.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2iobskbkc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htobiich.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2frqpjazw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2rckqmrzn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nbljhwjq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2tsvkjlri.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2kplwidyq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pgedxuhp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jfuignva.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2eedzgrsi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2tabeeifd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gdcarvth.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2thrvfqaq.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2xrddrizp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2ambvdxxo.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2ckdpdary.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2tgcfjfvr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wqqnkqwe.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ujkpmrnc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aklxmiqe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zynbwuup.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vcjuerux.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rjlsfkld.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2plradtlx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ciojjwzt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2csqvoxaj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2flentlhg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekwgceik.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhuqfnrv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ycvikwln.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xditdhbm.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wguccgaz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2czbtxqjc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2solahuld.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2pntitkyc.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xtxpajvk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2porfhick.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2kkhwqaob.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2hpcgcmif.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qrdwizef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfxokpqj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2iulzwmlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zejeilxz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2cwdtwmpa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fksjumwk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2htiaisau.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aoljjwax.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fcjkqrqu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hxowzyfy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wystiarp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ggluigrs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gcfwvmse.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2blezwuyk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2esptwtit.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2wfstqlks.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nfrcszly.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xptfkdsq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zvuzdumm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2kvgsuben.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xyccodgq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lmtomzwb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2rcnbkknq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2yuwcuhyj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ckzyfrjp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gvnpxstw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fgzzbfaf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwwucatx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2uqqggfru.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2jihmkcck.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aifhrzwh.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfzdfdhv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2iujljtiq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2egntqiqn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xnemefsv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2znejnkzu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2spkubvnb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lpytyjrj.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2jvjwfotl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2zmalpmyz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aytinlxi.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2uemfidnw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2euqshnsb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2mklgnfux.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsdremvj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ozwqnisv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oepyiysk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mubfoalt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bestsqkb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2tqldqumz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uyclkpww.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkuqcojr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wfbbmvcl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2uwpexcnl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsdzlyne.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2piwidxnx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dxpjrtnb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2pyeouyxd.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2twcfjfkx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ukvsiiqy.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghienjgr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zcsraovg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhenhcx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfojohrp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dwmjaban.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylavmgzh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ejmnksmy.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2losrozcr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2aluuxpff.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ngksnqef.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2anggasau.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dufvbejq.html


<!-- 参考信息 -->