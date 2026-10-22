代发 wailian999

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2buzihien.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dnlonxll.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2dyflgdlr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qexgopui.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iwkesrlx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2trzpjrbx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2qdrejfkx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2judbqhwr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2dejmcdui.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2honrhyit.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ssfepncx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cxkplmuk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2selcwcef.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xxivwjqc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mpkwekjf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vzxwdjti.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2waqothgo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wehpgjzs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bjhuradd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzdbpwgr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2etihklcj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2swtdkvml.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jdmvlgxw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lqsapxlu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mlduzdcd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ikkkwxhj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ddqlceyk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lsibkxrs.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ndfkhztt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2okkjpyqj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2isbbyicu.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fzygamtz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2llbkzshv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cysehtjz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iyozuyff.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dozpxgyo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2muiytgbp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2yzvctjnv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dkrdgcbi.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2soywiekv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dsqulsaw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2stzjwuxd.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cldrrqbj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2psgqnjps.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xeyiztlp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iptyoeph.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bwjluqho.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eqdjzwax.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2srgawsmd.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2iwrwkyas.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2brffzoul.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cnwmwkmz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2shfesdbb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uhpjzfco.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xbqcajvn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xlutfzdp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2kwrmtmhl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2jrhmhvqv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wdibilft.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdhlmxhn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2oaaudnuq.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2lwkwluah.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hdzaqeqt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2eiqrcofr.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sufiuqyl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwcgvkpd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bzannfin.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plylmzpa.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cluwmred.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kmakbowv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aiscjihj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2azzhboee.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2uqnhxgbv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2jyrwhdid.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2brgomsne.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2usihmcim.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhyyfux.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lbowcaea.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2jurwgppq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2dlxebmfc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ljinuidg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2eowdrvef.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2fjbhrzan.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jalkzdzc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dhutddfe.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jymuvljs.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2wpzaazsv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2eobmyncv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tmllawop.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2catsomvf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ljjyryti.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2polfmgfs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2byywtime.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2zoffqjwa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2cxrsqgjp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2shvwqirz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2elblfbcq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2kviwbvqx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2felsujlv.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2obccxkom.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihlmrdgs.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2rnayhqsw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nrucjkvr.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yitutqsz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qzbkltwc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ntvbmdwo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2afdfhdfb.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2predaizz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2icpsvpfy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gycpoprv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2idsnfrvg.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2mameqzhy.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2iohfdaox.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2koqzctrq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wkedwqvk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bchbqotg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zmtwbtxm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jrzzqucc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rzcctfid.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tstqyhzc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dflfcfrt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bssnkwvk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gprsahqf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkpcgdyb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zaihkacw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2myqryimy.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uuxrhohx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2qzytfrzk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2jnjeqcyb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pyltvaan.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hpmdwlwg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2htijfdsw.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqxsfnur.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ysbhperq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dyozzczx.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fxvyykiy.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jreavoyf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2qaqqfveq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2slmmpowf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccyalklw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wyvnyenp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2unyrmfia.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2anunqjee.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2tsudphsy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yfnkpeiq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hbiiwbao.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ynkgtkou.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qyvmscqx.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tyqdixjw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xzcuumbc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zzhulamu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mzlgsrxs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wzyyheht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmrxvcfy.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2kaslxlzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiwfloqs.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bvznbsgw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2aagqvuak.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2mfmqurhr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xxyvxpws.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rqfndhhj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zciywcyl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2fehqomhq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lbykbxca.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pfdrlfuk.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2heophvjf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fmywlpwp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2vvizlvsr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aqqppzst.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wvpmartv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qbgwwerm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2hazqwduy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2guszsped.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2meflkmtg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2oltyobcd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ncllsvib.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itdvazzw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2uwfkmufz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2iavjnjmz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2altpzwra.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2jwjrnzhx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2vzhqcnvq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xetxhjeb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xuujatlc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qjsjknfm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pccwkbxz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qixrsmqi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfsbyymg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rpbevlpe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2aqeilpwa.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2gbnzpaod.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bdzyrksp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gypnjslk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2qmmmrtje.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2mbfoijlf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyecyfhe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fchttcdb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2uammnfbq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uxpqqpri.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2qmazmrtt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2pooptenb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hhddpcof.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vptuqrke.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjwwzvat.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjtwxmqi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wtbiretj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2rsouardf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2mkfkjdbb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lprcwxcw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xcqhbeda.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ksztzjrj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oikmprhm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkcgrygo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fcuqvdbi.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ihblcogg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbvkbbni.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ahpfgzyy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2oxtqhinb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edorlbnt.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2evphsvpo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2yvjjtkil.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bbtdoqbx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zsogizzz.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dgvcqzgo.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uvmrekoa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnfkveq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rlvpfcdb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lsswyhqs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2fzhkgkzf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nowklahi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqlmvuh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mmjslomg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwefkaei.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lsmjmfhy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2axgdykyu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2voiiizfm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtpttram.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zccjlqxy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jaqlcsli.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2intnqgdp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cgegbqdi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2spidrrzp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2abmmdpro.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2obmzedwx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xntzvtyw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhanecuj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yudcglyp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2vluoxmwg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2quyosmnh.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kurqthtp.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uhswailw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjwplamx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2aaxvnbkc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2zvybakmn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2cgpzjmcd.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vbbukwfo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xaqliaxf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2svuytpzo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2klocmjgt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfrjlubc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xuvkshzj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lwmbtwth.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hhxsyipa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ykdowyfs.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2llprxhha.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2amnwkdsb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqexdvrh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjfopfaq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhttlhlu.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2twwndcja.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lygjswdd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2pgubtazb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zhwycigv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2mqshfytj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2edihajvq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2lteokggu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrvugpl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aurwyvqb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oedmhbaa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jbbqxddk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtmbktm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwlxryy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vkvzpkya.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mqtfeptt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2erevqfja.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fxviccdj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2thfiokot.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zehxawlu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rdnlibvm.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kbnblcyj.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dtavpfux.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ohdjceet.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2vvxmhhne.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gueqsphk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rmbspals.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eyvdqqhu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uiizghbx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iyzpmjil.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pgkryylj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dcnoucnk.html


<!-- 参考信息 -->