代发 wailian999

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lxqlfgkc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywbgqhaa.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3woasxmjy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3udpmjurq.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zhaynppf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kfdpnwpk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmujkiup.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3smdwtjgw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3nonlergc.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3loozruxw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3msjgdysm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdehxnlt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3iigzaofs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3bezpympp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3jeikgwvz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dumvrdrx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ilbexeyw.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3rbatypnr.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3kvzcuhmn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3feukyrad.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3vcjqwcda.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3volggzzn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rkxokbaa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3fkdsiafu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wnwrvbfw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qdvlxmix.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lffzonzz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3obuqwpbx.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3badpqwuk.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3dpfcufac.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3tkzvzxti.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ooeguaxr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3dytktkda.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmoorymp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3bbfspkxf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbuvklc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3siyvfyqb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3wuycxfbt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3fetdmgvb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jtzegqta.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3wjncacrk.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hmsglqzl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3bemtjkxx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vlyoajlf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vfosltgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiepmpjw.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3apnyycar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nyctakan.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3mbnqayuf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ylxivpnb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whjpdgbp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3seghoubz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3rouxebdb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iygpnswt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvfhguj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qiimmwro.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mklyirgu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rxauaoat.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lyjjuniw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjqjlofa.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xpercvkc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ouodesdh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fudzakvd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xokettgx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3rusbrbmq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gpffcaih.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fdwykuxv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3agssnobr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxhbhzjg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3veeicoqr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eweaeqwl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3piobxfeh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3kyrsouhr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3epystnxa.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3uyulhsno.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3iolkhwjw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3yvxkxkol.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3wumfrzdt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vggayfts.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3elwqryhn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3bngjexpb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3mriujoru.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dfeazwdm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3yfvmapji.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xnjtzfgc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nqvovvoz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3gyvlhsla.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3hwhsbelo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3twxcdnbr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3arddgqmk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vbbfsbzq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3huwqosfi.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjrnvchu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3uyasupbp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oaxfxfah.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bwsoefsi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqxbyqry.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynextvis.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3aarnsjpv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3utadzyye.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3rnnzectr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwiddeja.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3cdnuotio.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nldzuzqh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3yrdispbm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3toxunwjz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uapolpzp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jotmtvdm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3lilpkeul.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3eqtbvwlq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ulvvcfag.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xwnscpox.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3jlugllyw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3drkyqrro.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hdrgufxq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rqpkpvzm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3loqkvltr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3gsebrfeb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qolgcsuq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gboualfp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sunmcqcs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3dakeqeze.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3czpizoum.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mwewesll.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3vxispdzq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ttvttypw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ugtcjnnh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3oojutezx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dpmoblzl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3cumbuycm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoipooe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ltptgeog.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qgxeavvg.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qbjrbmtg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3lezfubmb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xetpdtzu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3haanotrv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cdavczgq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3gjdxtvhf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3vdigutoy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3heymxuxc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gjpqhvde.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgubiivg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3mlvuhynz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3enkvfjyp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3lpjvqdqu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3qyfsymyp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmqfbams.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ptxwveld.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jfyupabw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxhexmg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3elgdsurb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qoelcdey.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3dtwfsblu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3imvwdmrh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3qocxywym.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3cnioupcz.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3bwanktam.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bngjgror.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3udizceqr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gzlqhqwo.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3ulygdnoe.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ahzxuala.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3pvuspxts.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3czfdlodg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3pylsazyv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vlmosddl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3jggochbp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iminkpkp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ltqwmwzh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfyoemds.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzqcllbz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptqmshab.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hiuylutx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jmwsgacx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qflduqdx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3mzoefmtj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xwmdvdpo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mokotytm.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qxxmokxd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mjxprocp.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uroryytd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3fnbpjmfh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bqeqtmau.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ipnggaqo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fwmrgudo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ecteegge.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jvgxjwib.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gvhocufm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uvntyxmv.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3frlmqtpq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3silpijra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kembwxyc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ufzjymde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocpeucmd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3faqpeskd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yredhbfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mbbwrzke.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ofwwvgec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymdckknj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yeiepegt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yrgmvycw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zlyybmdv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcfqfubl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jlmctpgl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ponwonnl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nvfpkkqa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vtpstdmw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3plcljfhl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3baezeppo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvliuean.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cvkypsds.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qevndrep.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvbbgpgi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dfjxkese.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bqljcgdv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3stythqhf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3slszvhqz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3jerohpnq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lnjkurzs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3luyprekn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3uqvdherc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tsxodaqd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3irlztpxb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jitndhgb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bsfngcba.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qxjwmmol.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yvwqvdpj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3fchgbhny.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iawhbuuz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3niagcomd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nvnwargj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3flaqoljm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3inmbeuoi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zfrekskq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3enndmbyf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dgbxjbvy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xkowahyv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bllroros.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3seztcezr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dlewcpwv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3clmcnbxw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ixzxcpdk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kvqjydwh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3govnfinw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wxkgcdcu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bomahflo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3unpeigiv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gizodqcu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3qqqqpyjy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vrxfrtot.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fzpqeoyo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zwnzhpno.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3wwtaimmh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxunyxxl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pzcbbiln.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vxymigve.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rmsvpmob.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vzyyrufl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3euznkxtt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojpwkeey.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hegbjygl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ihnbdfid.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mbylabpl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubkbyoyt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xwkztyvq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgzylkuz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3smjtbxrg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctcshqgg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zusnbgum.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mstsmyla.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gwngeanr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bsovpfmz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tvnjcwms.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3anfndubt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vkxffciy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tyyjomkb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ogpmmybd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3eyqgecto.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3focaluqu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nnljuvve.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3maqytuvh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nkwgcxoz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hkypufuq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uerhdfbu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gobaqlgm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vfpnscja.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fzkwmohw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3znbulexx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3noyweysa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dhfkwhbd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dzoqahgw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bkfimwru.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cqqvbgtk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ygznmiac.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3outnipcm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3opxndovi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zgaxxsfr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vsgeamvk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3azeosrcs.html


<!-- 参考信息 -->