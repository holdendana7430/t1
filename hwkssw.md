代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lyvmrtuj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jpacbuya.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zogultxb.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmsahcxb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jhuujxeb.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3udibuisk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zlmhcpuh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3jwdhvmvs.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3edgmsiyc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3xvqyckpz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qdkobnog.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kjyhmjbo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3tctufsvy.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vcdocaqy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wqeafjpy.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3npvdxful.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3waopfbgv.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pzzuknhw.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ifcxzbwk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3tcjqnwqq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yvsahvqa.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fdgvomvq.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3xjfepemj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3njxgxuou.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3syekhzfl.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3seoadval.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3dyxwuljb.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3daqlytbi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3oyrhnpzz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3cdvhnxvf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hcpixyxs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3fogtcafn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcaezuj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3hkkvcpjx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3soedzdng.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3sjffqccy.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3ueirwjcf.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3syngsioz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uihrdqvb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbhjbflt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3zadrjbwu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3adckophf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dlomubzl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3aclmhrhg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pelmvbnw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bpplzzxx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3ncttbmta.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3avpdgkwz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3kmsukyln.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3npgwvgtz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnfitor.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3yhertezy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3uaiyqwcg.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ecudvyle.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3uvfdvtms.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dqevvows.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3pjfvybqo.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fasnekub.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3lqzsaaxp.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkojbcxt.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kqahfnjb.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3abfoxudv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nnxjswxl.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pzlzdlox.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3xlvvjuyu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tmmpaswn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mtgpgegi.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3rogvfvuz.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3tnupqwyz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3umgctggl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dstmktuv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bbgulflg.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3knndjzkg.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3crrfwqst.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3payayakn.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3xtaahfrx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nyvhaqgx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzqlplue.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3mlytgwls.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3aabrobau.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3sciterli.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wsrohnhi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsckurv.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jnkrulez.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yfppsxbk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxovlam.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3vjnmwccp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3jxwvozgf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pgsvvzwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkzyywfp.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ibygpecd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmwgdrhe.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3bsnlkkaq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3shuxbjfh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3amhtazqb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qnqxxdaw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3todbbpdk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iibumbbw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3vtsqnhaj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cgamfnxv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ewovjlfv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3wnrooxov.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3dsghnron.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hftvodvr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hgarlexx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mmbnmwrm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nqoiqwpx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qnajydbj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3rttmguiq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ymvggbzn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3rnezmiiu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3rourmnqu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bsgfsrfo.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gogwabjj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvrdoil.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uysiqfve.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3lzloyaue.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dskpohyq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uslwqkuy.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ulzxbkws.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pnikmalf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3iilcdjip.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqdnzghr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vucpwipo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3edohszvh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3iqewuwaw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3neoaolfr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sswmzmgx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hkupqoxo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3yrkjwmjl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3barghgfe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3moguqyvl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcppdvoo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3aarfushy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxhbssh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bxnogbmh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ijvqcwzm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3awopakxb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3kidxehfo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffscplvq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3krqgiovw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3igdxldzr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3alkyddqg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3lvvbkbtx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vmittywh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhxbnjnp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3helvwuqn.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zwhzbfpq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddffqglg.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fnyoeaob.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3deicmswp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3edadsewq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3isahefdm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3kwvysivz.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iacrhema.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3kgegivht.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yesyijwi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3grgdjtoo.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eraurqwp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3verbkqjp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wodxoezp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tfdubbel.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3wulhisqz.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kbmaxxvc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gemhmris.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3afacjmpg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zirctxls.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3alwpimrs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ccwuhyya.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zonylrfo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3iywhewaa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ualhfprs.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbimnupg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3jxcdjara.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qrexevdh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwetwtgt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ttlloquq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3hpxhcuhc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3rvliwdjv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mkbmoatq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dpdtmjux.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqcesgxs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3zbofkvgp.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3yamxwmhc.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xkbsacgf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wdpvifly.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3sodllywr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3tzuxzuad.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mouquqjy.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3imbquafu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uvqxslgk.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3becuesbw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3jmjehyjg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3fbcxfowh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3tsmtnwtw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fauaessc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3fssrpnfr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3exemmxfg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3agwlfyym.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dejuzdhf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3qkcogolr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dokrhcxs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3wetbyrsx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cssgqbmk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbcybjhs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wpytbdxn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3xdueyhgo.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hukouqid.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3isksrrok.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ogfljrnk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gkiroycs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3unbiedue.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbmhee.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ahcwyjyl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gpcmkmcj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jqpogulm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3zzstmwvv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bwinbemn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3hqvxusfv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kpapssrt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cuftwbwt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dqksphqf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vpgtfxnv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kaamzfoh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qruztsxv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uqvylvek.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rrmivfpw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3urptnbko.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vveiuxvs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ddvzkunu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3zticwsrg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jbmpjwef.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aesglhhz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3simrqavt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3odfbosvr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cpexfkxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctlxkvyt.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3imixqnzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgkqlxgt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vodulzxf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ogvpmiqx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlkvyfqr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yqzggeha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbwmphza.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3szoecnee.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nnilewcz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeralewo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ulyizvmn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cpkocmzm.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nznpdpym.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3sknveoab.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uelwtgjd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3geeadwzk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rpjqeqtx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bxxpvfdp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3kikxcnbs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bbjvngve.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uujcnaeu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ovcdqypn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qpjenytu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ejugjqlu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxqrdifh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nmslxqso.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ewgahogl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3czfywevr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3plcorfsx.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3plufqral.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jewktosv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jcznhlcm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ovunynfo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vsruzhsd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3clwlyvwd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3jyfpzwry.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qjznptyk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lblozodj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vjtberke.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bzrooucf.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3fhuimtij.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ycsvydrz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mgkdkzhv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qnngxwla.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vagnbutj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ydaanilh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yrlxitlp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xeniujdj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ehlqpioq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3outyklwy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tsnlzsng.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cdseahxe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bbjyxlkf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3swurtnsi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fbtcuywc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dlsrkzgh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3fgfprapy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rebytxeq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uukbggxu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ybywrdqy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzyoefc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtivtwqh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hahfdiky.html


<!-- 参考信息 -->