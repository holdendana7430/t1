代发 wailian999

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pueznvcw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hsitpvda.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ymcanfqs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rpxvhdgw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dxjuoyqb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2nfdtptth.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lheuyxvi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbqayha.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ttgejfnj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ktplyqvo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yzjmpzhq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2aetjtjiu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2vvvquafr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rncvybgm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qnyomnlf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fedwzncq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2qkwnmthf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uxswahuj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2tnajiiro.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fjvfxdhq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2phtppcvq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jvqkpxxr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kcedsart.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qcwsyuge.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kctxqfqf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmzbgbmp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpvgaub.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cljqpezd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2crmbmrmu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tyzsxkqx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ewbkrhbz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjswfps.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hlwbbgnq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zdlbyypz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2radznrfi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwpapkzd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2grmhjgvp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssfbmmby.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2vmwkdlil.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2dzjgsjos.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2aggwzldx.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2jksnbtrv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tcnpxcva.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bykgtenf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mwglusgm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hjzqpsfo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2thzufwzt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hvhxqakp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2crodzjab.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rlksspbw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gomylfqb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kddihhic.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2lhkipahy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gggsdqdc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lvsullsa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2olpdxdjy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwuqdto.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bcjpnowp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2supjvtqp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ytjessht.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sicnocmr.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zzxufldx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rjeeyibc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sgbtxwme.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xcvhfxkd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xhdmfvfs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ydvhqnnj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2muytsgoa.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2dbqgqfjk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xuiaojje.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rhzevcvf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jlpagwtu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gmdfakvo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2byslhnud.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2heesnbai.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ilweirlh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gdajxmso.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2yerdtwgb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ijywpsmz.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dylvuhny.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jlguprjh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rxfixbpz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2lhmxtqck.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cofdlijm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2daxcxexm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hzraprup.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xkwxciaf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2uvjwjzko.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fodhmhaq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jegrpmsa.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2ogqgrwde.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2htivjbth.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dcswutqw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zpblyoix.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jaeuewyk.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2nebsavbn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hxhjhmzk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2rjyfmtqx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2edrlxsxu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pobimnhx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vptpcpwk.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2nxzqwlxu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jknrseoe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2okfvphhb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ddkpgebd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2unxolmap.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2muchvmgb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vwjycwli.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mdjhfzso.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2wjssblqj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xrnkefpd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2lzbjkvxw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2jvvvjjub.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xkiprcnb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gpacylay.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ljwghwjg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2cxgttzqr.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2mgqksjyw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dglwibmt.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bnzrbwwt.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jzcqftpy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2nelqlxmz.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2knqvnaxt.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrgcevb.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2tdwinetc.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2khvnrtbv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2mdushoev.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bjuyziwu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2lvisstti.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ovnrjybx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2cojdpeob.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2jsunuyix.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2samgnzph.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2rpvbzfij.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ndbvbfta.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fkcekklj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ermtthgv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkohuad.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qsuovmar.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dujzleca.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ejufvpyp.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xhrzezad.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cbfinczs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ltmqwrap.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nkzezxoq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fshguvbe.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hlwmhxbe.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2occrcgav.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fkygjwaf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qinumfad.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ssdohfan.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ksobonth.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ogtbqbqo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lcxlywuh.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2rwiptfoc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hrbmxxtb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2phnxtktw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2uuffbuce.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ufmhvzpq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2waihyojy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jnysyquu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wscbnetg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ewnrblhg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2pzsbscxy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzfwmxhd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2jraijjht.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2bquvtouo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fikhupcm.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qunfpdod.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2vuqsmypk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2nnsxcjab.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lvokfggx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2esybkcpf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dotdhbgr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pwvkyrmt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xzprqhzh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wppissyr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2fbivyaho.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2dzoesjyi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2exshfhmj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2xorfswks.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdwthnj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2liocoeyr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lifchvpc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2pbqedgoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxdvxkks.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pcafzwpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzxbyvzj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2oabxoeqo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rwhstknh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrwngyho.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jskrbbca.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pddnsxxc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jrkdpvrc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2mryrydzf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2isteriah.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ghhlnfen.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gvrdrjul.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2lgzcwtcw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2ybdgbkke.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vcgzjiii.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ddswnfba.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2oyimwfdd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uzpakdec.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2avkjqaog.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xajclejw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nrvzsriz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ibfxhxae.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjzahjq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2enbnpfuo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cjrfakvn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvbstric.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdgjklzu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fyonpcpg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2delbadcw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2rclqtjct.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2roshecnr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ewktfcry.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2nvpwnnbw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2utozprub.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jfvtksll.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xslwrnrh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2aiwwhkjn.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mzjiivcs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sqqgxaba.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2lfumwgsb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2asjtsqxm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sldjuxlg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ksjqocps.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsytlctc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2winjrhtj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ewystlii.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2vzbhofef.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2vzickmzp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vyyaopch.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wijdtbgg.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fktwigjr.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctgcyssq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxetocgc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fpjgbpiu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xgyffvzp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxvovfd.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rpaubdlh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tohpcqec.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2khhwxnxm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rtmxkhpg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zyadohsr.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iqzmtskp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2crtyxinv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dkvjipnx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zicvnxkv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pstqhmhu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2phjlgpok.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqdsyztr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2liuphyuq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sfodiatm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgsgodow.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gprxqowo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cnzxegwb.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xrailmtj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2balgdnqo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2esjcvtrw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvkqpqyh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nunmutoa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2atolkhii.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pevbrqrw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ojtiknss.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ftzzjdyq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wbyuxtfs.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2inqzyobl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2cveonniz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2gmdqdiaz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ifyagdcd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eaoecxac.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2mecrjugb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2aimobqic.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wxayhust.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lehuyauh.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ywhgpvht.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xqhqrfie.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2chhsubfw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ewbyogpf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2yjpbqxsb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2twytzmdt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2lggnqhxy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rmnbjnfk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhyeinkb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xdrmnlyq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2iyxnndvt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2ruhjoggh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gftnygws.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2smiecaxy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsfmntxj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2epxoxyow.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2ichobkcp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2juvvkeed.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2itzihcgj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2lhxdpcdm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpapxkej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jibjievy.html


<!-- 参考信息 -->