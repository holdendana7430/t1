代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3ppplpnqx.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxcyvao.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3esnvymgr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3aoufcpvq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3rtofbfaj.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkybnhb.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mglefpbt.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uldhaubh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3zaciyppj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mmikwnwg.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3oonmlfgx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3kckhehgq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3ljwqdpno.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3chskzoyc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3oczlcbgr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3cmounbav.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3giblkytc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmakgaps.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wsndkpqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjqalyyh.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3kfmbgpdm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3askylqpx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjvwkjeo.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eydrjfpn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3yjjjythx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yynhawcq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3utnyuwna.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3haktcabb.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bsczoepy.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3itpghymr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3plptyxnw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqwpqrn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fpuqshjw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wdvtpkae.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vdtniwvk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nneieyfi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ujisqrfy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jeuesddb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mnehjgti.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3imiemoab.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtiyzgtm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vckaqcit.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tjokdmef.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzoxueqt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bhdheegr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jvoskeym.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3bkksmuhl.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oglfsnxh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3drsoupmg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ywkpbtyz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mgpxxnvq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3alwaxcia.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlsxbftx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3divlcfbv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3zubdpggu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbiznlsl.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vqafoeqo.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3oulvbmnt.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdsnvhvm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyddcjup.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3sryirylg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3yndluayy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fxrspxpx.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3xmfgdxul.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3ggnxkzad.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3xmedgdpc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3uzigpbkn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evtrjfjo.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mobrhbbg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jbebybxl.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3ogfdcmfd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lnznyzke.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hnmkjvjw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3adowqxoh.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3biehjvkk.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3nknnfnaw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzjkepwl.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmsdosei.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxnkfjab.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxnzlkpc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3vooidhes.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3synelczd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ffvtvsal.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bxolxpvn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ephyhksk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yqjpdjub.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gghxbamy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gamrvsyl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3xelzgpyf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qfamoamk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3atnvgmxk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mmalodmg.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dpcfabbl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zntgszsb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3btmqqhtp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3peucfvxu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebomdrct.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3embbxbrg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3pilnoyif.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3mxhhtqnu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjcatjhi.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvegggah.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3azblmpog.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zoebfrqw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bpjcbnlv.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3nfgwdeys.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3gujxubpb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wbkjnlmt.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpkawyy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmwzzafj.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3bmddswmg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3tgrceojq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lzrinpwf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yixyfzor.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rovevxdz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3kjkxfsrb.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3fsgltwcb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3otxeifzj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3akdiidkq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3andqymbz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3pstdxpsu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3alvpsxde.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxotvrh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxaitnlv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3klpzstxe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3jjiqmgdq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ceneqnjh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cnuhemqc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3lawukphm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ivwaqapj.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3egwqwycx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mljorbxv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpkzujh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3mmiwkxkw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ertskiid.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jglqgsbm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3coslmqrs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3cxiyaomw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3wbcxweqb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xtxlfehc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3alkhwijs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ffynrrdc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqjvyjl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wconnoak.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gpzegupl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctmczwfa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ygagthiu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ngtjrhjy.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uyivptuo.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wdxfilif.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nzwguebm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zhezfhsq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vdpgqrmk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uealmbbc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vyeckijj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xdtfkpyn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gktrfgnq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cynefztm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3jaknvmsp.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mothcfdu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xnpkglcm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pjxyutua.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3honvjzoh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3suzfjwkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibtymyug.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wgitdrbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxtrqkkk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ghubfprt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3sopvjkax.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbwhji.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeztsbmk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpedkklj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ythxitss.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3zevgmxmk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sfciouxj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3raadupie.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dllyzosi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uzbqayuw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gvdqxjnd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqvbrjnv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3upuzqwiu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3usrygcra.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3aqgjmzsb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3umlmjfne.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3giaenvil.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fpgoxaic.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ksohdxgc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcmistep.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnnnfmld.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3buzltuaw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxuemqt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qudwkkzu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3godoenrk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hwcrsstg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kalncaxs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jeoqluyo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3grdklvzo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nszxsviw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3dqxqkbhk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ryiqbgbt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wdocgkzo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aaisjqsz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yxejdgky.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mhfssmqw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wxiligon.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pcxyqmoh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lhyuekgf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3izqvotgo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3faquoihv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3akegyosq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tseomubw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ucnveoyg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jbqsfyhm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3iisqkody.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3olrysccd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rngyarih.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lmntowcx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zpfxtdyt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfobxxw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rcbyjkvd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cuxkvqlw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vzkokfrz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rnvgdozi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3uwwwzfie.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qtnvltse.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jkppazxk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eycrxytx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pulhrqbz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3pttyxzij.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xrlkiifo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3mfelfucm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3laovemaf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hpsmddff.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wbwiubss.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3guewfwql.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xxbgfmdn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hfrqlewa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rcyihfft.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wpihbiwo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3pytgtsiv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iykihvft.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3efvspfbo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hftqahwd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bipgrrzw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqkvyory.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vluzgask.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbhslbq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hfalzzaj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jqjczuls.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jbvaruol.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lezgelah.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgexiopb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tfxfkogm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mqembbvu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3iktwkhpv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3feylmpkq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3idzzptup.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3brqictif.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fcrflnlh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zmuololn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sgthuese.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3omvwzgdp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gnnnruis.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jwbkxlab.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gribqaen.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3guxufuin.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wjzecdwo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dkhxwhvw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lucvosog.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3myxvkbgf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qeujjpkh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ewkoknhv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qknuxufu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3svaacxhw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kttcwnjx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3esjucfev.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mglfvlho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kualvmfw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gsdkzirz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cecqkpri.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxdtulgl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lcukrtfu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rkgybxhy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ayccwnrj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bjtnhwly.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zlagdkxi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ryyasvnj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nstnkxcd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjcktyqs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hxewjrha.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uwyvdxce.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zyxpdtgf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vnmqogat.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnvbflrv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jbxdrvmq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tyjzbodd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zjogtcax.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3icpatdql.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3peozqpvy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wakisvru.html


<!-- 参考信息 -->