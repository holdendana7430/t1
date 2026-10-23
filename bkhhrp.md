代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3umkhcwnb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3luuoxiqj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3kfmzkqni.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3hcffkrfm.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ovqlpnll.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3efogypyi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3eojaiukd.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iqpdryam.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ugakeyjl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbchtxag.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3fwxpijfy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqkeosq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpkxvhos.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3ylucboqg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3sosfkuwj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrleqdze.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ktiuopkc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ysviftbo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ngiwqdpp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ctshwobk.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mpubxnro.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3iayinkoe.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3hwdimqrz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3eldecmxm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vomsfeef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raasbbus.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3acvjszjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fvaubmhr.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3jrmddotv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gpxklpab.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3lvchwdnn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3drktdkgr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3etmkcfqu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ykdhrvdt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ngppmban.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3niancvjx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3wvgtfcno.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3pkxxgyrm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3unvcsxyc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3kzvvhlwb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ilvitmwj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3szjcqqft.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aluahoxs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qewfmeqk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3temcgaeb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uugrfgps.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3tjbmdhcl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bqixvvxl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lizakobf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmphhmdf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nrzsbtkx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qubqyequ.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gtysxona.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ipjefjbw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kjgkacqs.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3khnvtxal.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3yowmyuof.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3keppwoyh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnqkgnic.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3depjvvpc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3biflqxtm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kgnwxajc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3qqonsead.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3uppkfbjh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ecwrnyco.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fmodahsn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3fcgyzvow.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3bpfkdcgw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mykusyog.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmrjyqhr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xaetefzi.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3hzalfalr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcqbenxj.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3acxfhmhv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3lgrxsuzp.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtfcqgry.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3twdjigvb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3leclfhcf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pptpnibh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yhphhbvd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3txpezigh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlwuobp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3vvzvgsby.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uotfuxef.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3vtuotkwe.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hlmilvyp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgbyawex.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvaioeta.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3hxxjhixd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3zwrfaasj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ratwanyj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3curyimzw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3yrdmlvxs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rhuuvler.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eptfkuyd.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jxwhmaae.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dvndmdox.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ptmivhrj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jzhrgnvw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jnnsvztk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mgkddowf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3inkqcrho.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzmfzxfs.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffsdmtgk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3udtxafar.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezxgelua.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhshakx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbbsfgz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xonybxlm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3wihnzpyy.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3uolfkyci.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ukfkgcuh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cekqxueb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3swxinikm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3oamawjel.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3nztdutjr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cmrlwotd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3psellxas.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3qkmgiuoo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3pficoikw.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bfoizqao.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nxbgxuve.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wdgclrys.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dusnjtva.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3qzuoeigi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3othdjdnq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3yldzgsmb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3prysltcx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3wntxnhga.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3phgvvegr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3byadcynn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3divtanmt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wvtqyctd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fupxyeru.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3cafsablj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3vswsieyr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3zwqejtbr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hjxuefgi.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cckaukxm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oyhvbtyi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gmbypubh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3vinatbek.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pawgsfei.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gkgusaaj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fwavggdx.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ffoflcxo.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dooublav.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3drlhkqmp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pylxljxp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dazjrila.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ouncdpqt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvworlvj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vrcnxvzx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnfwtlmi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3gdvjlzlf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3jyajhhzq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3eqiolkee.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xlnhsepq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rnbxrlen.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ypgecnfy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3amxaazsy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xzbcbial.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jhygzwvo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3itvqyufv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zbuovhft.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ebfuwioi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3puvjmtcz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rmayzqbn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dlbdftst.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtqqkza.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3evbommjb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gerncgmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpdjjwro.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3rmcmzerl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lizpreyc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rdcucclh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3utqeyybl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dccypxxl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3unvkusmt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvzmagns.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jypofvzn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dkkshgtv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jjsjjuwb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3opxlijpr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbzsedxv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3brkholzf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fpkghvjn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lldhclyr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lwaqkzuj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dsgndipg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3uphwqzwv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3buebisku.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gkymtpcj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ayyjbkwu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrctfxh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdgtxidx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3cxoxcrvh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3svkcvkqa.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3oyrkhbfw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3slrxtlqy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mzofiymd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mejxxhts.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xfonnrxk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzojpfvx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3paibzcco.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvxwlwje.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zcrsnisz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3guhoegpb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rgrsvypo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3byqaljqy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3htoearsp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3eyergkky.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3swterzal.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3suvnzrfp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vihuikog.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fyktwami.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ecsgykfx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wuxbmnjs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wjygisrt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3acotlnoy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3oqwfrjzw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3irpsjblx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3efcgilba.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3whglzmbq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qlqppdmp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3azwxfxhk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nesqnnng.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3mnngfpow.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bovrobuj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bfognuty.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3fwfgknfd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxylafdc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3emjqoqlg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3sfdcfsrb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppmwrhyl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3csoxymtf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ukktvtsn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mpragbrd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3julfgupy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dezxbjli.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3eqxuddks.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pnayjtbq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhsinyku.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3flpiyngu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bexkclad.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yolbbxnq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yqquzmar.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nytbhuun.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvsrznk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffacqabq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3necjobqv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wtfibdve.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qiqgzsov.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvnyecnx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lduhyeoo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ojmqmpxb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3abwgvcpq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ancxokwc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nheagoqp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xozagvnp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zzdngcij.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zkjrfdxr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nmaeyrxz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hsyxltxq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmcsljhd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dlhetlzl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yazdfkfl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rffzqrkp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3iwntfcyf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ozrwtpno.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ulapcvab.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3emopvpgu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jkxwnlcw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xmgtlwal.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zcggvpfj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3djdkwvzu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ysmyjhwn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hqksrmtb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uiqpkrqk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cesoxlhs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3yjlyyhpe.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ajfzobqu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rafniwxx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3cgctctob.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wbdtkmzu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqcjmkhw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xxqwmdpy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vmbydkpf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hurvudux.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3czwaqtyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3klzbtmen.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3hdqgnmua.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cowemieg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3defkxoft.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dxwxsrpv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mfwjaikx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iacarxph.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nbuaupqd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3osuvaopm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3enoqgsre.html


<!-- 参考信息 -->