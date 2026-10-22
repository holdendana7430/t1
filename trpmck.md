代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2pjtrojkh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wqgixxxl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2htbitmko.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rvbxwltg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wthdlmgm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jcqsrelx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gkmblgyl.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2oduefzsc.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fmxhqbuo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sexaqtkk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2tcnrxjbh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2kcxfxhys.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dehruqjw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tuvadzsq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2zaxcstkk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2tgzvdhpj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yvazkzkb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2frohrkcw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2xybppbpo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cgnybxig.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vsbnrtlv.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pzmutgcu.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2iipjcwjs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2armgcqqv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2urmpksma.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xqggrujp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2wcqprdny.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2levtgkdq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lmfaguxs.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfelzqg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2astgagua.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2msgfpoks.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sabwdric.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ynkykarf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oqlejalw.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mtsxrjnp.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jppjchte.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmzjnmd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ccoobvbm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgypfcv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2ypcucsfe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2icneqppw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nnfqugbz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xrpfvfpg.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2djtluayk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2riqhsigz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2eeqjzulu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2gmrdqgcq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2liufteda.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jextohag.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2rbnxzyou.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2lfcjwgaj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lorrznbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gntawxtc.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2slududmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbbifjmp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qaixzyle.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dkibikbj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2uiyknaqu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mrzhiwck.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bajqnbjh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tegornbn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2igthbykp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jehsjbeo.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2trfbnfqr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2aqdgtixl.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nceddjfs.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvucfpnd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nmalnkkb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2unpqatrz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jxkgmzrl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqhgdli.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cokxbudz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ywvsovzm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2kidvvegu.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xmgihjja.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iclpudxp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbofxfjd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2krwufxha.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oofqxdhz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zpuptkko.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2sfphlaoy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2jzrqbnab.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jhlilpyy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qgqeccus.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2aahtwcsw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2jnqewomi.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pgwbxjnw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2eqrbwagq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfkqnqgb.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2cvbribuv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cisolggc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oljrgrqi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2jztrehjg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgyyhvok.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtmvmtev.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hsbrtzuj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdupagk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zmxxoayr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2osskqslc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkttsxsf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2pflbvpxu.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2uemwscqn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlzkisti.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wailntmw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ebxtktic.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbejsdsy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2grsaypby.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2efarhuco.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jywkyxhn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ipqnivpp.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ychhujnr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cqnfytja.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vmdbkhyz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2msoknglf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nptcffve.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jszpoohw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqwixold.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2phfokjto.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2wgxckuxw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2qovgrxxm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2upqjqowc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fhzpltar.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wvkwfoua.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jsldgvcr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ravccbgx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2idajvwzj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2koxfbdqm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ngfugsei.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2sfhtmuwv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vuoleitx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmqhavbo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qzzjdcuc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jedfjtbq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfjtloqa.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jcpmopcf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbfmkghx.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2cpfvcvys.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uevwwqyo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mecearki.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vzxvpayw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wfbzudls.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvbfcncr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ztgyypkv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xxkoaxyj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2hhvyxfsz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2knvtccmg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ulzknacm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wtaibttn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2imlmasol.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dueoyell.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2daqmnnad.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vuyfjijo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2egmkadzl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xbvcbira.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2sqmxgevh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2nyytrtex.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2nmozchic.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ermpljod.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iwwnpjvr.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jxifyeer.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qtyhpvqx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2yyswmdoi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2smozuhpx.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2owmzkdrf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2syfyhrih.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2zbofhviz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hoeuyeta.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yejdocag.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ocbvmfkg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hqzbdzrn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mztevfis.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2acxlqipi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2yztlqnfq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ttggotjl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bkgwtbry.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dixzrqpk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tpuccrmg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nukjclep.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnghcwfp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2trilkgga.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tbiptksv.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ivfvifub.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2efgjabge.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hyohbutz.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zigfkzcd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tntojvbl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mlgdfkpj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2beignckt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pjxwlgbm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2klbgulmg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hijfptcj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2mzinwuzi.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2egqiekjf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qztdswum.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yyqbcfgu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2awlfjkan.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2wdvhbipk.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2zxkeymlx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hrcrzinz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkgozzap.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cjcajlpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqjogjfq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nouqmhdb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2betpuolp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkivtpoq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vosotgtp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bqgmwgnc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lghmwsqp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2rglyxrgj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqczgaus.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jggxtaye.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bzrvhhiy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lnpibqvc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rocvmxpv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtuhzwld.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2okuvkjkw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rsduhbup.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2owugruiv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pngwukzv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2lchtxuqo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbcwgbag.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2upizrlvu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2susrfnod.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzncppoe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ctvvthzo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nafjxbot.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dryhnrze.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqskurof.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oqiqarii.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2yarrwwjc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2odvmygye.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2jzlmlzri.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpfkxoox.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2iuixzpeq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2jkmvxeds.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2yjaalgyq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dbveagna.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zaokktrl.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2imnkcuxd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cylaemyo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wcnvbbgt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wddxjkgg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eopmmiix.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xkbyvzqm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jylgqtaf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gbpvxvwf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2itraqalq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zewensrp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ztwfmkdi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ytouesvs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ssajjgtw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2chsdivdz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gqhnhgzy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2pitvfyhz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mgwgjzlp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xmaapoel.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2aijwumra.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ltbmbyqk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybqewxck.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mgqdyfjm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xudkzzsc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pyqzmbtb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2snnuxwyr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qushvnmk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2etqqetta.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cblrmnfo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2puxocria.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdyfgrjo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaxyhfze.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqtxnmej.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2iydszosb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwuckvid.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdomdlpu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zovmvskn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2almbpfpi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2odigckyc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pvsmsngt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2njaqyhjj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bvckvcox.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkhjovyu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mayeezmp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2cxkwjjvr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jlfkwqfo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2eojaukhf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2suywstmb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2imxkdhae.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ofrtxuwf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nsxtpsgf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qvmdshea.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dzzkoeur.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2eymmmuws.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2plliztoz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mtdcuaie.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lneetgvw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vtqwhbqa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hbtijbiy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zvgvxjmn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vktxlgoz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2urvkqwmj.html


<!-- 参考信息 -->