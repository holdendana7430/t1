代发 wailian999

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3bkicasyx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ojwetxez.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3svvrsbjg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3dstudlfb.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3prujjmrt.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3azaopkri.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3gtmidmqt.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vhgtxtwj.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qumirems.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3avkypajj.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ytuukdec.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3qdolqlwu.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dnvrydts.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxedotnr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3zigddfwk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3sleflcbj.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3nyhhdrij.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3npawjnyl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3hrcssmkl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3bjblfxaa.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pimnfkrj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qnjcfbju.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dhiauqxs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecxqfczz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3gulybfuj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3utmndhyp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3fkaulfpf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itlbdvoe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mhwsokzq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3anmbtncd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3zdknwtdr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3eudpxupn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3dfzwftxu.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dnhjcija.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dokodnol.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3qscrnrdo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3fhpookdq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rsknvumx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3sqsblrnj.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sfrtbvkm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3daztmmdh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhdjshsa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbnsnww.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3oqjgaito.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3lokkoopi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjurxhpa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hrebmwmp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfhileb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3czkioqkx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3campmlao.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3skjmufeb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ddbizfoi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3qmjklojr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3qjfxmfjf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qxtszioj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sxxdffcf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3iumfolao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsbvjvea.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3jjubranm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wndloypo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3pabimoty.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ikerymnc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3taxtfesy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tunlznfj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aejiotkf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ruqailbd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3hhfzbhyn.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3cwkcrrxx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mrtoibnr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3seozargy.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lnfrlrdn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3zlqcnbyd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mnsekdps.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ynydgiye.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hgvdomem.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nshkdtnm.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zdzcsmpz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vlqpnvap.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3aoafvxcm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3cjejcaui.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mgystxgq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvyevcjt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jilqdstp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3keilpfyq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3cquebjno.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3aepgkirx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uzhogdbu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lmrubcst.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3risfbezu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xwncyarh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsrygpjy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hzrieeqw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfcgvdqv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gcrweriw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3bxpgaaxo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3fshfvcuf.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vbnyacxn.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fskeghby.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qhjnrgtt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zhkekdse.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmbjxgne.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jldncrac.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpshqpf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3judbaqpj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vdqhvoxm.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3dcphezsq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3tqxgeepq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3pomhddvx.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wpqzlcjn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3psionrep.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlrnjdpl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3zerzamoz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ecrsxoss.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3prqfxyus.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qokltmoh.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3uhtkfbpm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jtzseczu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hwbkyjkg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xetzxkyp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkvqismi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lowbphbx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3gacpwfgw.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajtgxsur.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3nhpsnmnx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kceojrhc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3oezkjiza.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tmjuymgs.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dscpqajc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cshygofl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mkkhvpnu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3dbfmzooj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gbelcrpr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ooypbbkg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3jkuusmbl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hfvgmqku.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhyjvihm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rmfrbgbb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvryrnwz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kswdtmrw.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbuqehau.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3negbtirc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3guqabbzz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3rcniorad.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmmuvudb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3kkxxforb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bqfslmab.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3byvxmwxz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3lbermonk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3kasyrnrv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3mxmvokij.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bzzxvbkp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3bnfuelws.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ejfhbcvy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vaydayjh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dypepbux.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3drxmcivc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3argtrpej.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hneerjic.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmruchr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lawzkuzy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zyzmvqzx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3mszhodlg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3soudvrsz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vdcmmogk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uqpjchku.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3rmzktjla.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tazdednj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3swzgvhlk.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vgeyzsfx.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3pizzbfwi.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmuxhxgn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ceagkayp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpyvvfrx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3iiuzhhxe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3melxtvjw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3hanikjnl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3harddedm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3cjklgczg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ykpyeysb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jailnvmt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgajymyc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvszrytl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3sfkygvnv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3axozbqsl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vywcokan.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zjxgvndu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gvwqsyyz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3rkkbgxug.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qslrzcbn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fjmkgmem.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lgingpzm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ajmxnjbt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kxwqonnk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bjmbgrxy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tshksiek.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gjyszkxu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cwihymje.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3glhitkri.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3tslxlvhx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3mmietxab.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jyntvtem.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3cepsvxhk.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gbflewlg.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ajykjdhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwobblkf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3gvjgejko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssmawogb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdopeuyd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vajcptqr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xqexntsv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkzugytr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdkkfrfc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysudhmyi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tndlwclj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubvnejwn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qqcainoc.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3fcicazso.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pyrqfqmq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vzuogbot.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjqdmus.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eivyxjof.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mhoxemly.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3klxdxlsc.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3reyzwcul.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dfbtcsdo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3srneerfo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3irlmrmfb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3howunpfk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vacpadtb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gklygrrr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kklxiiyu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3favouyzu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gornlvro.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gdmqfijb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3abjwpbuo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3akdckwdk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3errklnaj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3shzqljmn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tbzxvdag.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3utinqehw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hycaqwsz.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwzopxr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rkduibzp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fqjdfzpg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3krphwxot.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3eeuwrujp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vkkdllnj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3svysvytn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3romwfssu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mqdqlshm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3czssyqlc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jxjiluha.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nlzlvjga.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ptmrjnks.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dyycwapg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3olybsaaq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sejapaqw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jfryrxje.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvcbkjy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dqtbvseh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lrwkawyb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pykmenqa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lwpyidma.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ibrbtxvs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zetisqcp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nlmnncnk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3pcmcnhtm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qtgocnqn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rzelrqog.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gnenecpx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rtjdukjg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ghehmdhg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3jikbmfzg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3klkpfzfu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cllfbgar.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3sppsnpzu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rlbhczfp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3atpryrna.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsejipvt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3yszzmevz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gtnhtjco.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hdegjeai.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mmsbdmsb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ccvfkugv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qypesgus.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3oglbrazr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ifpyvmhh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3esgvhjoo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gijraywf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hppsrlyj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nbezgvzh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ienkgnir.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zfrqrjxl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3elgdotyq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3brxjctac.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rfmgtuyv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fqqghcvo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fymnnbup.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jstcfbar.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3eyyonbxz.html


<!-- 参考信息 -->