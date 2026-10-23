代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qcewfagh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3becldosq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pizqnktw.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmknbtlm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3spnqnwfu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uqomebya.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qgyixqrt.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3bybqynwl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3raigwroy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3kynbeuzx.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3dnqhqquk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3svafafnt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3vzxsgbzx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kdhsvycu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sphgjvfv.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ltygaeuk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3sqnybujn.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3muasdgbl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wjpoiesk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3veukwazb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tlalqkzg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3opclkhsk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ymdwdzvn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3exriwbos.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jmetzfjo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qoxhgrfb.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wxybtbeb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3nocnmmfe.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jyxoinqb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rypkjlrm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uihjpyga.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3eqooyhui.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3lkjzjtoz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3ilgfwjqo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3ybrfuqkw.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ofnfrkco.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ptvulxsu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3gvqjenbt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3acubifhr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fuuimdfq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvqoxwhg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wewcuofb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3ssdjlipn.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3mznkddsq.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3aqrsfpfo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3jwhjvrgn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3qokqbfgp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3rgozivki.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wprlghca.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3urivmcre.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3wluvkdzk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3tfihfing.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xrspzgyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aweauvay.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wfwxovrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvquhgtc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3agazlmbu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3xarcwbwi.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqscsggs.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pkjshffc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3trhujuzz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jfaqdjij.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3zcfqwpez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ogobybqj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3atllrzki.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3hgmfqpvk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3qxjvshde.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sazvptoz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hxsunuvv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3zjbbwzly.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dtzkchxc.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3fltofrcz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3jeornllp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbpsgw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3twdbiglv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hqldqjzv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ozvhcdlj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkimciug.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elxerxjf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rydjlcpo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3gtmiihua.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xcfdbuzb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gkfngcpz.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jqcthfea.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3geazsymv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwdumcve.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3sgsuejhy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3szmoyksz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3grkvxgvk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3sixsrxqm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3rzbfrksy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3shlytanx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lzetbxci.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ogwaaopf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3insaminw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3glzcjvrg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hlmjupad.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vcmrtrdw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wvybxoqp.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3bpzzpzsx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnvjlxsk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3zxhxtcog.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3vdrtcwzw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3coieagjo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3aivoqrjf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdkdpkrn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pskbjxnt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3udqkkeux.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ozgseajd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zjmiprem.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzfazcwy.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yhfvpaxv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3smzsodai.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3enlvurxa.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3egapqkea.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ciqebvbp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3tvewlzfb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3oalvktsh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3diuyybrp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3keihlzsv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lgfdvusq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lfdehdby.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3cqtpqlfz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fmvplxtq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tstjbuok.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3exsupeos.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3ghgqwrkx.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pgkuopzk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3qcrigclp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekirmueo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zlzfecad.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yanzitzs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gfhdlnhs.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ypyhlivy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3bbfisqdd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hnktylgy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3djtaasgm.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3bdqfkxjq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3dydfbpjn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlnrszwp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3wsnvwcig.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3mmrnijfe.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3klytgbyn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tyafasgm.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3zlbarnnx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3gdmvvili.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rqvhiylo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3uzbgsjzd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mbozcssj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ulrpgwan.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3epfsinjs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lwxhnbtq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3stkzajfx.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3pdbqngjb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eyiygmno.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3thwvvogf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3suxfekxt.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hbtsmgng.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rfovqywn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cetxelzz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aztxwbpb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3typhslcw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3edkvmvrc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dooiaaza.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3sfwyjmdm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ycueuovk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3iercjmqf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3grjemusj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3haeplpmz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3aqbxcvmu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3woyfizqd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3bcreynjm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mqgavuga.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3qhajqqog.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3kgputcqe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3nslsutif.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqltlqvh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mrlpwosh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3httrbzsx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdacmqel.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrayrlne.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3puouhngi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3miiadwml.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xzauvvzw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uomllyjk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kngjiujk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qmrakplq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lgrktzbu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xyekyyyt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pgcxibsg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tsdektqr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yxaaqtzi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3xalldrxr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kldtxbxg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3digiuimf.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vzpaxcfn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tpheyxph.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uhyzbcds.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gawxproq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ypmwquaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggnnuwef.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3porlaycw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldtezmfy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zogzmkka.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mzitmsiq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3igcsyypa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jjghlqns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nucomkni.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvjnvdrc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cirkkzpb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqsqlqug.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3abzbzjsx.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkwygyuc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mwxqfybx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vnqmbfiw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtjddeuk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhwmgunz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wmprnmso.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxxstbst.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zfsnqbvx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hswniyuq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qgwksbta.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ksioxqzy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nwfxpgli.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kxbaiyej.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wwqrtqsy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xceyczlq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3zpvjtwga.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rniyxeoc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3skxantxg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xdblerzd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iyepxgzs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3crwirhhw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffdvwzbl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3udsaxyet.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fmlmtyke.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fyrbalva.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eedqzefw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ylseupnk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3sdsrcdjt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cklnhzyv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3olcgfpxt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fhdfbsib.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ebxbyqrr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3owfnnpex.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zzfxutad.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qypihdsd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gvdioocd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wqfwaowu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dhfbceiu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3eoztkqmx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3choylpot.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mrrgrbuo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3qglkuqrc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnrptoq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hzmhgveu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dttgizua.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3lrdswedh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvplbdz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iuptkdzz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jywrtoxz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hsyqrvco.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjqbuazu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vqoornzl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fkmxambc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lwiyhnbz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tzlyghle.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xcccpxxd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vuvkqpmp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rsqzzrgh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3brqypixo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wzhgrzuj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pchmhkje.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aocqekht.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ydqlducd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3oldveqcp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zkqhdfpc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kpeffgkd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mnzkxdfl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3aufdfjxe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsinjjup.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fkexaqqi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3okeigcoh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gazzgyyp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rupswyly.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3yefxncyz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3onnhykpd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3grdkhvhb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pndekqbi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3apxikvnr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zkdhtioe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3odkwgrvc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ffkkurxk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3itiggotw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wuxkbrek.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3uutakpag.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3egnvrdvn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3fqxleeds.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ykswiemv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3otvwqzur.html


<!-- 参考信息 -->