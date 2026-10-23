代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnnnruhp.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3eixdldkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjeibleq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bhjmultc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wdhdfycg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tcprdxsy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zydjuctu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ivabcjuy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rfnxipga.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3edptffdf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rorzmxln.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3srlwiudq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3tehckpuv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ehgsnocv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jbyxwocj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qavxgfoc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3shidywyl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kwemerut.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jkojlrku.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vdrjinhr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ygkxlcaz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pvzoojfa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hkxokjgt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3husmathi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3amglmbbu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zvowuyru.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3buxzwpab.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qataapju.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3kgsbostk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gkqitnrp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pstipahj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mfhpfjln.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wpngrkmt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3hpdjtpfp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vhqgpjun.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3zjlpdqxj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3olurkrtu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3poyhjide.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dqywzxvt.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nxnvnkjn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3cmpzvzin.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tazbmoar.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfnstydj.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hftlmtzd.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3blsgwolc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rghdilzv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkdnlgwh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3itdeaweb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rdjiydja.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3edtuencm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3rwtteccx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tajvipmu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3iuvrpumo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3euozcpjf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3tpfddztm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3kogcjlqy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3helabtnf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dvbjwmxm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsahxlx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3enqektfu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3zmwijxzd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3krppwxih.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zrvnffld.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nzavwllz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3zkaywarw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3tpidvwrm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3antkygfk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rhaugefb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfqhlcr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bltckenf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ewfcqtlm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gcsxbqtj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3idacsiof.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vtcvtdwx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dwlammsu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vtfwektc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ifeeeewu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuiuqqfd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwpidiaw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3thgkvjvq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zvzspzze.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3almuktxu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qrdahatv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gcfbrllj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3nvihtsed.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3biqwejzm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3zdvgwlnh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ayqwnxhu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mxxomkcm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fyxydgey.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3cyiozjyi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vvlrzzni.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3rfnduqkx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3enycilxm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fwsfolfr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3juqsjnvx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xtghyglh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bemuslzf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3snaoixkv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3tmbyyhcd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xgapegoh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vllfimpn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3aphtwpia.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3aodbsqsx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3eyxlvhsh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tiowtevy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iyrghakn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3dlvngzaf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzesczt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3txgmxssk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3qlfsxaiw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3gqsgnlsu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ukpnlgbx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hlfaqpow.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wjmdzhap.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sjjezcij.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zwbvgolt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sceaebvw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mmyfktlr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ustosrbh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jrmiseoz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ujccbeew.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xwgvqnfi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jijommto.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nkszgotu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qgihrqeu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lbqbzrsj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vlxxuupe.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tfqlgylc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ojmsqpov.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uwoscgek.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mogcxsii.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cdmhrtuo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gprsxfrf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3mzjcrtnv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3njxbhodx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lokzqgjt.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eqhnnkgr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dwzbkdbs.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3khhbbjtl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3spjodijy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gihxswkq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paomfpuo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ctdurgcz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3lppjbllw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3fftnqnhg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3seehftiu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ejfayblq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uglnclid.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sugjqdjk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bwmdygzt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rorhpiet.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xziftuqo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bueyycnn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cyybguvk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3etuaskrq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3nxqafczw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrzxhvf.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3kqbguyjl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qnsjfxzb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3ejksvyqq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3paxvjixq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3oyrpqocx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cjiekniv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gzjxvqug.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3fqlwclpe.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3awhamrfp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3cnlppiqg.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3oagambho.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3edflmpyg.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ijwruqwj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nfnghrlq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3caymtetd.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3umglpwxd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dgkffwjp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kudpdvra.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3kclffsqu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mzanwvrw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kgbogqph.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3zvijpnmf.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tmdvofjo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3sciruajh.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3njwupufp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3eifxbakl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3szqignkq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjavrtz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3mhbmoalj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yckilrxz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3omvxsmnq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbxyrks.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sqyoxsfg.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jbehcirc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ybuwuqer.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzozrxpm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3xbaqfesz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ubwjhrno.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3fokuvkon.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3bxqgixzv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3niyxgtkh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3nyclvdaq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3enahpres.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rgddxqzq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3jqxyfpmm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jetyslvp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mujcvzyp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3oycgmeou.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rsfvffij.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zdezzlys.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lxkihdyd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rchuifnw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3cdiyiuee.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3wbllmdia.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zxosqycg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xqneqclq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qmlzmwcg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3elhhkkug.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3yepvmrea.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3bofznecx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3piwuznme.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vbungnyb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jpkguqmr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpiuvph.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mffajele.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhvxvycd.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wbvjssto.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pzcnrdew.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hsftvtap.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3txbkzaji.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fcxgttqe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3ljolypja.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bawdvkjk.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3queuhalr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3jizcidyi.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vweurakk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3fkznfvrw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nqfszjft.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jnhbgrzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmbkwwzw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3bkcqmpln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpmoieah.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hekrihdn.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3tmzjuscn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3crsyvcoh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3joiegyew.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3uhzdvond.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bblonwwu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3auicvmhh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3reduybcp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3phjoaxre.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3avokvlbc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3cuxdmteq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojwiwlga.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nfqvdbyp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ghokzqmo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xnvfrglu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3snocctop.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3icjkehjm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hjxjuuqj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qirpjlpc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3wzgvoxpq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fthlvbug.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3odfbgmcu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oweipoxl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajcmlfso.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3tjkmmnvs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gvqxetgv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3slxsvdgc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zlhgzqop.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3bouktmfd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbcxgwgr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3iqojcvwq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlqgdods.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zovdpmdt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3fhmvsfep.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qzsnuael.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3pylwwevx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hpcqvfps.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jcpxpfya.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3oanfnrwn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kohwzhum.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttxsvcwo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vguvnagt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3qznlzrtq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xiosxzis.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pwnrcomm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3auyvpabe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3cditxrml.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzjdckdy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ywjcdiqr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3osdqksmg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3njenonoc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mswpstgl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ygbghaiw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zegmlhnh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3xxflygzn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzxvfznq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dypyobcl.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3boegeazh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ahpkhjtp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bideqbjq.html


<!-- 参考信息 -->