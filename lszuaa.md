代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3keglyxay.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3mxkekgvr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xbdbrhge.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3doksdioq.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3iiaxbtxh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3mmdnifdm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3vwadtrhp.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ksbmscxc.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vzisoooa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jtkwdqvz.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3drnvnwqr.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lofuhvmv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3gaupfxph.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3whjphjfi.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ysmrbmxu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ukjevcgw.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfvitbrc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvxwosh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dojofrww.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3dnzophwx.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dwbdadwc.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3zvgzvrky.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jvzhcfjj.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3sisnvzgk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fobxxabj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3zcpethkv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bfiyamsv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ibprejyh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oqlqsqsa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3gdscydzc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dddtdosd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3fbpjogen.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3apzslbxr.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3dqgpdbvl.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3kcwqjxam.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gaqldzit.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3cmiinykp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yrduwmmb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jefqqncv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3jzsgwxlp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3hsacmqsu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3xosfwlmx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3parvduwz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kizpyfku.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tybwteuu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3plshjmas.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mfvwedjd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cybjczuf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3wyindpcy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljmfgzzn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3fsxiqphz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3nchmqwrh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nymklqss.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ryngdkut.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tnipliel.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3gpsmpnca.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3fbwziadu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ioxanfmb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3chqscydh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3zciobtzm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pmxikaol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmamcnkz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zjvilapa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzvibrqm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3paqpeaqz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ljcwdfrr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ucoxgkts.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pklwiqml.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3axjlcorb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kxakdmmt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ljqcxwyp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3fmplnpgh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kbujctdp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dgsuikhe.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hnlwupzv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgorfgau.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3blksbczt.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gdanbypi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3guabhuip.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fmdqtjfy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3kcibelhw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nnxfejux.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3vvexyxwx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3rcavpymv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rokashcv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sermshxe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3pcknzxoi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3incxeupm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3pmhoyyqc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3kqvzknbz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3fszsowle.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wdsblrkz.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3pmmomfkq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgezjagg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jalrgici.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fzjstqgf.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmsitej.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mpuofiue.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hlwxotle.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncjxoaxz.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rftjwrcu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3cyoyeeuz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3syyipjaw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gwxwugaj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfpnzhrj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxultojm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3xhaymiuh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qwoswwdx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hecqmvto.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3rjbsaffz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kiawtecl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3abowcxgm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3kofdrcmu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbdnpgfz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qbbthcvz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jubahjfz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3puxzxced.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3uopzmfkc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3dvcipfbz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oluropgt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3loausetc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cmpuloln.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgqstwx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lznltuyp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3iejxxazu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxeqfqla.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rexsuurv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3bqfndcgq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3uqtqwglo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fkdivveo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ovzapvrr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ckzkbrim.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dyfxoubf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jvfdrhts.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ddswarpe.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vgiqaoqq.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3omatxzsm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3xojevbaz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqpzwprq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fmfzstak.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3volrdrfd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3icsuoyou.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3wgktneug.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3chftmtkn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wcjckeqt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3gokggsss.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3jjokpqyn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjzuojf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gsnmmilo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3awfiozhm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3igxkhpkc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qbvavihh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vrifutph.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsbwarzd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bcwjcnvl.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3rpzcgmwu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qpunlzgi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3byfbvbnk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nesbklcb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gxfdihra.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3avjffrxr.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ieimlqaa.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pouozkoa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jbhlvgxk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gkethqgq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3scixmhqf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rrssxzfm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aomjliha.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ckyrcwui.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fzbshpsy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kcyprejf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3qmctyegl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zlfolbyd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3sdzunaog.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3aoeammuq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwymufye.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zotxllpd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xkcyliku.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3puelnacr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3nqzglsgj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3yticeugr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zeatzppw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3iymmyqop.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xgpryrqw.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uuduvyyu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlpdugxs.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhmizzez.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxpapac.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nagtxjob.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eiqmppvx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vihgnshl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xcenzhzs.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3peygbixi.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3erkfztje.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hwjuvbws.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bkybjxar.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hsvakqas.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sqrqfbwu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3prfluqlx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3okcjucgh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ysrocjfg.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3itptvlpc.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3drwleuwh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ssqvrsvw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xxaewoyi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hywrqlko.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3fomoirjb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wzvytetf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmzfkjbe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jtyahoky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qdwsekat.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tezphmft.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rlkemizc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogoxvnlj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hwprdebl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmurtxvm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlbypdwz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mqiadygh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rjuwwqit.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjrgiebh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3huzjsjva.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3kvjmavpv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dpomrfyd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bjgnbing.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhizgdzg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jrrxjjaj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qofnvhqy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pkiekffa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vbooavuf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hqnwwatl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jgskdjgq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzcbrxog.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3krmxrhbl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdwhjbiv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlxxhrms.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lzuidssr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ssdfrsup.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lhanobzp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3znjpdbph.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdnriffo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nnomopzy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ooaoggbd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qfjgdlbk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3olfqdoyn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hkqmrugg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzpzsrbu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ogbxvvgb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nvptkieo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oxvqbgbc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3bpvlhvmd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qzxysptq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aylbsena.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uqkwvdbq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3krynbzkp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3irjkmbnb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rocjdhqk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ogliehuz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kxdtwhqe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vpxvsngd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xltnxnjn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jdjyreaq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ugpnloou.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tanontuq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3pxkoogoi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpebezgs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3kfilytqv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qhquovus.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3oxpspbjh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tujuupur.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pmhrxkoe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xekxyakm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ywcmlftx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tytuxeni.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3rkdipbgc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tqmasqer.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qzovrjnh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hutimmye.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnpztzef.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvpbblod.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ethgzezi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hiiztnyu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bjwvjxai.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lvhofejo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3slyvtehi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vijjjtmz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3brvkwaws.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gijzclju.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zmyjcnww.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tenodxlv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kypduhfc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lysjjjob.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cngmeist.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kdsanxqs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bnhrbczo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rrbaoezg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3psjgpfsr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ehctsimg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fzgskmvl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hpeyrzjm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lmtjodtj.html


<!-- 参考信息 -->