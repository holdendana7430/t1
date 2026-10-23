代发 wailian999

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kazddpms.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gjizytoi.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3scdgcebu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jeylljsz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ytmwcqcl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3aedfechy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3uzxswxsf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vhhywerp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3jnbbotes.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hizdtnhk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tixtahxp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vlaodsms.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qpytmqsl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wyscpexp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3idetavap.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fgrufdlh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lyeosryc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3svzxtxur.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wyrrfamn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nspszavg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vgomohcx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hdarhkfo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3bjkivqmd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3cpdmncaa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pahmpmer.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ssoflfgn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zyupuztx.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3oxuklokq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kvkynjqa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kyherosh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vyyisoqk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3xvabmfcd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rpyswlrc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3scyybbdn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3tkuzzdqn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3aapshpsh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3lvswkser.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rnrbxztw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xxlgwyuq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nsszavod.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cnljesql.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3uwkqignv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wrennwvp.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jcpdzhfe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tunqjvjl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tvybviet.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3roomwefz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tyaebcul.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tjzlurfh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kaemsplg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rjlkmadf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3swxgdrjq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yplfqgnd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3tcyalnnv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mzxumvvj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dicqkacp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3abprvext.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ljvffvek.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3facqwjhu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qgzwrfow.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ssiyewez.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jrvoakbt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vlyavkug.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wpsctsta.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ltolollm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fgorbbww.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ecvtjjtq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wsogpqkj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cpmiphgw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bwvbppih.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xbkrcfjf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhfbnuio.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3sfqlquij.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ixyibvln.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3oxzmbacw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3odkktgna.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mssdkoyg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3kxubzjyw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3altctoxd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3dmscgleo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3trsuuohx.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dctngmuj.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bxtawjjf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ehxxvfzp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3egstknpu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nsrrvooi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yoiifxii.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gowkctnj.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3kvkyowdt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3iuozgtug.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rtvaelbh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ryzsnbyb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hvhanfso.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3nmphsecl.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3krgtvhry.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3srqntunk.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3owvhkdju.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3grymvljl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jqdpemav.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lbhjdhht.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xvrdzihp.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cyegwrqb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3eduklcop.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jxviyvyy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rboraxmx.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3trdlkgco.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3oeiridbp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jwcxlryd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3qporalle.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vaufdhre.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gsdohduo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3oqkrckdh.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3cwfqxyev.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3ofcburjd.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hppadttb.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3uikkvwcq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cnliagbj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvkriuig.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tikkrsos.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sleirzuf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dgmkuzxh.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjdyqsaq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3urfnqdls.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3chsicypt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3wfkzwpnm.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3vltkvdga.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jsyoskok.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qwxgxubz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hjtuypty.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3imrpatjq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3gzcgngeq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dmjwprvy.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3aamjfjwl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ayxmwxie.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3aitbmvxu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3oolnngvo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3zktkdlua.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3pqkcqqse.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qvoqbjxy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ejrdibhd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3tglfvjpr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3syuhpifj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3fyxrmvbk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jxltfxdk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rpkekjsb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3lawrecjs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3epusvywe.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3nlsrnimn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3nwmcfcck.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ciyuosah.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3aovqcnjo.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3jcwvydmr.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3llcmgdqa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfqgwyk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xruzipsl.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dumsepsm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vtdqbvfq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eafsrosn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3bkrquonf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3weewyihe.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3yoyjqybk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwkttnmv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hptjktmd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3zxgwpxqt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ripuvcwa.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ehvnktso.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbtowrvq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3lgiclefz.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3xldafwhl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3astqkvts.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ypdbqpaf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3srbnglaw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3runblhsb.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jyvbrwdp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3luclqquh.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urogmqxa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bxukewnx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3neqokayz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3dadrncoy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nwxrjkzw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkhqnuxv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3knusbfxj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ydwdvmdd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bgeormzh.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3vqovntiw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3dazohokh.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vrgeccoy.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lfoidjzx.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3fghxyost.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3slhwiqxy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3solmyutg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nezqdcof.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bixxpyfw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kmkqjabp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ppnmjaly.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dbepatmi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nbntkadf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3bnhzgudx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3frjrziqp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gzqqkyca.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3lwpesxfo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jidhjzoh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3iuiqydqn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3emiqduvv.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3euwaczik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swsmntij.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3cbddamdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxbcqmiz.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3nupfwhft.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3lkrvhdmp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwgztir.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3irpsaazx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3caxmjkus.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zedspqdy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zyhaoeon.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3udeccvgz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mvetrjwh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pvcrywvv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3bwsurgvd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nxerznqr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ydvedvts.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vzfasbuk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tkgdjpgc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ywyazxah.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xoyrqhhi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3inugzehr.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3stbzefit.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dbecsfst.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lfnnhine.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3optlduys.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3asokyadf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sarzzujg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lamvvies.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3asvpeufv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3menzydok.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ximxlqmw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3tqopmotp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3stropcoq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzzhbbwd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mirdvqii.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3gntwqnbu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3oliwtkgr.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hudpjqhh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3czvqrcai.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kbyulxgt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ilzyjtnk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ghfmkszn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtnjhf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxdcdrg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgrwgwxf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bofiggya.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dnaqiwud.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3anheauvq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3klzwtpzy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uielxhxi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3anncdklq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3largmhas.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3lartsrmr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sukfowhj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3txwrczui.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3wtuqltxy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdufrcih.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vlyluclh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mzcyctcp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzblcog.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uvjwnzur.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3gmkaoejk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcdxdjy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3uzkcsgef.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tewdeugx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3etnhxxfw.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3uisovxbf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3huebzhnu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qeznahaw.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rewwrrym.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3awvqgdkn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lczcdzhn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3apfddhkq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3tbkztcll.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vkwnusqz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mkfzaokd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kqnrkqag.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vfylpawx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ctuyntsd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dtxdnvua.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vtmkmfjj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qacgrlvu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3dkydiiol.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mvoverqd.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3wyrshthc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3iljjrvna.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfabmqdb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cwxjljmt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xzbuletb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrvaksjr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xfaboxph.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3salrwxdb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3pjnojfsy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3dwhqwisa.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zwbaylux.html


<!-- 参考信息 -->