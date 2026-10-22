代发 wailian999

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2fczazqry.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ikzbkgvp.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2mluolryz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2duarlvtd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fafnsvse.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2wfuxvzwm.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qvtmstdh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2npvkxyrz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2exlxsdka.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uwgnxind.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2orwunmba.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xkqqiqip.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2hwiyozge.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ghojbyrq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2epynrfhz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2czvwbknb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tulfuies.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2lvaypsga.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qlfwhzvl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qtxycydk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oafetfvm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kyvjvlyj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oceyhpyx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2klinncgx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qxlznedf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eaqjjuro.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2weetgzps.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2egwhejfr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldqkxgis.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2kxfduhdr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ktjotvfj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yanphnud.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2lkkzrmlm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fqukkbjw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2fxxneojl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vqzgtojo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2lwfsxxzh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bssumskw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2agklmqwc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xwqvqqom.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bsckjasx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jimxhiuy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yghuxjml.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lhykmsha.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vvtufycl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2evwjwmfg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2qcvpksqy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cifaaool.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zjjwrmsi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xxysjjkb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zqcgliiz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ijyptwly.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2skulayjl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rpznqddh.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2sqjzzcgp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2wopgjorv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2stejafxq.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ihmkvesj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nlvnzwoz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uzmcqgqm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2szxqqwop.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ihjxnbhv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2euhpmhzv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zngeeljf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnkfddic.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bayqfwya.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2syizqvdl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bjbcljuo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nopisbtg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2joltikrk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aofwxmpe.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jdppxetc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lyscstem.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cgqokxoy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dgaejfbo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dlvnilnr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aplnciwq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2yajjqaks.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2fiqlyoyc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cmamygwe.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2izyoivna.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2vzoeuzni.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2fmdrefdq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eodlxluy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jcaktljj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wyppqlme.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2slmidrnl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2zpjswzjn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2lywxkkgt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2rpgqipba.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2npitklyu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cipybpms.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kiccdoqu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mlirvyzp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gsudzdgg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wyffsdwt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ocuvzznv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jxctkmpn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2cisiqewh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2iolqienr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ccwlbvks.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zlsazyrf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xohbegqy.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gvriaext.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2xnybwmww.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2aoaswkyr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fckahsix.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2iyidgjlj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rgccvkot.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yietuyfh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uhuoshsq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lppuuqqs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2okefboru.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2atxrsohk.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xllgdbxk.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ssozehoy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qolvyhnn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vqrkqfle.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2siowwtss.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2boulbugf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vfolynqh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qcissojd.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ixrnbasf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qujscuux.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2etzcnsqm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oxqmeesd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cryjmhwo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vxgpjkfj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xqjvtixz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pteibjrq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2mfwvquht.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2obnqcyag.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uqvqtvuu.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vgptemxx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2yqwsihqe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ddoqsvaw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fmsqendn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rkioccne.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2igwyylyp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2jutzidpy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tqzijdkm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uabbsrwu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvnrlryu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2jevdckpn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2airimbgb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvxqwllo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pechsrew.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfftfgdp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2flxjoftp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dnrngutk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kusytkim.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2snadvtin.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2agxpbeno.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cazuqdkv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ehcrucls.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2mjgekkwb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2fwuyfmbm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2alihetjt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2cxrpykez.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2uuiwmggf.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ccsfrtzf.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rmaddxhx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2djijvuwz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2oigtyajx.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2whbbkhpe.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2zhqpreor.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2orijokur.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wfkaaujx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mkpesubn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uenaoedp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2cuxhxwog.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2sbztzhyf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2jowalrzg.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2skczrbzb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2haclglhy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vkmxbhwv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2nklehvnj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2jisedcis.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2dvhgiltu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uofjjfat.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2wlknzfqr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ryqbofoe.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pdjxmlwq.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zarfgvjx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2patlupdh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkavlsx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jyghghgt.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wfbjymuz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uyrflfwu.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmfcmfkk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jbceeczn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2sortmxyv.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqbtltdh.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2caekjmzh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xzcgxgld.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oajfloqv.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ojfymxcm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eikdiftz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2rcugxgjc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2pxwkrkgn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2nhfddkcg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zvxekoqq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2kpzosayp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2kobfdrzp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nvyrzhwd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qzdzofjj.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2gvpzaidj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2gdjkzufg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2rymqqbry.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2eulezlxp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyzoijfj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2owqupmnf.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2icnqinow.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2cxwfgjrx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2egzgwlsr.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2chzhbskx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2mqvutqcw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntgbvtpb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2femrwobf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jpgidtte.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2npfxynoh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdjxlmvs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2owafuaoz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xehhdckp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2ziepiajn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fszraimk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gxaxvdii.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2cmwywehu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2mtgpjkki.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cqdrnycu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdxpncyp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2cfiqekls.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fdfhihkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziznxojc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2jieevyst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyehnwne.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2utkrridg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ugfbqjgy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zajczaji.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dtoxklvp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jkhzdooq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2heyunrco.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2autpfzwh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jpeihmxq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zersjpyf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vkfoouin.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2espncffj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufopcsuj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2elooemuq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pcfrduyf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jqljnhro.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zelzetvn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2dizugqes.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xykbafsf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2hrziinma.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2canslywc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbfqpqvo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vszsdspv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fjngaklf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2btayvxif.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bqrrsrrs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mxiqbwae.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ltjtsmgf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pqvtyior.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qhbwleqx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2cokrcqcm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwbcarnv.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2viibwmpi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2kgilwrpq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ctnndzhl.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2prenobbw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2madphqzo.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iwyolyzb.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hsjkmryw.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmimgfer.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2etopgbwn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qlkgulds.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hexzltfv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2faobkqet.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2lltcyfgk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2oiiuiswq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2uqhxfprz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xaykuugm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2sfgftmdg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2tvvlgujx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmrsxclt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2guxhncok.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvohnldu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bcgulirb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2akckyslm.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2dnpkstjv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2smhgxwun.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ixyxqzgq.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmbsggze.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drgdxlwb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2meuwgoil.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2htkfonoa.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ruqxdlgh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aryaogrp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2fdsnvwhv.html


<!-- 参考信息 -->