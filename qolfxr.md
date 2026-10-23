代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dpupdcor.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dcohacln.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3beotrtpe.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tupofevt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxalclzn.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3noeftymg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dnkegmeb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mhslimno.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3bnumvxsk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3egxyrjdc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mbmcnisr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmhryyv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmevzgn.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dbmgmgar.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3uinjvykx.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3apznqmet.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3mplyikbi.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3qfblfsjh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ehiwiuhe.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ymacjgvg.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3vsahrwyd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3tmgysqpa.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tqgmkmie.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uxipowgm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qigntwcy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3tdwhkkmp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3rnkardje.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3gtmvmtyo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3jvxwmvif.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3xeffkkov.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3snbtevwn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xjorkjvs.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfidoji.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3rbrsfydu.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3xenaqzoz.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3oxsgyxqw.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rgjduqfa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ksqlgyyj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lbfaoxzt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3datrgtpj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3srczgkzs.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ashhfces.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3wzrerbsd.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3zowyaljg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3gwztmoof.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3envtcpng.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3nkjnvmdx.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3hlfvuril.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bmatytjw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wmwujckm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gicrhbgb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lqoaxcan.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3kasticoe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3kajiqjjn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rkuzwfmz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3dghgpwpb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3opmofrip.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3usnmykqq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3azbfeljt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3msvrlwfi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3pqbfwwav.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tjuzvooe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3hvmesxgr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3cdlsfgkh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vyeecoum.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wxrmhczh.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kdskilsy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fnfryujy.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swdaidbh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3stmbuktb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kdbfkrsj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3duhtvxoa.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3izdbbtgl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3vlruoqgd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ybhrgsje.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jbbcxges.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ueuoozee.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3vthdvaka.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3tdctftbp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3olqrvpjq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3uukbtxec.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yrliqvdr.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkvvdzz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ojuntcyp.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3nyxwyeip.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cymuzrax.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3vudmzytq.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3coedjnmw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqvwtgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eodwkrbh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3lubeepgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3frtvkizd.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3ucqvqosa.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3icfpdjlb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jgqboclq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dehubedw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ljkrvrkp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eiptsrng.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3aglcjwur.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kigyruzc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3munpdaar.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dtjacnah.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3myhafjyd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ysjhgipk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lbkiowms.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vrqhkzso.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rskkqtgr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xjgyinsg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qfbsbzyh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3emdirzcw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ksszdxll.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ursvxzpe.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wzfnzswp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuqfjsxe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qggxfszp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tylbrfkt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3khsqamzp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jnarhzrh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ddtdpcej.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3quhgjzax.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mtwvdaid.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pwmshnzp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntrbhfkt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gamaymst.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfgtvjps.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3citqwije.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3hpaczudz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgemohgs.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vtedbjpr.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ersvhqns.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3znvothok.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jphsnkxp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rinzczkd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rxmbzmth.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3kjfqyusg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jyxgnqma.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrtypqs.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ortjskpo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zuqcwgsb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmoyfxwx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufzzgsgh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3csipnrts.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3egnyxxqe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3scoyrmuc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yuulmhbh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiximgrf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzdicxej.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kpfqiabs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgcakfgf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbxyrxd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jorcncmf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uombruhm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lkiftgzh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3dehlsjaw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxddzbfb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dihkscuz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3ofnqlehb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3awtlbquf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ftlwplps.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jezyygcx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkgxhfk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3fprfwbif.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3hepxnzra.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3monpblzx.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3fhzepkad.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3rtovfevw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rqzxomoo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3utuolzms.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3inetarsj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ubmyvsbq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3oujikglq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ljixuric.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ajkwqjbp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3yhsbizmu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3ofxobhtx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oedzspyf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3blnghfld.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ufmbkmrt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vszrwpzm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xycaqbtk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xjneabfs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3klrroykv.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3pczmoidi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uarxesav.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3uearuzom.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bethapvx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3uwplwobu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3aysismom.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3vwblqoav.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3llihxiuc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdorukj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lfdtxrae.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3qxnuxwtq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3nnjjrdcn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rgljilfi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kwwdviak.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kjyioflr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gjbhrzso.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xfpdvhqw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3iqcfamqx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3webyszzq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ppqqkjpy.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjtmhidg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tonpqihp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qugpkrps.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3uurmsvqz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3bdprhprq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3cxlwrgmi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3pbarneuf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xmwsrbzi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gpvtvyyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nutttajj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfcftbc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bsinsugs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3desszodz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xetcfoxf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzjungfz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xohfluzt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3qdptxofx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3kpqnyorj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wnfcbakj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwxygign.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zjnkonmp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jwvvomns.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aewbybxi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sklbumhl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fcjjgmbq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pdoiwxgs.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zdrkqlws.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3aeheazty.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3npmikaom.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vqqpbnwc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gpicwiqc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rzyrjkys.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yjssscef.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ztbtfgyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jadxevvf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wlparlxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcqjqwsw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zksqdboh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3msxgjawt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3htphdism.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fyxhauoq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlzjmdxh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fawrhttk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pwjfovdm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fikhujfe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xbvdgcoq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnflgfks.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wjuhpryt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bghjcbve.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lktbbfea.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivlpvqvl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xyldfyvs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihmwmzxa.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kpnfeoas.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3qfljxkxe.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3eforxfly.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kidhpwka.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3kwfqoxbq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wnykwhqq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wucxxbdd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwnzyoa.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mbzwzzzr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qzyakija.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sqpvjpte.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dxgawkvt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pnocbyhv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3qdomdqsg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inibmafb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dayknzfp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3twkswxgo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ttypdzgf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgnarwse.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3culphuyb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qfgcvixb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xehvdjhe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jchalvfq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dcddxhwe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lcsxeqys.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3illuitdn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mnqvconl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3stblkwsv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rhmvtpvo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3coqrnnjh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3onqxhczd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wjwcjiri.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tkmxzqqb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hphsynwo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ouwggxdo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxemcae.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gvjeihds.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3idsorimy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jjizavxp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xkeupnhh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3spkutxgj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vdbuswzg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3efkfzqei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hplphhjn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vhyxxhbt.html


<!-- 参考信息 -->