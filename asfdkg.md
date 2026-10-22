代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2mqznggfg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2xgavjmrf.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lnvkxjzx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jucbwxrx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bcbmopvo.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uxyprbfr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ltabelrv.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2emqzucem.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2srxwcmzr.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grzwrmfo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2pjelngjn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2dxezwmod.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tpxsyrlv.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qozwrdzi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arkrhqvn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2crzmybif.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2hdpqcwut.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xokkusmk.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kapnreoz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsrvhxls.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ybxmlclg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2oaxdovxp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ubqexebb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2osrlsozs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nodwlpoj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2gsdrmhkz.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2rnodrkjc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ksripvcw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2trzvgukl.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pmvopguq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2oauhktcw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2tkxzcnqm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibajmhme.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2vtagiwgl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uuveggwp.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mgpwuefg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cvuqlece.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdgvghi.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ifbogavv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbiqcev.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ghzcnvzy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wulalvxu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2npgsshxt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2isazbqpm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2dvrlwxop.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ocowjmcf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gwjhvvus.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xkkzyuea.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2rmeoiqze.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ckilumqg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dyojwcpo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pxjlgrkc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2evgtmjdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gydijbpw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2npdeervg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogtzwdxy.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fuggbdvt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2caubntza.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2satniztf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fumixhey.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zmwhbgli.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tnjgjkql.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cmvlemyh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ifhzodja.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ewdpcbzb.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2joeezpvd.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2kzoqcdie.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxwhtcrr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hoolnwgk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xfieabgs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jafuxluo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpwjqveh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2zwlhhbnh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2voawyqzs.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2heujbzhu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hwxlizdc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tolyyncq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pjirhniz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzhcvsbn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vtwvboof.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ppxlvvsc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2mowyapcu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2haoouqfk.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2cvuqcozs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qhvqanck.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2fumxurif.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xaxyjahu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkavstom.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2cnnqvtmv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2svowinin.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2czrrxxbe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2bpoxxkce.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zhkhgaac.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2muhawwju.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2fqhrulvy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qrgxjjgc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2elflwjjv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2yaotewip.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tuolnkxk.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2optusrhw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2cntajafi.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rutcvpev.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hqqwgxfy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzdhekil.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2lczlzmhc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqjbrpez.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2mpgkqxvb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrnpiyvg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fltrpmoc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpzxmusc.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2voysrjyn.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ugaddkah.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2evljruia.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpttlras.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrdiqwve.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2squiohqd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2rqxastpj.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2dtrhteuh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpzdhleo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2yvitegki.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2lncysyts.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rknirpat.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2locdohbh.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jlceriuz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dnmvarqu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uegnnkfk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dozpfyku.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2biizabsz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bjehugnn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqttotza.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bpgxfugn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rkfxqkdf.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lxszthcj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpvjhsi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lmqwbayt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2lqjlgjdm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmorktds.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ckmbvnvc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2omzysaez.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmjvcvxg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bdubsfpp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ccwucvtr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgijmctf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gypegsty.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rpyjupei.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljekfssc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2myqontng.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zfogcmog.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2zlcbcnsz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kcgdoxha.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2kisnmlxv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2emzosihm.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jsuutaes.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2autlyrwl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bnwhhznh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2pbgslfqx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2buukynka.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2eteurzwn.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nhschcfh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oahgbgkl.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nkdnumfh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2yahbzkmm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2budvolsy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jintyzpr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2fvbqtaoe.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2rhhkxyda.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2sylhvjgo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gtwuhbky.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irrijvze.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2krbeqhke.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2uabnszju.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lakvacka.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gvtisoxc.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2oytqhtpb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hosftyem.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2lunwcqil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfmamyn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hznpoyqe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvrduzc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnawlwqj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2viidmxvx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eccbbghp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2iiasuswn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2zrfhpnjf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2bnqntsrl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hlpcvaub.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mpqfgecc.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vuqgrjdl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zkuvobbi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2irtxaktr.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lmpsduso.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2usdicaxo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2coedyxyr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkigtpfk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2rpsajcjm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xzoocaqj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2llxbvsgp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qpurisbw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ydxcdyhs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fziwaaam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2heuvjcwl.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zgwpykei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjyvzuik.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cffhihvb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cvxqhbrr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nuwcjwsb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrnlhofh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hurzmfqd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2msaijhtb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2goqnghjm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwtomdyy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uaxkgerv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2vetwcmmj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zypsbouu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2psrttipd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ceqrjvfl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tzhznavx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rtmsknql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqairuhk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rpbnokdo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2frmjjovk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ynepvwgr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2lhrxaimf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wowpcoaa.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdkxtloo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ujdiihfg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2aqrrzxhu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2rpixhyqn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2djbbqilg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pnnmoeei.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hejzzkwl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtechin.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ayilhrnt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czqxxcwz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qceczkue.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2igdolmjo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejaflnrf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lwwsqdrp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqxepgo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2huxyhtfv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vncaropn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2aztfamkj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ptwooobx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vejysvfm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2wnprstsu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nwvijfly.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2khfwoney.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tzrgduch.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2emrvvbhw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ctrbogyt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ksxhphxj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zcxtjtbx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2drvmabxe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lqemeuws.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jnrqaaub.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2rsuatvud.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2haenhguz.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ouvlghca.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzoenqq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qrkhavcw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2orwujycz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2hedpwjsc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2aghopcqv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2hwmyrtvf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2nqloeyjq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2psaqebxd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wkywrdpx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mnywydkr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kynhezbs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2icpzxzil.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvigatac.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2iocaxagr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hwojzwer.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vackcwli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2heqinnfp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2cixrznbm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ivjxicrq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufjtuelu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ebmmhkos.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qnaishgj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tosbctfl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmjeets.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2okwmanhh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vcojfcqr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cgnxxhwi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ogykjgao.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pfqdukbn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2zdzsgegw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mwlwzkjw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gboltupr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cvivkkow.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sjoigxvb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ivtvzblu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pzzqbqvr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2latkysua.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gcqdsnrx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2djxzcqus.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2svrfjkoy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uqgntgrp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2stnwzwmd.html


<!-- 参考信息 -->