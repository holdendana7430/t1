代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gtiyfstu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tgheeihh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3yorbdpia.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3aynswkgy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3apwlufwd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jbecwzml.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3sysqkhzq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3sbjcrdnx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pycastxv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mljivsyk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3xurveizc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3gkfopnym.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dbdsjnfz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3riftmiqx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3plbfrpln.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3trojbwzg.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zsgfztvy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ndkknazq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ljmmmtwo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rhplhsfu.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3xzseumkl.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zwstyprj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qtruvrdg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3atpkkocu.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mzzfkulq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3spltcvrr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hrnknjqa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3pehcnkvs.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ahgnyvbj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ypnluvrm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hrxazqhx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3andujvuu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pxdyafsw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nnwwfxjv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3llywxwcs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3howotexy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pkhsklfe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vkqtsjlm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3qnqcjjfx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mqhfzxpa.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3fcxtznfy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3jnvrkkan.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpqvdtzk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yespqvof.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3vgosuowl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3hnhcmcck.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztpitdgq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3dwfrtzks.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bpuugzuo.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tjescjjc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3iobwsbqj.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nyevyoch.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vhzjpebc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xtnlylbh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ikxowklr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rxoajvaa.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3fmweaumj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aolvmyun.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3elqcutkr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yeahkaqs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3zoorxzuj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3wigpegvw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qkhiwmqe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cjzhwavh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3tqwghdiz.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3otepyinr.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ifkbxkdb.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3avhjuhzw.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yoqtaidl.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yxvpdjxk.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3hlivmtqz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qlfulwce.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3wpbivwbq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3vuvyondf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dazlybfh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3odqgjiia.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3uesjqcvd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3gnebeudq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3gnedigna.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3lnmnqxur.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3cokorroz.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rvnuqrec.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3timvtbrw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3qtnsyvam.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3gpvakohn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3orviawfg.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iiorqcqt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmswodzm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3pimztsfc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hjoeifld.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkddtoo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3npoequig.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gwmjpukn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3jxwlxvtf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3omyxhbib.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3wjvhegcw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3sctttepd.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uvakcewa.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3warrkrht.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gnmnprde.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bxknqujs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3orshtfwk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3juaapdes.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3cjaffqgu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3siypqnhw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jjqahvsz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vlftudyl.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3btwxdqar.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zftgjdnn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3qddzwqen.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wuclqfxs.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lyqtsojg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3kqlsopgf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3eyesvyep.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ppsixihj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3mibmduhs.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3csuzsvrr.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3ymwenfcw.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3conekkac.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pwdvhpmd.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3usvbftwv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3rfojmaoq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3rdilhiqa.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3derruduq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3slgymhan.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3guooljzl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3psgmrixs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nbgfdgwx.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3nayrezhw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3imuctjlb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3bohkgmru.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3mqvvdeoe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3stzxrbtz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zsiptqlk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ebcrdbbb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vkdxhczd.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zlrkdthc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blszegef.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3qphkvelv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrhihtsx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3syuhvrgl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jmcnmpxt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dbazgvsh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qtliouor.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3klmhdnpz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3cgpacfku.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3smzyexge.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3roogjzsm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lpxlifee.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3umlikgzh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3rasrxxfa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqriquue.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hrvumrkq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bqxvnzao.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tovgpboi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3okhenunn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3dzhmlcun.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iwcrwzlj.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3gxbvnosg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gqjffjdk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nommjulk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3fzhjiiyv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkeduzee.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3yfwoqtcf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xbkuzjuk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3sedymltf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3zhachmtn.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3sagpxoqr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ixsjzdsk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3gzuvcuin.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftkfedqt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zagyswmh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhxtxmjs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3xpgjeuln.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3smocmhlv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3sloaxpqv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vmkmflvv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3jdnsdogs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3izcyduby.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3qvtajqun.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nizmwjpd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzjcwwmx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3oecjladh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tsdocjbd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tabkvlud.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zziqxuez.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ifeibweq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3eatgesbs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ehknzhyc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hdeagyok.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtokrsk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rirpkzvt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3qchhctto.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjijjyvj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tkgghbiv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3cdzhfkws.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3aalanueh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qtvfwuob.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yowjrwop.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eedjfjqi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zowfftjo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3nqhznklv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxhajpz.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ocfagkor.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ysqlvwkc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pxsnxhhd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nikcowqn.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3abchletj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3msntkpwv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3srpmrivt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3nhfrlykf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rmydhamc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jnusrqkt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rcffirck.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oolvblgo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aiuiljnq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qstoiexb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayzagque.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zlfybopn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvinoawd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldebkgja.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jtwvggcl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qevsxpfj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmzktmjx.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nqfiqyor.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eioogmas.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3muxxakxz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3huazrfso.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3fezvzxgu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjmhglwq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hhttpjti.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3eyitltpy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kdjohujf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ymhpacvr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vtymbmky.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wyxljbub.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3otltitjr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jcuvjlws.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hxqnddek.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kvtydrtz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3bejtrjdx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vnkoqczp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nqvcbrgl.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3icylyyhk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3momhznfh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dcebifvh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wsjrelmq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3zoffqkye.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mbmpfgtt.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3igmcqlvk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ishdkwya.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xfperzft.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vauyubjy.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3buukgfqy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zmaxvmwp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jgltphqt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3fqknywhv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ldccitwv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iurfykar.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3fdddvyaw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aifbtann.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3djyafysf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aknhubzh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3zflnatid.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yghtedev.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzfhnzpk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3yeoaqojr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3hszroerw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3gzuoctmk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lovxevdx.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kiearzid.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gwtxtyyd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3btcvowzf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nujozdrq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zdjbhqhn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3dclgmuxf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3nfspupxg.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhsonqsj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dknqwaqn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3efmcwfdw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jlxbygny.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3goyxisxj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3sfrxgevs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wwmukjed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpaemqmk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nnxyhibk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zygeriqs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gbpmtasj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3utrqwdqm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oivxdnrp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewkjommk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeghtfkc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3snwcqrrv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rexxwhyf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ppeqjbmi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3etpryhtk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjmzthwi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kkdmides.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcpxnrkv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxkktokd.html


<!-- 参考信息 -->