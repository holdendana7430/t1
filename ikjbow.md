代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qwivjnkc.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3udpzatzk.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3xgyokjks.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3zkofhzpv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3gmefhtkr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3uqujdlnv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tofhvngz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3lnhdyidc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ibvkkkiz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ddjztwlw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kwljhtjy.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3jtorgwip.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3aikkspap.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3gxwziyjb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3uletpzwi.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3plasqvpg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3djhehekz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3amohcwzg.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mkfcyusz.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3blycroan.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3hpjndsua.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3tssojzdw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3epgpvnau.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kpzifghc.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dgwyvnlm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sxqvfffa.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hydooalz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzxarx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vfkbgoxz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3aifuvznw.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sudhtefe.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xnzxvoco.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kodteehh.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3nqgiesus.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3etbukajv.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dfxycgsb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3qxntevwv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3yfdatpxm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdtdbuu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3vwkyglzn.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3jizhfgns.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3culbkwzu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qtqnkjuo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vncwbdli.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3mrtvgjtt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ifwvuekr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3odutgqio.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3mzgwtiwi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cbfkagdh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tvynlkrn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3evfgizbn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3pxsxnsao.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3acfaykhk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yyhdttjz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tkhwcont.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3gqevodkq.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3iwokkzro.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rpdvlcgf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gwvyrdel.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dgpipcmp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3nvkzbvud.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqvkmlt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wtjyishz.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3enjqedgn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rptqjhrm.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmywlrgl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3tsfevivu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eovxpgvp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3sgbbduwj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3yszipmom.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3fhdqrqvb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3eovzvbin.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3mexclcvo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lolqhvwu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3zsizypid.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3itnstzme.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yrfyvvnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqluxsne.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3alelxoex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onagaycs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vxzctrgy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3arfctmso.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3barxtfwt.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3suhmzfov.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fdrwkbpj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kmranqsz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rmdvyngn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kdextqjg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vohhqnlf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3qlbfqozh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xpiyaijg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3flszlijp.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mqonbuol.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vattzjrj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3obhganrl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ithcyxpg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qbyrxmag.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lhuusppd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3biinixei.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jfpoflsm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyixqupr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3puzqzmtk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pfyvfftp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zarfnrgo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ywmxstga.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3qfgfgkkh.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fgxcypep.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pegrbxbr.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xlqpdgva.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pbwtnuor.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3yayjutqp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3eolupdbj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytyithcn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3nrnryril.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3lcpgbedg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ecyjablb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ujpwoihn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3esnmixtq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3bgmnigvy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bhrbhery.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3tbhtupeq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqqzhnsc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3zzdmfpcz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kzchcjey.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3plqopnvq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3eoeyitgo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3fyvgewro.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqamlids.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3msapcmye.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3elmwoefw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aofauvyl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zjpeurwq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3inbzxpbf.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytldkquw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3xuawkfnc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3qgddnedo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xysrttdf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbhbbhqv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bubczvag.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjoeifpl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vdhxuzen.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3dgnzzyci.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxxhyfpr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3cpjbtelo.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mhicliqj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vreuecxe.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3hkfjjlvh.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wbcwgbjh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fpnthtyi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bhaxmpoy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3vipxhpqc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vguvwlok.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3rnczvntj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yrevwsei.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ibxqjxzv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xbrhafhz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pownphkj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3todppdjd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3lrkferqm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tpksiuzz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3idzgrfvz.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3xmknhgxr.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3btdpnvre.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdfwsisf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3awfebyqp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dcgpogwl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3knamwpag.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lxbsniyl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3iqefayey.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3ulxcjrie.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3cvinvcqr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ghxvqprj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3lmjdneyv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ojonjkyy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3avhoypqv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pvwqynmb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3ckmnikic.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3tniseusp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3nuvevxrs.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3pvzfsncf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3vfhacqkx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3trpcpwkb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uemmlpos.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hygwimeu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uoeqlfnm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pipogcwv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ufhqrtzn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3bpwbvpbw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ycahryiq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3eiwiumau.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rzmgvhlb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3biffwmwy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwuaqsh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3paflzodi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3pkchkvxo.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zfdvgtjx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oewnomiy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3eomzdtfr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ofdnjrgh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3rwphzkrd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fetakmss.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcdxmias.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gychyacz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzrmgguc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kcxpbvza.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iegqvxof.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3jndrxksk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3deaxotpl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3njggvrkz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fcjmezob.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nnxrpqli.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3czecmxbk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mipzydks.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vkqovwtg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eaivxssc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3uvrhqkwd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xrrwsrkx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzzytygr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tzxfzacw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zqoegjsg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kxmklpqv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3xppnavat.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ckgjnnrr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3afmesspz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofcivlsd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mekpjouu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbugtxae.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufhcetnk.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qakidpey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tukcrakh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyunxpqu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ocdpyvvm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wvqolokt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3meurimzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3oeouwsee.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ykvctgtd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3cygahooo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rpfuzryh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nkhadghd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uufecqcq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cudnrufy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rvklkleb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3klmrwilf.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3larmlfns.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xagkzexb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3iufgnhrz.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hathrdst.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sjcknvwj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3emkgknzg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3trmhseix.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aravqngt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ggzdxuhm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qbbdnagj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bhwwzlhy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmuvpcxq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rfdnojvg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kinrjqzb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3csuuosix.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zdtiymnw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pqkcmvlt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3tpbaokzu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rpidndqk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxxldsp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3eojeuhhb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3spanaoaz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ankfvxhn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zyqydixs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3llndfeoo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zzpyeqcb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jkwtdlfw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pswewpei.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qjwpthxs.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3isyzlfdv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3zzmpvtem.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3wlvecitt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3oaqkzidm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cjwpmweq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zzgtjotu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3llfmuokw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cizfekds.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bofjxsxb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gplqtkqf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hknqjneo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qdnrlwtx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kqnbnhqd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ajwtthsr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dpqgegid.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3trdyrptf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mmexvjnj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qpgjwhdb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xtjgarqa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wrrzzhgu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlopkich.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpumlmri.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zabmidhk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3oqfjeadu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kwgfqyst.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wpnyghki.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qoeueyzj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ngzebxoc.html


<!-- 参考信息 -->