代发 wailian999

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qokvakiq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jvxcxfcq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwebyzk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3ijjchibe.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3olqkibuh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xaidyexm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3uzfjpqyu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3agciosfj.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlgtlqsu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3lfgkvwpp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqetqgbl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mpotxevb.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dnhmifmj.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qvnqfyxi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3djurgoxy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3arultqoa.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ivgzajjp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3owoxxscv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3laveudzb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3iivyvpgi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kytfcwoa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3sjkefsiu.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3pfkswkbx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tlgvuwdf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqdmvkc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yzlegwvg.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3spxgxbua.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3srrxfvtt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3exkppwxa.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3imluucyp.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3yvqevbsy.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dfduuaay.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dfwgadvm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nalahosc.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrmzjpso.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ddwwvgkh.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbkrbpxc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3eepfbnvu.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ykqpxqiw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrdsdcd.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3vdzmjtmb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3sokdnvhy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ezrokgge.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3cnrwbvjf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ehvptulb.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3xcfgxmib.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yvhdsrgh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3kijgvxxu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3ubrunstv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpzharnd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3szrgvzlh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkmdprsr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gyimneaz.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3lloevmfr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3dyyjztzl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dxhpbqpx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3knqksfgo.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xbnyxyhu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zzqayuvp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xkaipkyx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3qslbltsz.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3fomnxaep.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ceptwxsj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3wdigkdhg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fhreminz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cdnolaqp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uwdukxol.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmwyckl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3uirgbuyt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wnetrnhq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3rdgcwccq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3sivqmyku.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkeaywob.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txznmoic.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aswoshcx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tosrefyb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3audnxhay.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3rptytqnb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3aqkknbcb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3svspyakr.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3qbfjoxlj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ongqohno.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3vvclrfls.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqwbclqu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3oimrkwnj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3jakfayln.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3cryqmgca.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hetiifby.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fguvdwos.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ucmdzfkx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jztkagwi.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lpfydmej.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlofkcfu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pwoaxnql.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wfhekixu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3mlrxbewh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3gstscqoa.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3twgiuvtw.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3ixzeivwm.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vguonjgc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxtlfscs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3zbkfoghh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3iolpilgv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ibupcwyu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3eivdgchn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3dxkshvql.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3mfwsvutg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpgsfayq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiiximms.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kkxvruzj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fguhfecx.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3flwxvesk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jrlygsrc.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zhwiutqu.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3veqiurhw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3swjgvovq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jiesmubf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dxykxwfr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rwtmfbmy.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zbiqpsic.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kpawkadu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ngdbylet.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fnhcnisw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3maekvolp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sfwghrlf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nzuzktvi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oibkcusd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aevjgvpb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiftsniy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxllodta.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3idomlvwj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3htwmbuzp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3fgorfrud.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ohipvsro.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wnaricwg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3cqgadnfu.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3aqhsyeiu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wplkqieq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ppsanqzl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wehydjya.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhczalj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kzmmweqs.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3sbcwkzsh.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3orjmvdpd.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jeowqsil.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3shsyewpk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gglwgojc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fquhvjfj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dhcsczvq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rnzurztu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vfkmxxwo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lrzzuknq.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3pttpzwbi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ngfrlpsy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gzrlwdbg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hkeyvdds.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hdtbsmyu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3txikqiug.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cpdygrvo.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ineycorq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3eakjeksq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3thzdokpw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3omotnycp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3zemzdrqk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbhhwlz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3onbbrohf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hqscelyk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tjtsgplo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vtrmcpdv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3xghcpiwy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3twzfvobe.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nauakngg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3meercdaf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hqkkgxnf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tgpwelcm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsokuqh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3caadqoiy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gpjljzii.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vtaqqovv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3glamfebw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ddgcpqhi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zxzvjghc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oxuonbha.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tohvdlqu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aznzezkn.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gydumbuv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbswbeqn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3txadczmi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3jrtbwuid.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbecjvd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zpaqqufm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ijpnyuwx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ajcjfgwt.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3mcmloqgv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wnhqifme.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xwftvruv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcgxqrye.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hvegkdyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ooxbnpzh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmlvqfls.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3eaiknxfd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3skdcpjua.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrpcrxp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzxzabkm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3maoewrgs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3inkxbkvf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkctnb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jnnkyolj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dmlppljf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ounngrph.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofjsdraw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3atujxgly.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nktubnov.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ktaunsqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gfqwvcbv.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3muxxkght.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zlxsrgbb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fexaoyid.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nrowweam.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yorpbyjo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3leykitve.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3plvbqtin.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bazprgum.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3iqftsdoa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmusprnw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3oiaaescc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3scificne.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3llpqxyjx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ogiqnvaw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htirpxog.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3oblajhhm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3sughnfnm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3uvrezatb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3hnbseude.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ddyxeukt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3izzaxagg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lehqzksz.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hadqoruv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qogwplrp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nevryxix.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rvwjtucd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3iacjypqd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oeoemjmu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vynvrbjl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3wxyepyjy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3obyvweaq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3juejopiz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tmkioubl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ldbsxxuw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cozqzzaf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kixklqme.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uflxbkni.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zyekwuvc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wmlkzqfn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wqzdllot.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3turmedgy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zgsfacxe.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3zfzcjevy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cfrnjomn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zyzqxhfl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzjkvuh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xrwcuonh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ivbhpqyq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zlzurymy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qfytjvvm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ifpligxt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfsdwizm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gusosnrl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3stezobxx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3misbsiri.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vqivlmud.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hnuoykvo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3skhxazpg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rjseomvn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vfiuiqlo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dwcvzgka.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ratdqszj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dukakpph.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zuobowpg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mtzkkmtd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ktdyjdsi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gnkejask.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3sdjmtvji.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tdutlnoe.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sgxorgat.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uahdaena.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zqvfyzgo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qghjdwyp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nihjfena.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wjbefmkf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sumyyfbx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nqkdlnjk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kixyvbiw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3sawxyjcw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ioasrwvo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nwatijef.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3crmepkdk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3akjdtgym.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ynoaycpa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3eknkckiy.html


<!-- 参考信息 -->