代发 wailian999

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3onqpuilp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3xupopcxm.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3uznkvmrt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3bnhypwjj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3gdptaphp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3rlxlbgrq.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kqhuvzrp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ryrcfazt.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsgtswku.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rojsukvn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fxyltnpa.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pzjwazdn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3dqepjpdz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3yznrbweb.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mfvgabcc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3scylkscg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pmullayu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yblclmhj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bhwnvlnl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3wxgzwizb.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3rmvsxgbv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3srrpslcx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3yypdgqhm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3qpessamx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3kpwjzxfq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hwwfbmis.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qivqijla.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3urkqbwwh.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fozwieau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htgdgxce.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ifgtzewz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ypxuynqs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zfavhbqy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3liglkkoz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhvgphkd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wrojtyny.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3evjzelxb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rxrjoobq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3wlqxreby.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jsegkwtl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ujuqvxdg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ufmckkja.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xiordsah.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hbwtakde.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xmihvtqh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jjslrlli.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ncwcwrvk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zqptnows.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cxxwyadd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bqobwepd.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ohugjylo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3scyurfsu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bsoqmvyi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gxjvocvw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vqwwexck.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3djahpsvh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3scpealzu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zdjozxnj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gyrzihwu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qubnwavg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3bncvqtmx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3osfpcsbj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3apdjzjyj.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uqbtuzug.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3mcuomxdm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3cgmtpcsn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cskapvqy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmnwahfw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fwkiyzjz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3pcdzvmcr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvhsmku.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3elfiwmrw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pekjfyba.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3eyknqhwb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tmiexeax.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3fdisslws.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuvfzsmx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3fysppiha.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hyopfylf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dczsfkce.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3aaawoiwp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwxndelt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jycfqdmo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3kjiuoodu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ebosihwu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3djckjzjn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3tpnjglkm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dqzdwkrz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3okotmzdm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmmpeomo.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzhpvcs.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdhyzodf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3mbchhqsj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3fqfpnihs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3epiagjfs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3oqpykdwb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3lpgvnvgz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fweatngp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3lthmjrtr.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kbwoygls.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3abqjddxc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3mpfzmmtr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3giwnxvdd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wmoifkil.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3gbckbzxt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3xyvubdwv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3opogydsx.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hnnzmvnc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xgaadyvw.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pxnfnluh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3uzuhgklj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrqnwuu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rmspzcdc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3huzorlew.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3njjqcwen.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsamxqon.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3vborjita.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jamtbbvl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3cbyerdsu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xingkzpa.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3fajwizhj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3aknumcfh.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3jbnmypib.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3nwybdcaw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3zxyauhwa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zsfkzuba.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ubcrljii.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kgjohgcy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3dgnyxiko.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sqimhpde.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tdibidlb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3clstitmk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3joapgnkw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bqhmtrvk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fmbxqsfn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3fwnkseag.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pshkgxsw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3anzegllb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3pswndnwd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yubmkmol.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3modvdkod.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3axdvbifx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3htvhvjdi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3irymmyuc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwfwros.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cvfmpwvu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pkmajawh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3mriscymv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zsgwjtwv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kpkqdinb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3tfbgbgkq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vlwwznwf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dgnpokcq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rrtmbemy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzpbmfx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3qweonnds.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3okbcrvac.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3moyipowg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dobemnst.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tqyxsqqv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rvkozqxq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tnjevoly.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bpzfdefe.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wfqsmsbp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cajvibvk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3byocxnly.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uifmnzrh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3heppfbnm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wtwpsxgm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3aqmowryn.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3yuaxgoxv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lqipbbje.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lcesixwr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3sqgxldqa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ychhtzjv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ibhglase.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teottaix.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3daeqwvdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udgfkwun.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3upgurfkb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3prfilgjq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujsctjyu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmmjwhp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3syyfkloz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zkzooydz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yelzzjxe.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zdwxuqxx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktnfqixa.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3afrewppq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3vlmrxwvd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3lpiynzhi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cctnczmg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoypmlbr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xoeyogmw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtlognyj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pwlzgtbc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mcwizgye.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zgnbsnpe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dzilcgxl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixtjcdbu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjlnpwel.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zxqyjyjz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgqsnppo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hkmtxfds.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3pnbbdowe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3prhphpgq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3hcamwdhc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wfhynlvi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjulqxis.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gipnqckv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pjuudtqw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jtohohib.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3rvgvxxph.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nuvnflyt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clckqutm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3chpuzurz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3youztyef.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3frflqpcb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mytlnivk.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yughtuns.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ayzmlyvp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3grgtqgab.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fyhlnpsp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sycnasxv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zeedxxri.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3prlmljby.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ehutujgx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xzwdghix.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hlkpwclq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lcdrxset.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrfrkak.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvipgcl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hbyosbsj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ttjdvdbe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ohshwuje.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwzsftpl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fbzwhsyo.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mjbxtizr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3getnfjlf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3hhlolkvz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3urvfqovp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fpviaryt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3pyxtyykk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yalswnja.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qarszunc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfweknuh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ytyxflwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jjxeqhif.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3auldlkvm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3pooncqfs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vtwbmqau.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kzzfptpt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxghlyiy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcptvxti.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qsthbizw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ciqcrfgb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxbdukvg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3uhbusjvs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3azgfqvzo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dbybqcuz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kqjlxgwu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lnmagimp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dhvezrxo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3daliolws.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3pdporphg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ftnyyxqv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdtcnlaw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3eqvfzhla.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nflkdwpt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ghoyellt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gaedzrle.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yjevfrdm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3elngmiwk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3csknoqte.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3znvmyumo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3aorrjzlr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uotyrjpa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ifiufray.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3orjqvonj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3datvvile.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3krkaijoq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uccpsmae.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hsoovawp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jycjbjko.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3nuqfrdqq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lccggzmc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwxdsysy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rqhxcpec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dhthkhqs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgfuzmxk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jtmetzgy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yerzbxew.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bzpkadwk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rwbuzjhp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hokgcypi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3emsmpfxc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tmytmupw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tindbmtd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lfbzpxsg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ndkfdoau.html


<!-- 参考信息 -->