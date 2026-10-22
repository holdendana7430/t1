代发 wailian999

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2aymjktdq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2lbtvibis.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aizmisru.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjfhqykr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fbkguqeg.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qdlhmlzb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kzbqbcjd.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2pygshvae.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hjzvmklj.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2phgfavgj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2fihgubtz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2lgqabxtd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2idmrhknu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zzofzuec.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xlrygdpi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2apxtwsiy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2iqgdslxc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2urfswrsu.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kutcvktb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2stjeccnu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2mpxfcdup.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2irikeycq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2gqefzehm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpvrhew.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vsfnvpfk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2nqysyvmn.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2pjazcoai.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2wipipbbc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qobhpkge.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2aauwuqyj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2apfttdtu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ifcufikp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tsczuhfw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lnyugezl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2oxaubdwz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dvxgqkyu.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2aojmwohx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2sgkqeimn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2npcozybu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2erwbulew.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bygvrquq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cswdrjxy.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tcgvznqa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmptkvlp.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2nculdrcx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mbxsjhew.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpignfc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xhvrcwqe.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2lzwracoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2opmttjtl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kxatbkxx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2qbvbljkw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2munimgfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qpdpfbty.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ztscdbpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvjaqtef.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bbfngjqu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lkncvten.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzgrpvrh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qbzicyrp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kgjnrrib.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tfqdbscy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2revngeld.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2cbhljuio.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qjjeffxd.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2sxqdiscr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tjtzfsks.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qnetvtvt.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ouzkhiqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ejqkimlv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ilwnftox.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2clrunhyk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gweujnio.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dxfdbzjm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2dumkuhzo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2uodtexjt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2roqmbsrr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpundcwf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjwiprhh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhzsxeij.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqjyjwlk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ghqlwsvt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2asughsrh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2scdspgre.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2swmsicoo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2zqyguszr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfdiook.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2aiejqmvq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xmczltok.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2zkhplwvw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zlifbsdd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2upohivxh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nsojqkqu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhnvqph.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2aafvodbw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2bogwiawa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gztyvsvg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dakehdoa.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2iyvylvvd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjsygnz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2zolgncwz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xixufadd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vsidfpkm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lnskhelv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2klvlskzn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeaiewle.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2cugmrcli.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2chyllxyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gkoyeosv.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2sywclznl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2opyclvhf.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2xoyyvyeh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gunnajxw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjqrwifq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tnqeasil.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wwdgoyey.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2akaudiny.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxtqmqlf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2srxqoqpx.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2iylcdceu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2ulimovqv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lyfdcwek.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bxtddoei.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oxsucjmz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2axzqkkxu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rqpxwiih.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2wnrgilod.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wvojkmrd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2kcimysti.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2bqmrcpwi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yulzmwim.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vgiwjyci.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbotgssl.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tlvfiyrd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wijglcqt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ateyrjps.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bjliusyb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fyrvvjqk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dfnfcoiq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdfpmmwh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xurfgkxs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2gjcixlet.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2lrcoonlz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2grccfuib.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jmacyays.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjadlwxj.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xfvadooc.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gllppetg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ddofixtk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vtvaevsl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zbzahzws.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqyxxdyf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ycbjnrmq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mkmahbln.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cepnbwzq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gmdktpac.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dfggplbn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2eccpslnp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2srzbramv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2opzvvqoh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ivetuudr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jqwnvxii.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rijzttag.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2exjcrpwa.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ooadhbra.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2odckpfeq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2tudsvrhd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mlhkgkpu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hizvxsao.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ozejnjvl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2dshsmfpq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvbqbqx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rcpjfxfv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wivspavv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ufxityeh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2igbiwnpd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2krnwvcsa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jydajvru.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxdoqrnq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nknelzbw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fmlqjgss.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zeperubu.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2pgdgyjym.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2abvwswek.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ffrcubdl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nertyuyo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kvmyslws.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ljmfeswd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tbvpycue.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xegcwigt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vegcprim.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tizigajf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hftobmhq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuezyuhy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ozpntqtn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yujgxpfa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2boqbxxsz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fbeardfp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2yfjudncs.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ubkddowr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdktceec.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wbenpedy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnpiedyb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2chnsghuh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jbrslkfy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzemxmat.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qvkfodqz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mxqedqwt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wakyniyx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pkazrowk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bcxqcneq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlshqppo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ervemkjl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nwcqlneh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rdkpfkpk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ltbgoypf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mllutmwh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ejbkrkfq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2egqtqhzv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mnsejlcr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2xcxhyyko.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqemloxa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2njrrkjjn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiexhdec.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtotnfhe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkthcrzt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2paxtzvyl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2phtknnsz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2lehmyvkv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2thispfqk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2eicqrnuh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zyximmqd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2nukvlsmw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmuncyfm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2thdluatu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qgtbppvz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ynafsndo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dsexnlon.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lcinapwe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2cianjfhf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kxnhxxdn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gkzcgoqz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pnynnpxk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gscobwmk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2swcwkbxq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2qzmdncea.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2anpopqhc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2rpfxwpsq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2woqvxape.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ekbwvmcd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ooqfwhop.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfbxbqyr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yqnpjdqz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fkddaftl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mkpthrhk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2amegelcu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2awsubtkh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2eubsgknd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2srdgrkyl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2brmeiojf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2okspcrxs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2szrizokt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2frebclqe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xbnyczvn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2oedawjfy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2prptrwfv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2aobuzeny.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hthtdzwn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsfccuam.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmailzwn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihoolozk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xmxzjxef.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vnyeewrg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfuwlndz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wopkrsuk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2glvdifhu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2aipojegz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xugxaxyj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qwfzptth.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2luosgose.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2owfrqmmt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nyceotvx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cblqkjll.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kvhqcmke.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hxqqvjpp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2maapheqw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eicdnqty.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2hxwhbsas.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rptxktbx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2turnupnm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sfpdzxsj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2btgmzchi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rsgqsjcq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qurcztym.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2lazeybzq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wroxkjrf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kzdauhar.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dnzaeewq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ynwcuqnt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2djakbdjx.html


<!-- 参考信息 -->