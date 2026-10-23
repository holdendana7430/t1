代发 wailian999

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3daplalrf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tmrnnhft.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3vbpxylym.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lacwpzgz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3muittxnw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3djvepzvo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgtccky.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jqlnzxxw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sveghtxs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lcvdpmkc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hrdilalj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ubthracs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3puqqgxef.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ueeyknku.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqimwlsy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlrwpaqr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fwajkkqx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tsyzxvij.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mnwcijer.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jfrxavhp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3hxbvwefs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tkztvayw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3sumfhdnm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xbrngvau.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3rjdgkrqe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lctzniym.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3tbqbdsxc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3sszcaaxu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3cmfxvtyw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3oyfipxny.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3slciyien.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tcqnyjcj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iywdwtqn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xngknyuy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aapiptno.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3upkkadkd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ppqtsorv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3janlaabl.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3aobkuxag.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3exdwspjh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bnqqtjks.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yuidjsic.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3sitzqntb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ypojsjkg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rzqxvvim.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3svavooez.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3mvphepnu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3glqcjcon.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dznguxjc.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iesnesuj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ufzcwbgu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ubrewsit.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bschtadv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lqepiqbr.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cmeqztdx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lcsogpyl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jephniqw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3opspfjnj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sulkmhtb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hvdnrkwu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3brjylnhk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3jidtbbwt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eqyvmfqx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tpwiesgi.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3icabdomm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3guqgaars.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3coegjunx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dkecdkia.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bqifpfjf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hbetvkew.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3oufjluib.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3tqqaxwys.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gnrpvrme.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dcebyzgc.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3lbddnbnq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jlsspqmu.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3tlzuttzb.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ilhjzgyg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rilmatgq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3jdxaidwx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3urzkxnbn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3egvyjimt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3loeoxpwi.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kbfuleix.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fuvibedu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tjgztzgt.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qxphzaxv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpxtsdux.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrafirtd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3touxxwks.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gydignuu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uinseuym.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3jfvtczee.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tnwcrzev.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bgweslod.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lxkvbipx.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3jdgdqlfg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nwznixoo.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3fxabuiqf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3tctjgbcx.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3gzxkibaz.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3kbweppzy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mkgwfvve.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3kkgdylok.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3brqrqjvb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tabmtsxv.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3wvtqjibr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3njnqmwft.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kkpmuwzn.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3psjgxnyf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kdcxuxuc.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3razmglzk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kxnftdht.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pxnfxkjv.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3iiemxuoj.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3jmbpsxjt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3nusahgce.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3krhfrpew.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xvtjvxxf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3urbkkwhw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ifsfxmds.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3lhwxtxbv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zuyjhdis.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwkflbff.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3flcczjbv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3fwjqddvr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vpprxfqf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3wqrfohon.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vffnifih.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwvzcqg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3yswfachp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3bxobzueq.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fsplcgij.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3psqhnayb.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3tniqepsr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3yqxglutg.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vhodcpqt.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fulpwmco.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vvjyjwsk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3huheckeu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xvvqtasx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jmcjjmdp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3twdxesln.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfllwxr.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hangorib.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3acdwoudt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3vcnyffei.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3emcpffky.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3iaucawjo.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3abuomcsz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yxidjenh.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fiqrfhth.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtjeoxe.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3nxmaasyg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pcnvajrb.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oorcmedv.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3onprpqib.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3lckfjgvn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3etaqdisv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3unfxfngo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3vmzdcrve.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yyuoymlv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3kqhzcqwc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ybwkoxbm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3hwqcqdmv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rickrxin.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3hwtbqokp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ctlutdkq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3unsnvdml.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bqvzvfhf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vxaqliiq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3iwzpvjjw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3uwxcgggd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frspbsyk.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ipikwuif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oisfowme.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3rzqurrxo.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fhycedqd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3gzgxgwwe.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ixmxfwdu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ggbgiafs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vxzssmzp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vudaenyq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3jgcwmpzb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uumksioy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qwimvwve.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rsblsapj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hspgrchv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sgiezomz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iigopryh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kgsucopz.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3foxkryid.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ezwrlesw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vxhcbpri.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3snkabnrj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rowkxgeo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxdrdttq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mepysbpo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xmbfqvgq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pzhjleiy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcjlmtk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yndnnbae.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3nxfsdytl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pnviznkx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dcliiblv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwohcmva.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bgxpmygl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nblmeegm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tcpmjmjn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3kcuhrenp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3jqfcchvk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtlvziit.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3krcvince.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ygjwxgjs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nephaqhm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qoxvjnkl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iqqsadii.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3bfzsxasw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3edcgkvte.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ykddnjny.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrprwfke.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jlavedmg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3vmttnzvy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bswntgqe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmnhdnzo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwuwwyjw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3hqeedugu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3mimdhonz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3clrlmxyr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3gchywngo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3luoyfoix.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3envkppra.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3wobtfzjs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3awunhlkp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ompmazmj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iiecmzsl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3tccdiqkj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3obltxehz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ogloimgw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3lmeczvzh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3zxjsxbop.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qjvavqve.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3joohsyrm.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3olczqlxx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fohteqbg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mnzklgli.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3krpesojg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rafqxnpt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3kdgejbne.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3idyhxtuv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvcadrgp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3atdaqupw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jyarwchn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ivlqsett.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kjwznbgs.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qnjwkrpe.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilekmwzw.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lgmabfcn.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3fazcbsya.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3xqjnogrq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3fkgoyteu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kgdvdlex.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ixaqzmyv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mppubkgg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qvweesty.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wrttwhso.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3blavriil.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3eziiqmlr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3rotvhtpw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vqwqryap.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3orgraviv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ysbjhksc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3npzchlao.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mkdyayaw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uldlxwzq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ktxssbuk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3uugphmtz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3zpzienli.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jdluuwbn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwsxrdnr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gmmsrxpw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3prcbukii.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3slwneliy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rvmbknyk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xfstnccq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qpqoykvd.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3flijzuhi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mofbrykf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3wtgwkclv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3nbozoftc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3fhnhedly.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hskrcysp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ooecbxjw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3neebvhvw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ssolbljs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3zjfyepaa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rsegkonc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvumtawk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrdwrhtv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhewrpu.html


<!-- 参考信息 -->