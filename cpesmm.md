代发 wailian999

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dilnyjpq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2txylzrqa.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dpjoffrr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fqcbbcuh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2fucorvlh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2txdaiaik.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2jkecbjsg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2awptxcxy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2riyjbvsq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2beyitios.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vqvpyeum.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2epwmfvog.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ogkuontq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tchycbqa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ztrdxmme.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uetoxpzk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ajldbqqi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2heptnfie.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ejnxalal.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pdtocmdk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2oivznqew.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fpkorxix.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2kjgarwau.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2oiilhcro.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jxovwjog.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zdhfpxua.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gazdonaf.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2htxrnlpu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qudxhnkz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2bjxxqxkx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2kqbiubbk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bdygpjfq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hqooljfd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xkhzlpxu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cozzjlmo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xheuxxyk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kasjfxja.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rmufmajn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2jelelgch.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xsdmwuqk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2fscwutqa.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2eclngjhp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2glptszrj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lewgrsis.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2occgvgnn.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2naujiswm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wkmiugpt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zvouanvh.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fokuxdta.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ddqeavgu.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vhiziyzk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jjghzfxh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fefzqnts.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tgezwotj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mcyogbwb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hpbibwfg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xxvsyeaj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2dhxmyhjn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2enkbaxzt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2simhfdnh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ngxatzzy.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gjujdusq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2meaqteqd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2iscucpat.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gssrqxdw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ioewrjls.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zqveishp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vkqrldxu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2snwbcite.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dlfsrhye.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2weqwhjsv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2knnimzts.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mxjyglqq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kqhtddya.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qnvheljx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nflnekxv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2lxxrhuri.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2djjxbzkj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qioeeavq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ifdkdyhw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rbbwkwtc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pkkohytq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmnmgsjb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dneydvzv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2yaozavae.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2taljyiww.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ifichgzz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqnfzibe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zucqldxg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ziyfvgon.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pfjnhneb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyzurlbo.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2wioimnvw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yempldbp.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tsxsjnwl.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2haihkcqz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2jpsmsdfr.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2dsykzomz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2sfhjdnej.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2btlyrpxy.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2iydjyhyo.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2txluhcep.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2gyhrbrzg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2amavwigk.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ujijgnyb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tmqjlqiw.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2izxuvprd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sbcojvwp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2kwiknykl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2rmuxnyus.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2abxiuxte.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2uykkfpvk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2ensussvu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2aziowite.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2qmcpyewh.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2ckpbeuft.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2tgjdchhx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2pzybhxxx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2lcuyguyg.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2lslhvtfj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2tcrulrbh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yzhanshy.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2shzpilef.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrjlhvnb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2mxbqtear.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zsaqubrp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gmmztwid.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vbpbojhl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2afoyzfat.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2sqtnhxst.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2yywexssb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2bwpwhwhh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uiakzxne.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2djaqbjuu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2wsmfpvzn.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2onzvjnnl.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mouwhnep.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ndfawdrp.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2dmcmdjaq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dvdiwcxr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2resvvtsp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fussorcd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gvzwxzic.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2xqhugttc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jsnzfxuz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jwhfrbdx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ayxcpdxs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2yilykqfw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nybgbvlg.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gitulcrs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2xkxjcoxb.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2hvgmnwyc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2czgbylyv.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2htmmhzee.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pokpaawo.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vgybymkl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ipktrwmw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjbleidz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkugeojh.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2flhtrvrb.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsvcwbaf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hwqqyfkt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gbrrbmai.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tnznodhg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2grfawtec.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ftlokrbo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2jecxlxgd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2avicnyav.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2suzkqchl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhqkesd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fzehwnyr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2drzwzpix.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2aaiautza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfdfsghe.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2ifhfuxay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvwvdwik.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lxkcjteu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2coydlxpo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drkmiilx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jpndctwo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ajmawhtk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2euwrzegi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2jujacbbf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2guzgamis.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jwtjehsz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2eqmlaawu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2jwtnkofg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucdrezbg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uaawimoc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rzrvymue.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2obocgfhb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2xxvpprbi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jmqgszzd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hbpeplkr.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2gmlenhcq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2tpguocvp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xugtshng.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yvcbwmqr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rpcavnzm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xocdubjc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2aeyqitwi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hppztfiw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mobgslob.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ijuzpreq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pavpafdo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbumphmb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2imvubzcz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2eacsruzx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnoyutdl.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dnmsjvpv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lipjabyu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2przzqcwt.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sheivfgf.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2eguksnde.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffitkfst.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2vqlnhrkx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2itgaccyb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ivziohtk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbqfubr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ywmthdhg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ubocqebx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2rewfepbk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgwevub.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fpuabcqy.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xkexvnak.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfaterwk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mzqdgwqd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2yopndygm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ebeogzwk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsogqwth.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ikfbfxnc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2oyhayvdx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2tceqhkho.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2affhfaxx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgsviptk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioarjreq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2fadormva.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qpconsrv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kaxunbhy.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2auhboptt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uynddsrf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dxdfjiyr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rfozqnpi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xgfuwphz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nwuohknj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tmejgidl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2vhkeyyoo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2codatqfk.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bwzylhrl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sykyreoh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2axijingd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tzccbjip.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpsegrrr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2guqzgdft.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cdbcghat.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kvveaodu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiplkisl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vccihvym.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cttayndv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjamcbd.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vktjzbsb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2fholpdhd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bfznlrxx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sdassnzs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqbllsi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2iutsmvkm.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zscgisjl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cokdjwmd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vfwgftuf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qtewishx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gmdtvheo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zonkayqq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2uplpkhzw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sobiwiog.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nmziglon.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dmudnioh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fvjkoavn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2eqgxjpun.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jnpnoamp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kzfdwwzt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2eimxnzrf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cqjzlimf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jqrfbsri.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wefkjqrj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jkeshvja.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zrzllhft.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2suiferzz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yefxcmaa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ammcctvz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2apfffggj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2zgiasfek.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lygtvmkw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cnhmsddw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mrlhhblm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ulnilmhv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ijcirfwj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2thwzdugg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bxfjqfrl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iaoomusq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lfwynpnw.html


<!-- 参考信息 -->