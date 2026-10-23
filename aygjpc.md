代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3pntmdbzf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3woqqhrsc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgfrtoze.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hnpgaffo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3yefqcoqi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3dyqtqqdq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zodztlam.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3nmzssgqq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qwkfykag.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3skkzdeqo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rzpcwlnv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jbomqdet.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3edhljzrz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3vywsixli.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tvwbmkoi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qwotxixi.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3cakbyblp.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3frmwlmhh.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kxhylqau.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jnngymsl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjnlysn.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3hobufnpt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ctibstgf.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3dyecqngm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nisfahdj.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3gbuhylsn.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3yywmyzec.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3apyxndgf.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kjuvihlc.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3acqvbxei.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3lnsrsiww.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3igpjfibn.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3wgmhnsyp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3sjwomwjb.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3tuhtfujg.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3upfdwnsk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cykhcsyf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3epuowvjt.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hpudprcg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bdettyxe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3oamgorfa.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3orgawtiz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3dfyuozog.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3hktjhihh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ikqikeyi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3krdezmkk.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwuxipj.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3krynetbr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jbsxpqgt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxtmcio.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xtdjahnm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ikiyzyea.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rbbkajiw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ioefvzvn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ybjerpgf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3mefxsijp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ftpbixcm.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3grqswmvc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3palkibpf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqyanedm.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cfakydvw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qsxvzejz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3abycmpxy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftkuwcwh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xkbywmby.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hvoyduxy.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3djazdysi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dutzurni.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ahevxyjw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qknimffn.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3wqufyubo.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3xvxlgccw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3ixorhxcx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qapvcsvr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mgbgsadz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3cmrbfozz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgmbsgye.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3oxwajxoy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pzpxhojg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ncafvbcf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3mquzvtap.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eyoqxmmq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mftmmymj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3purfbegn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3juweefoq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzknsfym.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3xtukfnru.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkdkllgv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3fpjzomju.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3eblcpkye.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3fdybfzja.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nbhhycuj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3gqbzioil.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3muwempbg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hfcxdkti.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zlahzzbh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlueqaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvediuat.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3kwqdbfoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eikbfkix.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3hbwrlfmr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qaeugbme.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3inzezcbh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wjmfxcju.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mgmzekjf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yzlmkdld.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ahnldmzg.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hksgrygu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pirivrpl.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3eswcoqcc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rrafhxpw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwckvnse.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ehjiesyp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aajheddp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pvqadkzk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tajlbuls.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ldqykenw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wizqozek.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3fqpfvesg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wmnsejtx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbhebsp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmvptboy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyeaumdk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kspqvtpc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ciqtguxl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lzsujjao.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3tglzjxll.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ugbqbvgb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ufgbavac.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxauhriy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kafaiytp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kywalwzz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylcgwlui.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3oqjzjayz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3tyxbgnpc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hloaaanf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qmrllsuc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dydldtvd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3duaddqrm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3itgrpmwh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aiqtmoro.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3palddnoe.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3yqgskzty.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3hciehypo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkeamvpi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zipzfmii.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3nglzqwcl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3rioywkir.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyokultd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ctvopdie.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltugornk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3aeaqvntv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lempnjse.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3looehdkt.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ulvtulse.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3xvcmuuwj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vieylntt.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zkntyoku.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmtzadfi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3akwyejky.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lunuddtv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgfqzrvv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3evwilyci.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3kueymprx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3qsiudgsa.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3msprzvqe.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fyqwzxfy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3btqdwnha.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uakezzev.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uruqyxru.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3esbwkukn.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qybgoudi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jimoxdsm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3bhonsacu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3erdoapyr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhkqtxoa.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yffgfgye.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3phxouexo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tqtkukxm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qnoevlno.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkvkxssp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3xzmpctht.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ayrtptrr.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rwkcpjrf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3udcqfpjv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dyplndtb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3edwwjllb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3juuwbxhz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3boojkxwl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxivgakv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3crdedksr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3zgpzxxnj.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3anguegpu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3iuonyziy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zfkmvwpq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oobulqgn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3yuitehtf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3iwsdezwe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xplyptkg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xtkhkgwx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3betmjrrr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cmlqfqks.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3siwxixtv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3grykplor.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3glgthmqi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ldegpget.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cgqhpfnn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bifcjsth.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hxgfzmgm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iqornfkm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pqzxikld.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cqxqoors.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ndcghofm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xlpxvsnu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cagqcvgd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3yasdnivl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vzebmehm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3vcsqlsce.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jdtbmwnd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ugugqsuo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tczdzogu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvlmjhgm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rbpasmvf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nmqvaxqs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3alrvlnwm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ahxuvdzf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jlxjtutk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3brwurxau.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3enxmvxct.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3joccxahm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3heezdlmw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ytkzcyji.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3emkvrexu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pnhkyisd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yeqahibf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ufjlquru.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yroqkjbc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dxzndqup.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yodpcphi.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3csztjtms.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bywcpcer.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3tkaargwy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3eyntgkpb.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sbkhwulv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqexgzql.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vlhonqgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nudqkrxt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xzbzpcrk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qwqnespj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fezwpyic.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpsnuoxa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rycyrrtl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vwkjxvkv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fgiqasfk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ddjthdqp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pubhgtlh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnhtgnbx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hvndmdcc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rncaabng.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwupjin.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cwbasapm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3hehhorza.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3xevannnk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zohmevnn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gyqiuchd.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wgivpofy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3otmnwiug.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pbgqzlbx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfuyttmm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3njkvsgxi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrtvezsc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3onltyccx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ylyspqfp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ojkaihkr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3gwyevdfb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pmnwtqii.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ltutuvcw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rxmcyraq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ahthyrcs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jpddipnn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bquxfcln.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqdodsmw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ohnlgxwi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ckapxefs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3caefurqt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3clsjhrfg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kbqirvye.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ldrgwiwe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bxhveqxr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3nqeuxoom.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rjitzgam.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3eidasjmx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gexfkemm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3byxwooup.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3uppnujeu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3klxosqnk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3awkldkhl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrjpkwht.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qypcgznb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xvsepxba.html


<!-- 参考信息 -->