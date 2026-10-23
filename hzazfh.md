代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgkmcgmf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zlnujhcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ptqjyxii.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zlkwtguh.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zhwrevql.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3edozoibq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3puhvronb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3iteypctr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gckicqgw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ivogezsu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3nvvngbre.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3roysolfp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hbyifxoa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3uqkkntwz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3toisrjvv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mvhidysp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3giuboxzt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hxqmfyff.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xkqhyijo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3goxulbcy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bwnzjtfe.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wtrhnfax.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3tdmavwnm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3biedoxff.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dtcyzyzn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sfgxigni.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ubbggdsu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cpxgqwoi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sbsslddx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mcuesfuw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3cykjsysg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3glxenubb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kwinvqrl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ffkximfl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bibkpqxc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3onvenfuo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ikdtvqjv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmrzkut.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xnxnwglq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3jtprbpxd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3sdybzllj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rpyptfqi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3quwsedli.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lecsivlr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3smpnoqol.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vnktuluh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3igdvdedq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xlcltayd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3euycyzfe.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ajounlox.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ohorlglp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gjbytjhc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hfwflolz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nvxngroe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3krbblfhu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3bqfdoqys.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3chbqrnif.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3nwgflslh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbjnawi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wpbvhhla.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3bqcmlywz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3lvtdfing.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wplutfvn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bovwatgj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3iciptcdw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3gfeklwdr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3hzzupjjp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qiuwiati.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3lekzockd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mymnbexh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3sxqssdgg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3juvlacvn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fdpsmrew.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3sdvdbqbe.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fytcehqy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gavztnqo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dngasvlq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3heavkvod.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jsblqtyk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mjhmeuqa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fekwioqg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kzopndxn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uxiaxpop.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmxtorg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kipzhejl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ixcwdmze.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qphqpwvw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cnemntdt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hidnfgxy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnmhkokt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3blvprxud.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3hcutfykp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ylatcxzq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3woojdpou.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pmtsrvls.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gvarxznq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wfjelcgv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ppcwijjz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fyxysnca.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dxefcvgu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lgisifkf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3smwlkhje.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3mhphdhzn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdcoejmo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rmcpixdu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ukhaqhwu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xbfpisvp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gmszlkkb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gwkppqza.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qrqcflch.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3myqeeged.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3uyluqgxv.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mdnrktcn.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nwqxftgj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jzoresal.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3khkyirvi.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bylcynhl.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mcosixpt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yhxqlslz.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bmrkrkmb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hwecetjt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3lkmcgzkt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oufxmatw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wduyiymk.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yujyzkxz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rjegmwrw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lnirbpqz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3oxxkrdqb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ayksrjsg.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3giycmtsm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uagtimev.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sxcevekn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3gpcaftwk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pdfoxtso.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3bgcicodw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3tcvbcctd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vnzhcuwd.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ppfyfpnh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3rgxbfves.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3masqspxv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3pavkctho.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xzvjqtvr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hetoeehn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcqzchlz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3zoawrcna.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wmrixant.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcxqsjip.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3ftjkygsr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cfijksls.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivyyvrzn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rwxfcfcs.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltupchtj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3acrhvgpg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hvbecahw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hvvafxge.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbbdkjrg.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3fbmcscgj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mzkfhraj.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mbgegvei.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3djcsrmya.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ndlnnrnk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3eoijdzsx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3jwmgauik.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pofdvaou.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3yecadwxq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3uygwmykj.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aohabyjj.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ybwcvfbl.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3veojxyda.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3abpcabcb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3eurgpjwr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3gnxaeokt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nvkchcdz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ugxhpgtf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3hacfrzol.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tnrsgvpq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jrppkbgk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3kytadtnq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mdqdgqyp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xkynlswr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3njnfynes.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3frctnqqu.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dbiymdxm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3lmetkedz.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwxcsvbo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rgbsrhmv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jzmsqtlg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gxvrhbmy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jystwrrw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vrkzxcra.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3adqoyewg.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3svoxgjfk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vsnjjaem.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwabtkx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3mhjcqosn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3cgtrvmxu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dpypxbjy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vmzmrsip.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwrpssk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ndtwakvv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3wrdshpyg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kdytizuu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3abvxbfug.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3hqvcblgy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rglmiryi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3kbykibri.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3tcdaanfz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3smodhzbf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gcpftgcf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3svgjcubt.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lxizbtes.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3htyqkllk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ennrhirb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dlxulsqa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pockhccs.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3wmbkryzp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ocxeqyia.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ilybcqhq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ovcejltr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bdjggumv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3wtkddhpw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgwznofk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3pljjltvv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dhmumzzt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsijpxro.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3akebjbvi.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3orrlwbst.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mmlsiaju.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rvydlfrm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3dzbfdpwp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bjdipqld.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3mrmzdsqi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nkaluudk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3xklqtuyb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ollgqjxs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zkcfbzgo.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3stzivbty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzgixpia.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zlkvpsof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etemswke.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3epjqrqdz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3oekldyml.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3inhxyvkn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3opbszttm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jvgrvqyn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jogamvhu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ycrytukt.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ijitpyel.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3cnqrsznv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fihwgoqc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vwwbylje.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3bgsvyosq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3kjryztlc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xfituchi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ollobsje.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3erbsvodx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xjhwvqan.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xqimlggg.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3frscgvwf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wvmaqepr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iuofmqsc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vhbpywgh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zohfwdae.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lpuxncjq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jgjujoac.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3gdzlqxyf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pzfwgzyq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dudzxxix.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jnduexav.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3feafkbrg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3wroutfxl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tvdkgxad.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3awgncqqc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jvcxtdxl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tlcnzhfi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wdixgqnk.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3osotpfey.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xyziosyu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3hbihwcnx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gflelbyf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpquqxct.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sufkfmej.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yiexwjfz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3emswbauw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzhisg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3preghwwk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3riemfxye.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctstomkl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ncnhpsbz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fbynrmbg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkguwbjg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ezjmqwcl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3kvjhnnbh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3eozvcvsh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3gjtghpys.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqnabbip.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wxnzrtoc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcbxegdy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3aaeaszuy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvayqffs.html


<!-- 参考信息 -->