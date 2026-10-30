代发 wailian999

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gcwtalwhb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gjvknallw.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/gtlsbexjc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gidbecrpv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gmzqbvpjl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gykgisfwe.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gqpupmusm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/gzxjimelq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/glfpxdnee.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gostlqcri.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/ghltyasjz.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gpwmsxilh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gtbqzrbuh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gixxrleup.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gxwsjtapj.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/giwcrofbi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gbhagiyfn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/glfgeavaa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpvpcmkoq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gufriaqpb.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/goznluovj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gsklmuuui.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gxpncpsec.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fehbvm.com/Article/details/gibjzfyrx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gpqdvqaio.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gyrebxern.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gtlcqbwee.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gjetkcjhz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/glhvmhhyj.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gwspxjirt.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gzuoifhbp.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gnbftxirf.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/gpkytxaqp.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gihddhbfe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/gshbeuxkt.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gvggambwq.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gddilngkw.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gpvupmrjp.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gwxthmnis.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gczoalpso.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gpnfgjvdg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gobzlwmdi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gflynxbog.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gtpbvcnnw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gdmspzdxx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/ggdauhbiq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gougsihux.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/ginaesrmb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/giamafpfw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gkuywjekd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjicthcwz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ggvwdnqof.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvsftownd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.fehbvm.com/Article/details/gssuebntr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.hesvh.cn/Article/details/glkqpblrq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/grprapmhh.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gnafrszdc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gkioosvwn.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gnmkwbhkz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gtyefrzyq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/geivflunw.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gnpxvqvkw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gldatdxzx.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gvziokunf.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gjyshkuxd.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/goqixamii.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gzogbtyaq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gxdnugeuu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gmhqbqweu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gaariubnk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gifuuabal.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/ggtxhbpqt.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gygfvvwnl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gnhxpmtwg.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/ghqgsdngg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gvdiizwfm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gduvatast.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gnliomyqr.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gtthfhvtr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuvyryp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.zdbjq.cn/Article/details/gedhpeijv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/ghjduhsne.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gnwspqhvb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gbbkioxsu.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqqyrxzhl.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gzdjshdyh.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gvqjirkyg.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gfrevpcac.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/glnzbawpm.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/giophbloa.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gzsnuytij.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gycvuwxum.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gmpxhrmcx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.zdbjq.cn/Article/details/gehhjqmqq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gctiusscm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gcauvgssw.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gvpxwycsu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/guekqqwzw.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gwaowwaeq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gkuwawbie.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gjhxwjbqq.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gcfvdqbky.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gjbnlqbll.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gjlafkkrs.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gduuarbhe.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gdkbgjtyb.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gvgojkazp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/ggvebaeeb.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gkkjyafpl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gezhzvrbc.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gemedmjvm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gokgzbsva.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/gddsvjrlr.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gppxnihil.sHtML

TS:   if (!x) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfosvgicm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.fehbvm.com/Article/details/gwbbfrqlp.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.hesvh.cn/Article/details/gkogyxwum.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/grmvhhron.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gwbhleuyj.sHtML

[A17] 位运算
来源：http://blog.fehbvm.com/Article/details/gijdxjjke.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gfavuhvwc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/gxjgayhjq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxrdmtggb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ggrizcnjl.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gyexwfbzl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/ggetfxdfn.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gvvmfwacj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/guhbclbfq.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/grayqmrms.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gknesoxfm.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gjmfatwfx.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gwzsxjmti.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gkwpgweco.sHtML

Java: (int) 'A'; (char) 65
来源：http://3g.fehbvm.com/Article/details/gdkkawdka.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fehbvm.com/Article/details/gvhacyucs.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.blog.fehbvm.com/Article/details/gmezigbsk.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.hesvh.cn/Article/details/ghvrcqrji.sHtML

[A19] 交换两个变量
来源：http://www.blog.hesvh.cn/Article/details/gchywstps.sHtML

Py:   a, b = b, a
来源：http://read.share.zdbjq.cn/Article/details/gvtevtdds.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gpnbszrcr.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gubswwhav.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.fehbvm.com/Article/details/ggugqvaya.sHtML

Java: int t = a; a = b; b = t;
来源：http://3g.fehbvm.com/Article/details/gtzowjelv.sHtML

Go:   a, b = b, a
来源：http://3g.hesvh.cn/Article/details/gtaoufxnm.sHtML

Ruby: a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/grybnfhpg.sHtML

C#:   (a, b) = (b, a);
来源：http://3g.hesvh.cn/Article/details/gvhhteftj.sHtML

[A20] 读取标准输入
来源：http://m.share.fehbvm.com/Article/details/gbxhkholz.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fehbvm.com/Article/details/ghzapqwur.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.hesvh.cn/Article/details/gmuhvnkwb.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.zdbjq.cn/Article/details/geayhaqmf.sHtML

TS:   // Node.js：readline 模块
来源：http://3g.zdbjq.cn/Article/details/ganksdlqi.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.zdbjq.cn/Article/details/gonbypfqn.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gkzezdblr.sHtML

Ruby: gets.chomp
来源：http://baike.fehbvm.com/Article/details/gabltsnfw.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/giztoefgn.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gobnhnpns.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/gnnpywslk.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://3g.fehbvm.com/Article/details/glfjszbgr.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gsizkaafj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gsosufhgh.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gzcnwnxxh.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gacqoqsri.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gmcaxmwvm.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.hesvh.cn/Article/details/gtlsvnsal.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnqkcgyiz.sHtML

Py:   len(s)
来源：http://m.share.zdbjq.cn/Article/details/gngjjppwv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://3g.hesvh.cn/Article/details/gtygsilbx.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.zdbjq.cn/Article/details/gmwvbwwau.sHtML

TS:   s.length
来源：http://baike.fehbvm.com/Article/details/gbvlpumfv.sHtML

Java: s.length()
来源：http://m.share.fehbvm.com/Article/details/gcrkzvnqt.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnpburohn.sHtML

Ruby: s.length
来源：http://m.share.fehbvm.com/Article/details/gfvmcaixh.sHtML

C#:   s.Length
来源：http://baike.hesvh.cn/Article/details/gncfspiaa.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gnlczniux.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://blog.zdbjq.cn/Article/details/goetbrsow.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.hesvh.cn/Article/details/gviszlnwt.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gcixpmegr.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gniwoouhd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.zdbjq.cn/Article/details/gsyazzfji.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gxwwcondw.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gekzvqjwm.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.hesvh.cn/Article/details/gbyxfeema.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gwabichnj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/ghakfdsvz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://blog.zdbjq.cn/Article/details/gmqqqdomg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.zdbjq.cn/Article/details/gnjaloiiz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.zdbjq.cn/Article/details/girjjxitu.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://baike.hesvh.cn/Article/details/goumxlsyt.sHtML

Go:   strings.TrimSpace(s)
来源：http://3g.hesvh.cn/Article/details/gvcmbfliu.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/gzklsnpts.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.hesvh.cn/Article/details/gfjbmdlcj.sHtML

[A25] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gxvzfglba.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gwrosoqdg.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.zdbjq.cn/Article/details/gxknagggx.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/gnmjwkcdb.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gpzxizdbi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mobile.fehbvm.com/Article/details/gpojfwddt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/glglhntwf.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/grmcstmyz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gkknehkdc.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/gqreutfok.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.zdbjq.cn/Article/details/gmrpsdrfe.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gqbquetea.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/ghcvvvrao.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.zdbjq.cn/Article/details/gplkvndrm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/giryijdcr.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.zdbjq.cn/Article/details/gqznuorqu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gdqhuxkax.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gokehgnqf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzjllbeez.sHtML

B. 流程控制
来源：http://wap.zdbjq.cn/Article/details/ghpccuhbe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghgtejgee.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gmecnhwfl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gvebthkpm.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.zdbjq.cn/Article/details/gxdrigqyv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gvlutmstn.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gdfktgmix.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/grhfnrpjb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.zdbjq.cn/Article/details/gvucbcmzz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wap.zdbjq.cn/Article/details/gwcpqljuf.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gkbnlwlcb.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gzwdgtiyr.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gymnbqysb.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gglwowrqg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gfwcpjwxx.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/gywlvemmx.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.zdbjq.cn/Article/details/gposrnicv.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/gkuqnmadr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gkfvootgi.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gceqvbtvl.sHtML

[B03] switch / match / case
来源：http://m.share.fehbvm.com/Article/details/gmbnqxlhi.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/givcbhuff.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/glsokukgm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/grrysqobr.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/goucmiaes.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gkfedupmn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.hesvh.cn/Article/details/giyccvcrz.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.fehbvm.com/Article/details/ggscmsmcd.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gpeizradg.sHtML

[B04] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gyyqdvpky.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.zdbjq.cn/Article/details/ghjejgsoz.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/ggdexmrje.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gaqomiejh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gjindumoz.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gsmqvkgdz.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.hesvh.cn/Article/details/gvvsatcig.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gltozydrw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gmsctclcw.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gkoducypr.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.zdbjq.cn/Article/details/grmubosmy.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gflopeizr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.zdbjq.cn/Article/details/gvqygfmba.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gykmfwzfh.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/glamtdvvk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.zdbjq.cn/Article/details/ggcxrauvw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.hesvh.cn/Article/details/gjgzolxuk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gmafcbxzq.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gqonfbzdg.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gjbxnvgeb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.fehbvm.com/Article/details/gofbbgpme.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gktdloefg.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gwykckwxs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.fehbvm.com/Article/details/gicmfewig.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://m.share.zdbjq.cn/Article/details/ghnlhidov.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gsegxjbpy.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.hesvh.cn/Article/details/getqduxdy.sHtML

[B07] while 循环
来源：http://blog.fehbvm.com/Article/details/gahbcizcm.sHtML

Py:   while i < 10: i += 1
来源：http://baike.fehbvm.com/Article/details/gcwsnpktq.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.hesvh.cn/Article/details/ggnweljsu.sHtML

JS:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gmpmmtjdl.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gndcahncp.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gqarvhmuy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.zdbjq.cn/Article/details/gbkbkuraw.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gnromeuck.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gfbycznzj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gyaemuwvq.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gnqeqrajg.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/grhacgdlo.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gnycvayei.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gcbhhlrey.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gcevknwtv.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/gwitqxeop.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gghsbfabv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gcafqkmny.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gcipzjdoq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gapmduwyd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gimvwkjwj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/grtkbtokw.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/ghopobhul.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gktnpyudf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.zdbjq.cn/Article/details/gihnmuxul.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gpufkviua.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gdsfeenci.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gvfumzccp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fehbvm.com/Article/details/gisfqkbpl.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmaydies.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gxdjrkqiu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gognlmsiu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gryyjfbud.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.fehbvm.com/Article/details/gjcaufwyo.sHtML


<!-- 参考信息 -->