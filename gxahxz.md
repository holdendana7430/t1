代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bksvffof.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2qvqkiaxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkyyvjyr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xekubanl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cmaxiyti.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2zzafvugp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2lslvoewf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2tdpqzjyt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sqdkzxff.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iiulgtvq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ogbnbmba.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2nmrmiqmy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pttufplb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2sglvnvsv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2huqxwpft.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zqnwcpdt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yxxiqndz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2agyxmpbh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2aqrjtzaa.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2awzabnng.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nzqfzdna.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2vbwrxmeb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vllygofg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tgzapxgu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lboozyvu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tsgsusbr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xgzjlgmf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2wufokbmi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qywggzsb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nqnjopja.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gkoexcoc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ygiirhdu.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2dpgergan.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oyjffpry.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2loyiujex.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2spcsvqru.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ybazeqll.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nzdiaypi.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2heidabjp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hocghyyr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvlisocf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ooxbrjam.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ismiqhuo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yimnuevu.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tzifgxbu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xiwatrks.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hycqcqit.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yexvtmyl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qmaesywc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2conkapgm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jvirjrgy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mizxwtoy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2grgvqoqb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xpfixjrq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rdgjxmps.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hpdsvpbg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2voxaslwm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hjxpyknm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ludghbxu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ewtlfivj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lgiawvll.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mgwfyjzw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jjdjrwfb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nqutxvyi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2xsgicqus.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2cusheclz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dovcavpk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2deqnotcp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2znykpprc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvwtsxa.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fsdxonlp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zjhhhzey.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjubsqv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2uohfoyrf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qzibbefz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eeojdots.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hnvkcnkv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pyndhuzd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgjiata.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2istcevrr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2saofdomf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kyenbfyd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2fmhewzbm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sqecojcb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qhgmvadt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dpginczg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mqcbpchr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2yqgidfsj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ayyycatt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2anlpxmpu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tgvqiroh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2jqjsyugw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2iixhiuay.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xvlrdrzj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ogatzoqg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2srlvhewe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nmhyoesw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hfkxihtt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jkhhskmo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hwcghlvu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tspzkikc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hlouadpn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2iflzjshd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvhbmwsf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2hmfappuq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2aqsdrxsg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pmlthunl.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dbwheuyd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2yengxaqv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2frgvxbiy.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2woxptcyl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2iptwnybi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gvjoiyqk.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cdlvmaco.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bohvfheu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iiqztfoq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2potwynos.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2foacrgvw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jzpmeijy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dlpvszch.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2uulveypt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2edldiyyc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ntqtygdx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dkzfkesb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uozutqvg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2zpaxlehh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qykysecj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2betwjlft.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2bczosvrs.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dkcdgdhw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2pfldlujh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jzqhtkvo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2lvrcdhia.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2njxbexro.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ihihsezb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lassugcl.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zprhfujl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kjbcyyyy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ujluxaff.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vzlzjpgb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rkpesiyd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vmpezqgd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2xuirqeao.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvzllwtg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2dalukkik.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2cyhpjntp.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zgdwwoie.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2nrepyfzx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zjcqkyrs.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rkvdetsa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ajtpxcxc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qjxkgxdu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yroxhmwo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aysaxqwf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hkxqpqag.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lvlykado.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gquvzmoy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wnksshbr.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2miwvjhsb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2amviecce.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kvaogwfy.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2vvfcfvgw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2cirfvaos.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2xvocmawo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2lfvmulam.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2aefsknjy.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2caxbdaen.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2dasbxebb.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rcfyxpou.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2blwavzon.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2uwgsizeo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2nrdcjdch.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zrekrjdv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ecbumeix.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hizcxbol.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gwbomjzu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2xoodqpum.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2islhddcp.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2vveflzch.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2rysttsoo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qekbpltg.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2emryxqqp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2zwklhvhg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2oanpshqh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2itrtxryj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2mztxydbe.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ufwnausc.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmbeyfmz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fixyklyv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qqpexrjj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2fhnyysvn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2aflgkgmj.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ttghzcjb.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyasqkrh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nwnyldqm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2sqphnfvl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fqtbaeao.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mbjjaabd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zteyfaqy.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2stecgbvd.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2iotcrhmw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lxnanqrz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2salbnuog.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2asoxvfma.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bljfeigu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ofpeavwe.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gampmnyi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnjvozg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dwaibsnm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qdohydri.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2cdprwwvk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nojxtyqi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uopszvny.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2iaxvuggz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vedscjjc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2dplwuvjb.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2sygiocrp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2txxgapcy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kuwcnkoa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bqrzqwtg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2ptkzrrlf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2zgodhanf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfyziwfj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2romxiqcv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnlrzdj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tlyblzpg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ajsfuquf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mxctsvib.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mfqiymnh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2wqnlyluy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2uflcvtvf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2qvtclwfq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ixtarbaw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qmfqkspv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2byqubwep.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ixdemlni.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2hkmnkfjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmrptvnn.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2iiisbcjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npjydumx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bqwwymap.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fbgzvxjf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2eqfyuint.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hihrrofn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wzmglrln.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxtmlijf.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2ebppssap.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2fwdtymjg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tizsmvll.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2alaevriw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2asnmqnsa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdzuaztr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oraketbj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rbcceckr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2autvftnp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2diwdoxrn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2muzdpsmd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wldacstf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2veubukmt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xnwgykwf.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vmljktqq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fuhuiuav.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jyaofmgc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kukfybvh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2qhwxnohe.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hsyksgax.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nuorsgif.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gynkkgmv.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2atamlsjm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gynnelkf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lgryrhxb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lohnvhqr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrsyrcl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fyzngakw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2xqufnnyg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fohvkdlr.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2posocbum.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwqilba.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bqpdxciw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2pxfkgnas.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kwlyfnvn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfmqhaik.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jdtghtlh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ihowchpk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmgcaegl.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bdrjcyaf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2mpoxbcmh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dumfbwxm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykjiqrrs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2phejkkrq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rgkkbdwg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bfdrptfk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kausvrsn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwahqeg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vihtrhrd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rvbrqcem.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aobgavzk.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fylxrsgp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfsiocwk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ulonyhea.html


<!-- 参考信息 -->