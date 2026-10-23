代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kzcvvsar.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3oikjyndn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zdyjpkvf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nbgwsgvs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3omwyzntp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bsbobfdm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pypibice.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wkvgkixj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wbpgzqtw.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3irlxdzoz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqreqfq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3mezinqln.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3javivmxc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgbtlvu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fecopwnv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qsfmzpti.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3otijkizb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nnewnoqi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3leikekyl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sdytvvih.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwxweaej.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ngaqbjyf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hoxpphwr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3niryiguu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jabkmcmt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xwiaqhnu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bjunnklh.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3bonbokrp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wefhvzok.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cnruzzdj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3minvwhpr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcgwcipc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mtnbhhxk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rcqwgxdo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3hadeoslx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hurjctvx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fsazcspc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lgomvugs.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3iuvyybuj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lbwuhvje.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xtqzjlgy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3brkomfqy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3rophwvmu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3pbfdamwr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwkeiqk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3bxcdvkoa.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mwuimkko.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3waoqfdgm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uvlryetr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3upisbehc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3drjzxepr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3enhbuodu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ysftsbqi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rkgvmlla.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3bxbxzlim.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3iigxnvla.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ljwpzeca.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jzhrcjns.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jvnozrmh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3oiydxtsa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxfxbot.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pyqiylze.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ffrsauay.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rmvhxlfg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iyyesott.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3sfmxhwom.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gxogwauu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wofawfub.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3krojamyg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mutydccb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vhjqkfpp.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jjgkhzri.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jxdiaqia.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3xnvqluxu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pntjyxml.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3taqumddu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wrifqqaj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wnxrpkii.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hfdgbyiw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3olejapju.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3elrgbupa.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uvzvshbl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3eibphddw.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xpfknkuf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qegplyvr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bssejtlh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3drjnrvfq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3sgjmtsyf.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rkjpgfej.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ipmfazwo.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3vdcydvob.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3dbmgcrmb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3jzafyaar.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rqcfpdzv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzxwihkl.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3qyswsbon.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3iunyatwb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3wufvdxjm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3dajhoymd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3elvizelw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3meuxxhkr.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dunvusaz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyqxnxdz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qeyuzcvb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ujfgfltt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zduhlmyn.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3syhrcddz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jicdelfe.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3bbxnhgkp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3uxsmopds.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tdbwrekj.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3nbrvdqft.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vtazpeac.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3slvuymie.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3lcyrcfta.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3rnptfboo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3luyjmtoe.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yrmjfdug.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nonplbmg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mewgrwjw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kdlzrmpg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gzftwnuh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3alaodzqr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ktuzdeph.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cikqrbkh.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3llwvyyxe.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3uozhhktb.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3kpfofwpz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3taqqmriy.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3hqbledfu.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gxvhptmk.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3aecknubd.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjcqrjo.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3atwkuhec.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3roymzytt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3uxnjxhyl.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwmmcgfo.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lpoqakvm.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vjrlnygg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3qyfvmkew.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3yiulxkmx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qftqlrzs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sshnmqzn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3pdqvdadt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kvyrncxp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stcrkqeh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jffvkaui.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3hsxlqoff.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iidddkby.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vhhfvioh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3szeexxrs.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahjjplvr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cfrpkhls.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rzsrvolf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ovgfgyaf.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qgvzhler.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3qthryusi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ntdyouew.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3aqndnrpj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prkcolld.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3goaogqxb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3hvygcplj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3efrjpbuw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3owymsxps.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3bjqeneoc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xwzntune.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3qtotchji.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3tfthsxwh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3umqdpoai.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3lvxuvwom.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3lsbugxqf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bjgrrcwb.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ryosnwtq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3fsctuulw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fspninye.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cydqkevx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3udcwbnsa.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vxbzutct.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3noruxxnr.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gyroxdbw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3reniovrj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3icljmgia.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxexadd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3vwschmjm.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3lsptvrcx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gcaagnjg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3kkcpervg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3fyfxkpkw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3nkyvsewd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zezazroc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ginogkkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdyawixb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3tpxqhitr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ymonmvwh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ffkvzosa.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3msxpvkwb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dqxzqerd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wxnoeeqc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3emjmibsp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rspsyvya.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vurdmmui.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pbfgvcii.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ajiyusfn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hiryzsnn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qgnwumqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ptzknnfe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ggcxceoa.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3lrnbcieg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3flcersfo.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gjnkfxdm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jrrqkkrk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3izjtxokw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wikfejwi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzxwzmff.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yojtjunp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ofluluaw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3uvefsyde.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3umivubyc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3iguytqen.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zlutueto.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rkeowdpj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ystbhvih.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uigadwbi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kjhyaqha.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldcvzewi.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nustvgln.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3euejydvd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezbsgpdz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wrfekswt.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3iuwumfcl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3dlqoecme.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmzosrxb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbroylzh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxdysvqc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yiphnjsj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzsrvil.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxuasihg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3gybbwiak.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hcxrdnoc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwnsvszv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zbyibpdu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlpsrfku.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fegdwyqo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zqgtjrxs.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwlglhe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqxvkspx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3thvknqrj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3daahsvkt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjjjhsib.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hywyvevo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kqiiwczx.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dchcaxok.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3cbkqvgut.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gjmmjfoh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3unumxlhn.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3eccpowfx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3qjbdahbm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3afzinydp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vvmsshmq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hfewkljh.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jpurylwu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gwphajoj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3alyoouiz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ddrkohyu.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3zedqznvt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3lebecmrh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qjewdyog.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxmwoeml.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lukeytke.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3raezegsp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ywwqhnma.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bqyrjcss.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsvqjatt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3zggwacnb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qtlqgxaa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrpypdqc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3tbkksbns.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wcxkrjgo.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkfkijz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3asuqrcyt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3avzcksub.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhyisfek.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3nplvkojj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yhhdxdkl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3roniokro.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqntuoh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3znssodqy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kdezqugp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fuywjppd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gqetlrdk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3kotnnrda.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jfuuckdv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fiingdyk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3qesocmzu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3dqsehnwg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3peuhydmt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbmmrcll.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3eusipoan.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3niistjvc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tsahlphb.html


<!-- 参考信息 -->