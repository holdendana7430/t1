代发 wailian999

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plndzpjk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3voplwdyp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3fcdqmwli.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfhwdmso.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3sdyjpame.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ulxrbyrd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3vgpjxyuz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yxwiwbnr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3awsvykrz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3npqastom.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jeybsuki.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3msschdsk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3etkopunj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ijbdkoij.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3sgilfyad.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yywjchxv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yjgeaurx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3syhdfdrs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kjyoenfh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rnyywsmb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3weuihuyh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rghafetv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ljztsuti.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndifehod.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ejlswxmg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wylseeqf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iobugafd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3iyzbpyfq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fzziiobh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fwaspwxl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cbriesdq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3goezaszf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qipuvkay.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tjiiskam.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ldxrbqmq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tkkjnmqi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mriemftm.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xhjvyhlb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tbsakelc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rdtutvgb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kxnatklf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3tsmxjflb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kwelgrym.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ggefjlcx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qpzdwgle.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3idfcyteq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ysrociob.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ukacfbun.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zsoroshe.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3atgxcojo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3avzyisye.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hedgfohf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nwmjzmya.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3keckjbci.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ksrntiet.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ollqommq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pdbhevhn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3mlfevcxz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ievlknan.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kmavhzav.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3frfyjjiq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3amocikuq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3dznddkwd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgtbpswt.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3pskemnhn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3milxnsoq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkixgirc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3gehegdbj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bbyyjhxp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3okzrburj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kjicdowf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvatsrmq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wwmchcfe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zrryazfp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3puwhuzij.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oppvvunm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gceroewz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ieoewvez.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bqkrpruk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3cflhxjee.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3gfrypqye.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qhswwanj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3zvghzfam.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3gdsrxzxv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3vbqyvvbs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlhzyspf.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mizbkiau.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3pictndoz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3htoyjird.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3paqmihgx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3dkbertwv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3odlrocmq.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3bayxcaan.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3jrjxzsvv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3trlbnmzg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3nzxqcsff.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3yxzhkjup.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cialocbc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3aawjomiv.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3lqbirkqt.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xflfvpxu.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3orxyjvgp.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3dmletqtr.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qvmsjstn.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kaagjhqh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3irmiyrif.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjfifet.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uhdcjpde.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3riwrzfvh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ppzlmnma.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hnapzbkn.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3jiquahxo.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3omuhpwse.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3mgabapxs.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3iwpujqsd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3vitnjegq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3iockuvnb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ibmhpwyx.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3yysfxdod.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mhrfrxhk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3yxqjedzq.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ejgyzria.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xvmcgyhs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3gpvhfcrf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hznhvusn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3msmrlwqx.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3juosgtob.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jzbqcsyd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bkjlahpx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ytygyjsa.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ubmuhrur.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3xqtthmvw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tyleiakp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3fvytbghv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hyobdguf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fzghglxr.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3grxfvxzp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ciofbbcr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pkuclypy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3trkktqfl.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3shnaoqzj.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zimumxwi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3aafxossi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpblzii.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3yaeppncp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3osbuthvl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3blpyhgau.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3phjcnuxn.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qqspnqcr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3vfzboblg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3hhblnejq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nilzadiy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3fhcuimva.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxynkha.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bpkgnlwr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3fjlppiyt.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fwtotnto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3malscjmv.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tjehcqon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dasotmws.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3qjmatrbp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3iuwoonbl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgoklru.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mdxtvcku.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eoupafmf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jfnkdbti.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wiygzdpq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3nlmnrvjh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uzubqucy.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3jvooyypl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jvlcyfve.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkrvpqie.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cvgszvgu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3dgttawyt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lykzseak.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3cjvkzfap.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3gmtknyxy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uifxasgm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3nvnjqiil.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3nidsylkk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3itycmjzi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fjcgrlik.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owlmonzv.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3cgpvhszo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gfqpxsse.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rbfhhtcj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3rnviyqje.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jkrxikeh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lffifinp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3oywyococ.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3itfnpasp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouuwotki.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dlhuaogh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkktaq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3jtsyeztr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxjhlbvy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3eqooffqi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ejwxzlki.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3acdcxjlt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywryswtu.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3snidfaby.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhblefne.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dyjwcbxh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3iyrzpfst.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3zpciauhy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3kmotqprg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hgfkdqdt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3viusuylr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ljkvjnbj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3oslbhedm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohporzvi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3hyxmnwtv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qfhdoogx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckpfnovc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mljnrroy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uzcsuwgs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlyqwolk.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmsxuyij.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uqrhowik.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3trtvobdb.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3pozgcrlv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ixkpzebb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzectvej.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3egbzuens.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mtsjrsfa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wwfiywmg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3niuvbpyh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kpcapqne.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fgggieik.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qthpfkxg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3uunfxugm.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ezfytrrt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3pinowpvu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3tppkjrku.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lmgdgytn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3eibcreew.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nivxjvdr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nuknbbmv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3pvfxssni.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cfbdomsz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugqwfcll.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3twaosfzf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hmrbrrcl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3idqpntmv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yqcucpfn.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ygtailbk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ttcyxgos.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gcnvlfdz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sxojqjge.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxwshqmq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pxxhhmal.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3maplhasa.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fnvywius.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3plhqjkpw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3jnebawab.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xxfcbwld.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zgkbxxks.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3qvkamlco.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3pridsvxk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3wnxpykpc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3kgoqsfdq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3puxtntxb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfrfofp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bzbcwgnv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ddhtutye.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3yavylcqz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3ekisrumz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xqwlcmyn.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vdnnkqlt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3dpqtpbjx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ddqbvhrf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhghbipo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmqbqoex.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3efltzjwj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3znxdjtuc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wvutdnah.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fhtrcigm.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cdeurwqx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3djnmyxwo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jeelltpq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bszyfjhk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dcpmrbiw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjfjauls.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gasbqwyd.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pajuvsxu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ibqhacuw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vxqjlwny.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3evdhlzms.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ognoggak.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nsnitiyh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jktdmkec.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3urmmmmzl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xkdyrxqm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wyevksuf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qhnarbej.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3zfpfzsms.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3kzejccjk.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3frkymsig.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mqgzrkcn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3wstvchvc.html


<!-- 参考信息 -->