代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2elfjovts.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2anfssevp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qhnmfocn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lzgolyax.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hmdtkdgk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2pssunsaz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sfauixfz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ndedjvdo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2adjscqdd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gelthbzt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2lnsvqlvy.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2eocezdpn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lkfmbydh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2muftoutp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vsxrlodh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2byjukfap.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nxjcorru.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xnsqksib.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fxbvliia.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hmbudpvy.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kfqnbkai.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2expwpcaj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zkgyladc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2funqrisw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hhvximyk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ueiiielf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jlstdaml.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2zbyklkcd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xebomiea.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2smqrwmzw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2lglzdboc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vtivgwuj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ldgywdrh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2czuokant.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gvyfjyyf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwhdfuum.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2insrktln.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dtamjdha.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zzowypjy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2caaswgbg.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rbwwlukd.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rfbewuhk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gudiegbj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aliiynap.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qpktuhei.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nedfnylm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2mpxbqrky.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2wcdtsleo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jdvyewgk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2irlczwtm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cvycvsrs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lnoyykgi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ghjimzfs.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2getdsjrb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zdfbkagc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2cpopoeuo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ogkzfgsm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lubyggef.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2tzpyknci.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ixgclqnd.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wynwetup.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nihjesjm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2apwfutjx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2erypjbec.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fbdgvzwg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2yuxaoaqi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lskflaku.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ndhcvsik.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2muaybbhk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrygzisf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wbrcudtn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdqeold.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2swwapuuf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2lhfoirvm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wxqusdms.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2khkqxkbe.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xzdnlymx.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hkzzrwsa.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2msdrvrxf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dzieeogd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xofjodpy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zdbvpfck.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wwplkexg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrtlfgd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2irwmmkkn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2fwzkwmrc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gveogeiu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2veoqeaqc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ukmezopr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dqthngtj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cqglovkv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zakricjf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vptblqji.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wbadojir.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ohxuosey.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2swdretbf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mifpuant.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fotabvaw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2msmjnnyt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zkkeolsf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tplopebq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mrazsbef.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vnuaklqj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2myfutuvu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pplzanbi.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggcfaeoq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bintdsgz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zofeegaa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fzuuqdrf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fyupszpy.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qfjdgylk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zzinfkrf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2zzkfdykr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nxzmzffo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gbufhupj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tifujjxw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hhmtjnen.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2zxhzrket.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2icpzyhbz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kacqpgsj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zrmxwwhv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kzltitzu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2skrfdxua.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ntiqyolf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2llawihti.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2depyfwvj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fbwfrtah.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2nbffbkhg.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2grdtyxhq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zyfbiuwl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2isdxofwj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2rorjbgqh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2tssvmwoh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2btfdhvcw.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lakzivfr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qddwhsvx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ekfodejl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2akhdfmdz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2chdglozl.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qwpfhetr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tljsgvtw.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2arucdtxo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjboarif.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2akvmhhyk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yuwparxj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mezjptvc.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ehdtltzo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpaujjzy.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ouumeeaf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2uklxrltj.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ulnbuham.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fqwkbukp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ppdkztsk.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2fifdsgcy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2zrawdowi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lljuxyln.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2uqjjkovo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2aeynbefu.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fpndcump.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2vtjbpcbe.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2derybjyk.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ywchfskn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2sxcoreif.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2osvmelea.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2atsqhlat.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2yggwzjck.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2xpqbitla.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dnktfoah.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2ttygkdbn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2sexziyxs.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2awmulsfz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2fvsrogar.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2smqooknc.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wanqbkzq.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2lnqsfpvp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2npwjqmhl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2zyabifrd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xzzzzxiu.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vwbrrmqr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmodgssl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2etdbsrdh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oljuvjwe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aviwftma.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2gvpelwzj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2csbdxdqq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tulqbfam.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2yhqtbvlt.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mdjvzmpi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2hhufvcpq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bwqobfar.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktrdrcey.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2wvnhpnaf.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cqjuafmm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2paklnybj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gntccbcf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2frljkpzj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2pqjsswwf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bntxuqqd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qomhuvcq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2vjbbxqxg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cgkkiotu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2uphtdloz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2eptstvci.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2djixzlcx.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2glftttdf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lextwdql.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2guqxgvzx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2keqlvmgu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldhmrwok.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2aororucs.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tsatdkqd.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lcnpwmkc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mbmgehbx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rglkhgip.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rapfkmof.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cftgolhe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzvvrxv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwjfhtxo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2aanqowvh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmbagqn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2czbsqjkq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2khocmdpf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2iqqdtbrd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rjqeettv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2dddstcsm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qarhsqev.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2krarzpbz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2eqqgjaaw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2rwccmjgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdqoddns.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2qppskxqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqeaygkz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2svowutyd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zgpamhlf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhiwdvbj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2stwxbekm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dnlxunna.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kulcneaa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkgreusa.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2vvgrqbhq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2voowjozo.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2soxcuepl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2uhefdfxn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsejbsbo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2okyespbv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sdqdxiwe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2qdeeslwn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2gkjffazi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2nogdorlm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2tsrmlxld.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2wyuwtuxz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ewqisqhe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lvprohgz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2noynogjx.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhrtvlyt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ecrzyycy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yjfcyyud.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mrrxsfrb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2puberkom.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hlmanlsk.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2lrgwisqu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnqbzstz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2olyysrfq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2geaokgwn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvsxwopa.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ihfjtifa.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2orsstfbi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2svtzolhy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hmdmeckv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuibclj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2boujrhry.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bszxgcku.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xnffmanc.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rtrqbwfs.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fhlnwshk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mcedsjch.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2riejhwja.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bousiskk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2yjuuwggt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qranvhww.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ertuttlp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rezstxrd.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2avteudsv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hzwprdve.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2iwbzlcmk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiqdayfs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2azpvxxsp.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2blyiuele.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uusiyulx.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yrevkkdc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wwmbptqr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jijkotrh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mpsbzxdk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ieslxayf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zebluunm.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2iqexpgoj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pdvkrjwv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xqxpdtho.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bzknildq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gbstrhsv.html


<!-- 参考信息 -->