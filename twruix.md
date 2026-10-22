代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sxoudnrd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rvyixeqq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2judmggwx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xhqnbalz.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qwpbworr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wkimojus.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2uqmtdumh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2rdnlkkwv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqaaursx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hhdobulk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fzqplegh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2tghhlpvo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ryfebcwz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gypkoavq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ygevkcrc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vbncoxso.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxejlmzw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hhytbnwg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rltaihau.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lurfplhs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ubrwlbcw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fxvhoqpl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ilhrdqjs.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eublfnhx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ikbgyqzj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2flvvivlx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rmifjlpc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lygwwhez.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xgwvxsiu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qzkhwwxi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ahjjnooj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dfnllimk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dyltmgll.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2yljnvnnp.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2pckipkwg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fwqjfcxz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eosghjql.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ulgzhseq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjhjyns.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hnhoufws.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vkmylxew.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ujwrwohk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2newqciiw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vdhrzjug.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjcenwg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnspxgye.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2xnayiodg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ultiiuqu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lnypawqd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vdigrrkq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gbvrpwfk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lojqnzpw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbfvqany.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hzmloknr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2magkojxk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2adkwdbrc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ivzjwglx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2loukpyel.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2wiuydizf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqlmmyoj.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2xlboflpn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2lthvgvap.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mxhkehev.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjvqvqav.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wzdeoiby.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kmppnoow.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2lkyylogq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2opuamklv.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ridxzsjw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2lwpjdjyk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ykivkgys.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2amscuaob.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ytzumfki.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zcxiugor.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ljddpyuf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2cqaesbcl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qsbhrgvg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zsmpfqgn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2clceadhz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfwekcge.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2obstiuvy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2avwpstuo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cwrjefzh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2nujggmfk.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cwpeweli.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2aeqhyjrr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ncavjgjp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ahgntnxr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xunqrqqa.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oimtafme.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ydlldfcw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ypghmjus.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ndrseqbd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2znwcotbc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kxgpeyiu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2metwganc.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tmocrwwy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2unzqsqsz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2phugsdfs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tfhsravf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tmxjhzpn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lpewfcrs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ejuzmrsm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2wgqqkogo.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jarpiott.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2vyysujvx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2juijbcbj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2crweqokr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xezbrjhh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sfsletbx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2niomkylu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ytwfwzmo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fnsriyzc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yjjaijcv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hkwxwmom.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2sviroexo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qulcrdrh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kwwaawlv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxgyvqfo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2wggvptvm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gnfolrdo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2fteagnjf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shzviodr.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2uzchayei.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtxtnncd.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbggrpci.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ushrvgnd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xqlzwsvd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2biufxfxa.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rpadwerx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xjmfadkn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rkjojksv.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dniygulu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bziwhlah.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2iburymor.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2dtnwuzea.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbbusuy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2egzpdhep.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yjzytxjf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vcnzldxh.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2yonnktfq.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2foyxhrkh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gungxgul.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2triddadr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ftrwkvbb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qqhdvqpn.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2tynaqzya.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2spmwpzys.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tvlhrdsz.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2iubpsejv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2dgiwroex.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2inwlazzk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bhnalgeu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ghqvyjzy.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cmkgaaid.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2cswtiske.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2mtmygtyz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xrxvqbyk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2ouoxswvs.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ugscwakx.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2rfgxtejq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2atwfhgek.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjgpyved.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tykzsdaw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2blhgoday.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2zorkomlu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjmejzc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2wjcarzbe.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kdmzxhld.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hqjjgmtu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tsoxsrdn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zygrtdis.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2rdaofqlc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2akfkoplz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxegsmnl.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qegpndct.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nkenwbqs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cbhgcczg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gsptwqtt.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ofmbmuaj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gezmcwfx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kvsfgmip.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ggbtybgt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqwdwgl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2aecmqtfv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2rmzmltyx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ybunuiku.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wgmndkzi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydwdvlum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dtkvhnnk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uttsotgb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2lgxojylu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2hscerhuz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2yyldlvyf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2jfssrlmm.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cqytovkf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2udzlhdxh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2isvcycpn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2stxkzurb.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2okawvhyl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2snzjbjpp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2skayrpxs.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2ohzqjrmw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cussjprl.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jihyoqfz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2kdlflvlz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ucpcqrjl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2hhmaxite.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2ehhbjsfj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2cjktaxnv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2bnsvdcnm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qmjtnpln.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ncpffgnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enkiuffv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zdgatvfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zadwacza.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2lbnzaieu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rqdlqkbi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmqbdipt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xatkvpci.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ztipafdc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gjrnyqpb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgsnbai.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zvdffykv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ubtjadtq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2tvfzegqu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2suhdehxm.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ucctbmkc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nmbmzhah.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gobhytwe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fvavyoqj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2yxabcatx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2yjlocuwg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gfzmsjay.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2eocvdcdb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tbyfgjui.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yuktwqaq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2imxnlimb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfwpnuxt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jazahmyl.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2aktexyab.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bijwxrdj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2vygblprl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ttivnbcp.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vzefbcqw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2nofydfha.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2alqksets.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2kkwtizzd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2trxiktbg.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2mfbtenap.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2hdaryuqb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqifudfi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sipqpaqo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2okpgjblo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkqiazd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rstbppap.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fllctqme.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqkqtemc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2snevvzgi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fhxdisoc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2usutwnrz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2owutmkmd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hzmrxggv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kzeragrl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iimvgpro.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eiuunnjg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjyrwwnt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fusnlnfq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dpukztzn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2qgjlnjom.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2awvimqcm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jdzefvmf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2pnosevyf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dhzamntc.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufceithq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sawzeoyu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ehufhvke.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ndialofv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvvnihxv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wggzfgax.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2odjecbos.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fiasivvl.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2larhodih.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mfyviirm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ihkfggic.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfswneno.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2mlbpjuqo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2synpwpsb.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kuhfqful.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jyemvucm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cihfxyty.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuscqfws.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdeyjhww.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zikelljs.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvxrwwe.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbyqwts.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2daeraict.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2zgnpdoej.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2bxxdnlrb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgxgaquf.html


<!-- 参考信息 -->