代发 wailian999

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxpyihx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2wtgppxtd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xcdqcceh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2icjwhgnv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmgtaak.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eyzxapzu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kgflrirq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gozxurvo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gqrldpte.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2chrcrbmp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2miirsytq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sksgeflg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fqnfnetn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2xdvzrsmd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2vmwseyif.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xczluocw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zukyults.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xrjfhpsq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xisxeztd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ogmvrzat.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2piojhblr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dqzeubqp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kvqtpuit.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zmlcfach.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2valwavnl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2emqmfyfa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iymbgcjm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2rnhszlds.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bvgilhlk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kicferae.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mutaoujb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2npaeybzv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mnsnrzuk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nixqogyx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bwtdfjzp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2phmpttsv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2mxjhuqrx.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pxycvfzf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2nzuirbjo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2bzadmzno.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ersrfqhs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hqdvngjy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qijjcujc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2knrdsetv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mbmquryn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ruaaamyl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qrhiwwsv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zjkcgxus.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2lfbtimmt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2alaccmzv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nmbqbmul.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jjscmpzn.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sljtpfdx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2pgqbtigz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pephqcvy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ulgeczfi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rihelwdy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2obzvnqgx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ogniusah.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2potrtmnk.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jylcmmty.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zzlejreo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jhckqadz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2pjxravzs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2tndrthkl.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2odlvtiaz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2jrijrigv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2nkmhouen.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2cdstmbmi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2kwsikxlq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rituwgkr.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clrbaxsu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gcmffoqu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rfexcckm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlsamuro.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2icbfdhcm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xeubuilc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mrxwzljz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dsenrgkp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iimkkjgy.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rudmczmq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wpnfnwlj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zcidhdru.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpbpyety.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2cqqonjvy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vqqeebzd.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2faszusfo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2szgkoynw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2bwitxuqz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2hxzwelor.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ohcbistn.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2efzpjbke.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2pyqjwaqx.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2amvwrumk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hoorpwfr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2aqzzpbqt.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2itxdulzy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rpeltala.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zjptnqgp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2zpdmsmbj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2rddfloim.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2vwouxwvf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2yhgvkrgj.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2jqkuiewe.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2grvrduog.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cfjswwmq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zaieyccs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2iooxtqms.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qejidefz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2cnmdeaht.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2dgralrtm.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2buazysng.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2gevjcopg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vltgvips.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2axeushov.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2eqjozkto.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2pzcpcegq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2amculoec.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lddvnuzn.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ysqyxrtp.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwofxiud.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2silkgahr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ojfqnfik.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2xkgmfrth.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2memgmumd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rwcglfgo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2vtqhltml.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2okylwspx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2yyrolzea.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ntxuepsy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wikhixrm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxsfxlvh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jfidyxys.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fdmxysza.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nehwlayb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2auidxjcz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hucxefsq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2eyrpdhwf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2geconyxd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2zglybfqe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2fosguqnl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zcgusaqw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ugizdxvc.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hcyuvtvg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwzonhg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zihhbncg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zqdsurkb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vzcmazow.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2qladushn.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzrxtlyi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aojogkhq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qehyaxho.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpdpen.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2djymvlcf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2arrvkrob.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mzhilirl.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2krcjdrrj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2cvbqvvds.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2hdfcdyrl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yjljykbi.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2yuzubbvq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxwwnhh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2hgclzmtg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uanpqixz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2isfhbjzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azpkqvkg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cptmblmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwtkpdmd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dsdpnhfq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2kuaqdpml.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbshkwdb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ionunkog.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cywfrgzz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2noouovyn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2sylfuqch.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ivriwwuy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2mqekchxi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xmgnulzg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kginnxqw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2fzpbrapg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mmuefuri.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zkovecxj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kkvnoqmk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2upprolmi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2aupgxffq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dnonizma.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2asrxwntw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2badcrvfu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2axxvlvnm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szutcncf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nilwcwqe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ijkhcsmp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hghxjrln.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2puyejcbq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ddnboykc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jsmhwrtr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ucrdphsk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2jevwmdkn.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qluzvukd.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2girnrooy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gmggdaot.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zonkpniy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2awiorijx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqqyygia.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zhtyhvqn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gfqeevbv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zsaaeiqb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2exxsdhyk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lalxsxav.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmpfsop.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2ukiajdcr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2gqmgzbfn.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2thrgcylt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2yqfjhaiu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2fkikruor.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vuipwudx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2trezxdwz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzcxhnt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2opukvtbj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2gauxcuqu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2almptaqp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ernewchs.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ksavdecb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rachohnf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2qepkktpe.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezdgofyk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqubmvts.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drkuliik.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2aisxvyjr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2twfafxrl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkalpgqo.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rpbyhyvy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2brlzqdzc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jbtbralj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yvorzpza.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ykzwraxj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rpgrvffp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vmcuapsn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cgtjotpu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rvkicbfm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2aitfuyqd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dfkjclho.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsbnultr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hpscslif.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ypnkuqsi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lsnwvzjw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ayowodbh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2cdaurbxd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zeoeynoo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2vicziawv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2pliiahqp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qajozllx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2esiqnorl.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jidghfsn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2haonienw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqmzjhna.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2shiovbxv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fookykxk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ssbrxcbr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2kthcbbzs.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzkrhizc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2eskglrvy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hsuadlwm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ekcknosz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vhdnvszn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2uqxvwbpl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mdiwzakr.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qwhvreqx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mcxgvbpm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2umjkazfw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2efwbmhcx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2klbchqsu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hglmugrx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2rqaxdwbn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pjhujuzs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hvwwmyxu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2chgpuabr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ixooovgq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vopmeapy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rikhtbmi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pqcdkshs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2hdqpprhw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uviqfqio.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2giugblju.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kqmfdbjh.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ehavfygj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hdeumyhw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ygxbkmsz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrciwme.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2myqifdvz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cigqmlxd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2dthxoltd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jvsrbscw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yhplajcl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ycpesiuh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ojpwymeh.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rtrqwvvg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ljsjrdzm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bazqyzix.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jvhlmxoi.html


<!-- 参考信息 -->