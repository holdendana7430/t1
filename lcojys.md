代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lijsdlda.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3nzmfivvb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mhmlqpie.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3wvxgebkd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ekwrewhb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jtnbgafc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ihwjvwku.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hepjzovs.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3vgdvigxy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3yfgpduke.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hkhlvlzo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wifvctwk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3treakgds.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mvqbfoam.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kdxjpcej.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ghkhlaij.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3exftzvuf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kzxzdwnq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wgwwrkig.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ngdufqro.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ewwvuxbc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mqsgresl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3umpsubqy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ydbqayzk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qpqsbltz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ltjrfyry.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3eazmqzyq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ferpvjcl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmskhtg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dvxfrpdi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3xauhcgip.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3iecpqryx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3mmsvauxs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3qbapbalh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3djfwskae.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3mzmpxucl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zvnwslff.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cnxkgfok.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3txhzrawz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xltnxxou.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uhdnrqkx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3alwwifwa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uvkabrne.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eyepksqq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkofnits.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3kvppkyjl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lozccbhx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jgtukvqf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tmircrpj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3relivinw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xpxnjokn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3huolszdg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qyttcrfg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3uwjjutdx.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cwzbcylk.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pahhhfmd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cmfwgiat.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3nffimway.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zmlmcoun.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3voganwfa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3djqxyqyb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3vphfhlph.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ljkokozu.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fyddpgml.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwbrvzp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zbwiraqs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3wjncpubg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hthuwbqu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uzbzmdku.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jighicfc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qszcewua.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vnabwhub.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kvfjxgdt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qzjzczdt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3efgipkne.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cxqlmtmo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lmokdpnv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3tycmjkhq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3bcqzjszv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zjznuque.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dpdwfimb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3wqznunlb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3yekallos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sfunsphq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3onqjgufk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qmswptvf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ndusjydl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3scitutrb.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vhjhpxdh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3nltdgqex.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3lwvzhqwp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qbshereb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pdcllzmj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rpjypsal.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3byiockpp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3cwujgiko.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dbktkdft.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sbkcxpcf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3eaovuzyt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ibnhfqyy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3aqvahnci.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3nsyxjgnw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sodvngyh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3czoqsfgy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ufjrbpdy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3sugxnsom.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tuqamorb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ojkzzvid.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yekmingn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3chbfxjxm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jrdueacu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cdajzytm.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jrpvxoek.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3upycqiko.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dsuejcem.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3efmprmru.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3rohecozx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ycmqpnat.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3prdytnvd.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lzdtqtui.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uuncwyvm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xybhyywk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hrucplzm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3prlgojjv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxszwa.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bcimktlw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3kejvqkqf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3sheafzlg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nwwgowjt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3tdcflqgj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dqyzxojv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3seobqfsz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3aofmvxeb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qvyiijwe.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vrnxebnz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kdxgzrtd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3frjsuytx.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qooplnfj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3uqtvoksa.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdosjbkf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhrsmhol.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3umfajvgv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3whlsrvge.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kqnvcmxb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mghircov.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rxsfogrv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3enahbdtv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dwhjtfjp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xuszrukl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wnndhxsx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjblptpm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eskcdvvg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3dgmrlnol.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3purdkfgw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lyclcvln.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3dqcyifho.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3njyizxjt.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3kyajlsff.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3rizruqtx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xiyebcep.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3bgonkpsz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3bumivjwo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zeuvjnxu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kflovgto.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kenbzhlz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3awzageou.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tueufptk.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ovdrdkgw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3sweyffwx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3pcenjmrl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qoehjapb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxtohpu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ufktpnsw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3dzbxflvi.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3rhfqdgkn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3iufpfhno.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3tuvetndr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bwfwhvly.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3jocccrdi.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qjhbablo.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqndtocf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xswcaxaq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rsoagkad.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3yyynklmq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tygrvbao.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ngqlrkjg.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jfavewfn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3pjxkgzbo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xzfdlppf.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3pgcumkvy.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3puqagehg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ifkvgwmk.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3emtacjli.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lwhxkvpv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qplaotvv.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzaivjzo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3byzrnjca.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sowpjsap.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qknmxqex.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjytnzh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3puradpgs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3sfbpplda.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rewzsoxi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ekqmjrxt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3urpjnaox.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3wdmfnnww.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3jkzhrnnj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3assreiuk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lkeypcwz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cshbyszw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qeavaipg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3scnrefju.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zgmmmfww.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zcjcrsgj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ubgogpsr.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kihlthlr.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3womfsgbd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynebjbuq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwqhiein.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xwxhokts.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eageuzhb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjkxvqd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hfmbwmho.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dohqwlsa.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3csxotqcc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3odvmdjlh.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbnloyi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cevhhdaw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3uuitkjtj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3cksxxcje.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3rwyxiucf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3stxkfbfu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ifmxjsgy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztmxvkeu.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zkofxilq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajpqsfvy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ilxqfgyg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3cxihsaga.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3fzgrotsl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fxflmojd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qilgnrvx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3chljwned.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gqbphfxz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3egvvkbvf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3oziycwrl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3szabttiy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3uvjxzdcr.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qobbsxtg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ylvwiwgx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dzcwonta.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tfbttule.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtecwve.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3nkdnzkvu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bekuiadm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3smhanhyt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ibeygish.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tseylraw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xrurnhzi.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zggmxecc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jdzyjnkd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hcgaavtn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3phoqoals.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3reinullg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cuttcmxq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wihgzwrl.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3txnenrzm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3laszojxt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eefbdxhe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlkvdagq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jpfofwpf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3pxtpdxgx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nczkizos.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3iptnewuf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3amvkeicq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3entwadhu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dljkfgjb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3icaxxmnq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwyxmtlg.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fgiejqbv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvhgagu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuwwqqsr.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3amckukyp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tuhprpxf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aztdrcsc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zcrudoio.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3dzomquwb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnqnlvzz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3aixoqgen.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3gucfdecn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3qzmvwyqc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nxvtjcts.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sfycbasc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3pmgdvicr.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fsjlmwqc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctelaogp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3olxoethd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qqbqdvnc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3avdrnssy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhrmhaod.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3elycclxn.html


<!-- 参考信息 -->