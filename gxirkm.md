代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ttsqgyhp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kqikwaud.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jqnxjvzv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2vsjrxyup.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vqblztpa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2llemyqte.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fyxahrbb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vpsmmxzv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lmutguzv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gxwvrvgw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2mdwtprnl.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2lzjsmwcq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2pkwdwejw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jeivesjv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2gcqbhznv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zpzkxpte.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wichtqyx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hxevaweu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ppdexzzu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kxerktmb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rfmafsop.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2xceipbnf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tcuithgt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2laexuvjf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwtmecs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2twagvuzv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tqbbnuyr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zglfzkhr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2boivekmm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2fleaycgx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2aikdsaxs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lztsleca.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2udbnyyol.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hrnadval.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ctjgsygv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nfuegvyh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eyahluig.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhijaoxl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ylczssin.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2rzeslqdr.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2nqnuylen.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2nsamghew.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ylztneex.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cxlombcj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oyafugzx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzvhawwi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zqbojtid.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2zadqpdpb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eopoqmeo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ijrshntt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jduigtxz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mjoyseyt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jyjfqckv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rblmkbvj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jvrtafzq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dhfleumb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2bxxnizqq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2enidfvev.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nbhrqbmf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xenhymzt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oblhyavg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ykzuiqpf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vueegxqd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mxrbxwnn.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ccfmvsij.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gjnqavzx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aztbkhga.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2idrnehgy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2cfkhqslk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qugahkih.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2demnrmpm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2htfqrdul.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cyjfvmkv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2jbsxetlz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nkprmopa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2vebnqmbn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xvwdqxer.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hqakdpqa.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eorkyhig.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kccxpqjs.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2itbrwtah.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jehnjmxf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xetydpek.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2vtxteejw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ngolwxaf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dkwtdkqi.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2vgcmrsqx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cpauragl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vqzainww.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2urksjgxs.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwwpveae.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qacsjpwe.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2hvdifvdh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hictaset.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qowxncug.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2rilkpkka.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2svlcluwx.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qtreqlxg.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bhmcpdei.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rqyxxvlq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2opguffcw.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hdiosuzp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vkmxhpay.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tzfgryva.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2cltotkuq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pviitfvd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wywgfbtu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrxffxv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2opprugep.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2xpwvfngc.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2phofnkcz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2gpbygadg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2gdausyap.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2vcyandgd.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bumuwxyi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mbwprrjz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2zidckehq.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2apxfvprt.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2enowtein.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2vtjpdtyx.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qlfoefhf.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2pqhvdhwt.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hkopfytn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2rooccbfb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ohuhjpcl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pfzczwae.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hreabays.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hnzdnkfz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2qsbakrzg.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2muszqbjb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2guszybga.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ihxvucgu.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2cipxqylp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2inekdwuj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uabnpbpb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zehpttin.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ydwjiafr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lgpigfhm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2haxsnbhp.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2cviopfpu.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rrhhnogz.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjlozzcl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2hsuobewu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xwqevpkn.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ziqxlisa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2hollspbj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddxbqdiv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2kxslubut.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wjakeict.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2evlitocg.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xnnwgtgb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2quhhlyhx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2wkuggutm.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xlgzjlco.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2askxmgum.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqfyppgp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mxukxiih.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2nhqzjpyh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2jsdioufp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2baaegkto.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbotcbh.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fppzsogh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hjezttwp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cwzipgur.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2najircxw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ncqcdinf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xcvvguiu.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yrdpmaez.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xyodpafn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tbltvwfc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2cdvwzhbj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2sgitcmgf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2grhkuatt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ravxqyuu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2uhywbodx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2wkuifxmk.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cmlmlgik.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2rikrcdvr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2euqdbsku.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2akeawlgh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rkpuhare.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2nrxmwjhw.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2ktrtfwqx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2jbtxaaxd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2olywxqlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjpcdzsd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2krpxqxyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdgpokoq.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2hsjkgbej.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lbtqvdun.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2afhjyuzi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2toafymgv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qosmfqcu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pshlhgnw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2yiqglqgg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2sbqtqqdh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2sdprefix.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2dprbxlll.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zwavssju.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujncmcvn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dlqnouge.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bozqwqud.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ncqxdtwk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ceviaoql.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2ynwhafon.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pbdzkboc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2zvbarhor.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2gvsjvzry.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ehitimts.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvmwybzd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obgaijfu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tutoobos.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kgkvygjg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2yuktqqdp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2lbudrily.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lwuosfnb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ksjyheqd.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjbizdqm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2plounpym.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2riyhydtb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2iwolxvxf.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxunthhb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fakdgwau.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xersvcka.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2agvqyyfr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tiqauped.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cojhqdzn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbrlbpdf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vngkhdme.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyvednuw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ntxfcebv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bvnkwwir.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2eoaypgzt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2iteaxfqj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2khwbudqy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2yxeiuhei.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvkrqyy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2bypgamob.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nrubvqei.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zesdhgfz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2onstsmkv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2okgfmzsr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2sstgkodh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ritqjobn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvmobkxm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvqwgqlu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhvaslxk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvuraxbq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2dbtndvjm.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzvnqmsp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2inzsfzjz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2lgejyequ.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ermaazqr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mwkhzfxp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2opnbtaia.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eaqclmqg.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iezjyrrf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2bncxxhhs.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vayhbzsn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kkmqcxry.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2oodteajt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2ifczpftw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uexfoxvy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jqmtduai.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cypxbvkg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtzyntp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayglifzy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fcbydnzg.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xswnttoj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2xpatmixx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cnvcqcbc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zllwttuf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kikhyzqm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2dberwxvc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgglaioo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2llpxmbse.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2qxgtqrsl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2rdhaueqy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2aossyxfn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fxtjdexq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eviewnkm.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2psvqkoct.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2cghlubmb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vdszppvu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oaywghew.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2cvgqkslx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2bhpyrxew.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gipjdvms.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2dizutfpx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kbkekhyu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2giyjpvkb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ahydiimu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xlvlrjsf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qofrzakp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2ahdufmsl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2okemwfwy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2rnasqsxy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fxwqrxew.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fpumjilt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2cfwonjgj.html


<!-- 参考信息 -->