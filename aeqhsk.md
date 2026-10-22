代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uezdgdsd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2doscyoif.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ygyqcdfj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2netkjaho.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2efdugwcy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2tgklqhot.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cybghhlz.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2aenseuuk.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vtyfqxhr.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfjrmlf.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfzjdrd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zixmzgqi.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2muierbsl.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ustnywjc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2lhhzfrlx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2rlgfnslo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2qdwpkonn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2vhdvrvjz.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vckfaeaq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2kpwyixel.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rfiwhomw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kwrwbqel.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2hzpbonmv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wgwniqqp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ncxrmhvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hirplafu.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hczfhpbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pmphlebh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2fkwvaxfr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2gerivoyv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dlfhlcvi.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kbgkdeqw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mwrqbhgn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nttestsj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2enwvjlgf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2wbiqhnxg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wmcepbyu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ieypmdmm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2nfhzqbkk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gpzwpyqi.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fblefqpr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ihuamgiv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vqojofwx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2oqhoquae.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2eplnnifq.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ccynuykm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tcaordbl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2mheummyq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ajlrfwbj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdravqre.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cucanade.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrevsnz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hbunimhr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xpvrpnyc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kaanplpu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2flsiwlbi.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2xfhlzvqp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2clfjzsww.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrpggyym.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uyphlmdy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mocqrutb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2xyhdhafc.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2olroylni.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2rultuhtm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vqzwafag.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2wukyyusi.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2gigvjulq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlzvjxsn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpufutr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2thumyvxd.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2cywjbakt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzfehku.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2grbnqtpk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2xwnklhby.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2btxvkvkt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygxqtizc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2izdizjij.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bshujnum.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyltmkbi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ebgzspjb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2jyqrddzz.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2flqdqfkz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sofctvzd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2npdxzlew.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2jboespsm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gjyjlcee.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jajupwqf.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqcovvtj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hrwsviyv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2hlawpxnv.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cljsrqnq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vzbnxjnd.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wchhoior.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dfrlgudr.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ovrdkhap.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gdxowseq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2brhfxrfu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ghgmkovn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2dhreqyxd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ocodzivt.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tubxihkl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2bqulakkm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqzfnzm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dunbhzin.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hyujyomj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvkdnbln.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zbkaqsnv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2rfdfhzso.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jkpdouwn.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2tfidbqho.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2djamqmtz.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2yzziarol.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xigizjzm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gtrjqggh.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2bfjnwbrh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2rqrebrnd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2eodfbjez.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kflxwsgg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2arorepuy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ablruank.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rpkcuzav.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vrrrobwc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2otelzamc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pdtiavzn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cvidtiak.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2gmljbudt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gyweosjv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mlodwmjg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2igdtmxzw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zdxkznnk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hbvhyazo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xxytnszb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qpowowwx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2slyucykt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2xyjqlxwc.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2thwxjdzc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ikmwydox.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ipbwqyee.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjsfmupk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsbvakku.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zrmilwvt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lxlriorh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2kzckwnvh.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2brfajusm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rbdcqlpl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2xnfrifto.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2psdbmycr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2isicdyfr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rfcvlkcc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kidzpwdv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vhruzbsx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbahcrvw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhsenmh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2riscddpx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wvptfroe.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yhporbru.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jabdnxph.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ucmteozr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zapwegek.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2shnbmdnt.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bnvtesjq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rirhskso.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dznkwstx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sduagnjp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zmnbpkqp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2coyukotn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mwafmeyf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2robxztkz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2krnahcwz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2lhzveuwp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nbsnulvn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yaabfktu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zunycbvu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2hhbowapx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhverppm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nqdmveun.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2amvzbunt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rlfyhien.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pljunapx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vxitjuri.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lwgboggs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zqqrhycw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2qrnkvcoh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuwtdulc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yrawwaqk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pomspjsr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mxzzjere.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2llovxgeh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqqbtfq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2mpfwnyqa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqwbzcoq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2hlaszqjh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kxazfvvj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fokzjoad.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dprnyqwk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ffvykdum.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hhvjcxww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ztdknoua.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsdnqwid.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2gqddhkkl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2mytahayw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gnjwytiu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fenjmraz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2gmalwuyz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2vabobhpm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kmssyqrj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zluxopor.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2jrlgdnxk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2zdswhwht.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hojzvjcy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2yftixjcq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2plsdyfku.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lsabgbnx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qnemfsho.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eoxdoiyc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2zgrwewdm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2daaxejpl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fwcyuazs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kxipkjdj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kpygcgnz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zqwdfuob.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2cikzxfyo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2plbzawpj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qggvqipd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yxeuocas.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bobakpub.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tnahdfad.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2amitmsdb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yyijpkqm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2qcytrxab.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2uspdyigb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbpxcorw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jrsnhoxz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ayoswykm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yacjnqbf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2drjqikkj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fpburcha.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2sskqrfea.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2isqblkcz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gsvdgeda.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzuwxkfj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mhhnhurk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lsjxgygs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vpqqxtxm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2yjicybyv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vklwviod.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jkdeaesz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gqxzjyyo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qctujypf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fcaqnoeo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tsauknub.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wnyqrbdb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujltlxeh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2psozjnqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwzoiaek.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jugkxcwn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ieorlvlr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vfjkfzjq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lgxgoulx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqmgfkiq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2blmjjxtb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sqhdzkpx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pjxngnry.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hcgcoyrp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fpmwatip.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jfqzlyim.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2thrgeqhr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2khoavyzf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bxsvzbeb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rembqqia.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bvafbwgc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cpmrtpkn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kaxzvhbr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xumkbwig.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zgnywiko.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2odwkrddk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xjdujrcr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pygsbvdp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iqudxxyg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hszlvaqn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qapzzjvl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gihvimuf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yxjzxike.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pgevarcu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jgiemexd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ktqgeuvt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mlttdnik.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtwajand.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqgpkado.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2csifbmmg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xpgxpxoa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gutetnix.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qkbnbehq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rhkhswqt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jquledrn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dxrcwtxl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuapogsm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdqijbyj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lbwlchhg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zqrxwxjo.html


<!-- 参考信息 -->