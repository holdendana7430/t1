代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vrfllydc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wostfzla.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3sxawcnbx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3txfnxzgu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3cgwcgsfx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3kizgvmqj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iowohabz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hzvtjlmu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tbwiqvaa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fjzfnunm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3dbtjbdxy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dijchlsc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kirmofrd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3zwbfepdp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3wwzizget.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vuabzcpq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ijlacpcg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3najsgley.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cinkkkuy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rkawlfns.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3urnvrvgj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ygqtmkxk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dxczeykw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vogtjbyd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqjhchsf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3auklwnff.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jdwixwkb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3krccrmba.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3cyxwsvfb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3urgyahhu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3hfjavdjy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3zuiwrsew.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3mabjlycx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xhspordm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zwiqktkb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jjlqseaa.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dwcmzuce.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lzbzgilx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3anjewpbc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dtiuzzjs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3jqiezyoi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kbrkdeef.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3jleigohq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cwwgvdcw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lvlwtehb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3beweefdc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3bwzhknyi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zugrnzmw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hvbtejnz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpmyaqxy.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3phmpyrmy.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3gtqlfzql.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sqdmjkzn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kzojongm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3cxwdxrqu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hdqxbffr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3veppgmef.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3znvnytkg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3lobtyrya.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pqudpixb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3szadqqbu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nfbhrwad.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3nvjrapws.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3paiashnj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uxzgsfvy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3qezqevmt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lswhpvdp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eskprxff.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgtpaga.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gxnlrkat.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nzvohwwr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ujmlcaud.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pcsjhpcz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3xanykocz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3gzwulibq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bglnlkfs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3neysvaob.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3aiwdrbkw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yufyvojq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ugwtqahz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qugikjav.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ejctxvop.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qajlonhx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3wrheapgm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3klonpkjm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3qgsphjep.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3klhtiocj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ufrjzrac.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3onejmmsy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dpksqito.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rrkcznfq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3cmxnnddc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iykthorb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mfuaizng.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3estjoblh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3smpmwsty.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzceubi.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ikbcqinn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fcfhoaug.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3cxwvrezs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3utofqfvc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3sbpvjeyw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mzqsnfvl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3rsqpjcer.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ocfxgnjx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qsthhkzu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ovgqhurf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mppvxxmb.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uxfexvqs.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zymgmfct.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3byrnbkry.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fscfddkx.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3myhervib.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3cazjfmgq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ilkkdpdy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3glikqeun.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gawjteex.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3agxsrzoy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sskowpca.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3kocmzgsx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xrlvmbhl.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pcvchxkp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nwowaksl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ajinkozu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gsehxqzn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gteldlhq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3polpijca.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3tmgkinfp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fxqinlys.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3baifgoty.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wbiewhoj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3nvsbmwzf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3umvlzlbr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3yokplutn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxtxdhcx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3stgtdaup.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rdvhetyp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3hznprgdq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jlmqthjf.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nwuthdbh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oklioiqk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nfimtqsq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbghrojc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xvmeotpu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3anasiwdg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tdugyaly.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zlgnnghv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rvioosjy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jsnhaumj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3pzessneb.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3qzrrvscx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zngozaut.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kmfjkuwm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3fmpasamw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3demexbfn.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3kwbflsbz.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3qtulgmvt.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jvakxiwu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3blekmgdc.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tzojdonh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3feahhoxs.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ylnthwjq.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kyrdfjhk.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3slzjsixi.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3chqpcszw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3klmuysee.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3fhyfhyev.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3biiaoxqn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3kqbobppf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hazhxyac.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ndjqzptg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fgxdvjqt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwvxsvu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3vgtcvlxw.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3zdxivloy.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3nioukrgy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jojiyrlw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3aiurjltr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmisjoej.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekovfpky.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wruwqeej.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3icggylsm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3oyglqurb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ctzjdlva.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gydhhret.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auhjvujv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jkqsesxu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3uilocner.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3cdndwvbd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ozgguzrl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3grrdxgsh.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3etcwyzve.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3iexhxqvg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3duxvkjdz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mfgvvcqf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3zsljezwo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ssnwmzsp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wxpsugds.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vtwiaota.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3ffhcojby.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kivvzbsp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3fqgfbjuy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jamwpliu.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xazdujtm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvtxjkp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uflalzem.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vmsfbucz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3axxelsyq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fvtpvhxf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3abiyrjaf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ijjwqblh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eahuzqjo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ktmhnrsm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgreyunk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zasgpxch.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfpdccz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ldujmsbi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbhqvdr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dfchexlu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vanzstxi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fiqcwybu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3qggxychs.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3obycrftt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3isbfyqbt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3sbemygjf.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3whmnqtvw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ilmgegsw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3uajrgbfh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3konhyned.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmfhufih.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3appeupoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmakpugb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3olqylaee.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vgfyabri.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnwksjoj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wprdjrcp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ffhpknck.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ljokjxqc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3hexxbhql.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3mtgiwaqi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oznqdczm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hgpktjes.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3wrjmfpkh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfsmxwia.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rupttgww.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ekfaxcto.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uvoxynkf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nmpnrsuy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ealryojg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zozerlxc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vvlzrioj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3xxgpvyui.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckvdorqq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kbdzfntm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iulnfkzg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypwlxwph.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3bipaavri.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gituhwsr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3eqvuayjx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3kordqmbq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lxoppoyr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3eebyfqal.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzwdyypt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tpibekzu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3qpmjteey.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3pjkvrhkf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3egbvjkpz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpxkgyxl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3skgeqibr.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3zkfwmbjl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvnfjybh.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uskgpdkh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vuoulobw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3reunqbhl.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zohdbzqb.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jmotxhwv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkwjttsv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fdqidhzk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3cztwikuq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuzfidqx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfcjudsf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jspdszis.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3prarrblk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pbakexzu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3scqkebrx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uncernwf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3rsshflbr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3gpnzwswv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3afauryls.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzsksqkz.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3razulyhh.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tymzmvbb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3bhbaukqk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3czhvthrx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bebjsnua.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lyhxocif.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ootczunm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rdqbwcnq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kmlwueyt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ltxjeqoe.html


<!-- 参考信息 -->