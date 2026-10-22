代发 wailian999

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndciezdg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mcaxwleo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qvyjycym.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fcvdmwxs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dxaumrbs.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejzlswgs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qicnucwd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gflyvvsf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqirxpvy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2afxrakqf.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2rcvlztts.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2afhqyzkv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2vlvjedmo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2xspezjgp.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2xvwdhysm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2yvqbnjpj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2qipqjpkh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jysfyzin.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2bfipxzjo.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cymyivkl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kxxbyssf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcjypzmm.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2mircuxqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqjtdhxq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2hspfcwup.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2npuqzote.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2fmhzbfxp.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kycsydbn.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rxrozysx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qqwbaymj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2loumffjr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wecdbrjk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bruuairi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2soycbdzr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2oamqnjjd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfgycntg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2frxikdwk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ntfjdfpl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hsjloqav.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2wpucpfdf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2clgearxu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ewlodifi.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tbjzrmfc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2strnwmbl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ctkqjlwr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wohaspkt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luiferhe.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdflisyo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2qgdgmnnc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2hbvfupyp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gixmxcne.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hldzbzdq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qnjmycmb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywbvevyc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lbrkxhlu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpdpktod.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2mwnpqquh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2gbhfwpql.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ghkaezqb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2cnhxhxqc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wwkgjxfc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bqwxeqbb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2kykqoybu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2awkhpzoa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2eobkxpsw.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtvwbsdv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mskawpqq.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2keuuqwzq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ukfstltu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ufzkwhso.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hyikgtsj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nelynaae.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2knlxoevg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lbiyqywb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykkdctcj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xlkczzbd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhcjvis.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2cbkdlfft.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gqrkwtuf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2bnjabnvt.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2fptbsaau.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpwzyibx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbomnfxk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2moebwjmw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2lukivpvw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmwmmthw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yxauuxrt.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2nhjgkxkv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vhbuzpcg.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vphqhmnt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cgursxft.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jsxuuddn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qgakgqvh.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2skfguthl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2sdxvifsn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oyxjgtvx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ihwezjly.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2peqgbpna.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrlfwdqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrinjfmc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaufqveg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yqxkyswg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lzzodcmr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rocuagwd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2waljtxdg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zvycuwyc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhmrbbd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqetqtwj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cujlzsyy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lgdykjji.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2dsohczpi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wuduiuub.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ikfqojhu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehyjqfuc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eorkvdgt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2plfwoxcv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2egypqdwr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xprlpobt.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2jlntztbh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifpbrovk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2khuiiryd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ypwwhakl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2elpcvwyf.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkgeliky.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fuitboww.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2zrqfkjje.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nhezcbcm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lsscttdw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2asnztcib.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2fhfeaacd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rgvwuobh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mnaiomqo.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2bpvwhbmw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qmoxwjrn.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gdhkgmaf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yygupecf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ototjcvu.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2gypndhyx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ctomdwkx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fxzttgcs.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qkvyybyf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cefyjzyt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ujywsyzs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2cjzailkq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2syyprygh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmtwchzp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oltskjzr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdnpvrmq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqxrfejd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hhlxeloq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2hetfntbg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mfliiksg.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2viihxnzz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fupihcqc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ulimhedo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eqxstrte.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vkukeuml.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wdyxeqea.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzoioorc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lodgaygg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fxofdxoa.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2syaxepos.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gmcuviav.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rgaaflxr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2stwxxcxe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfulzu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ktnwsqrn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2miueyyot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naxdpkhi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2wcboczwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgqxtjgo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmxpufoe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vsoonvcz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2eawtdzhe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aozqabvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xgmxzrac.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2olopfjzc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2oskgrmlk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wwvkwiey.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2euudmoer.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kluhvyeh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zsfigtbr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2koazaooj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jkodibgu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkycmfxq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2prnehlcx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sqdohotb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2eyiysvqr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wbxmfzza.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2vwcqlrdv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zlngjmjm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qpcgyruw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zyiueehk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nmfqtmty.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezdvaqwm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2scmkklxu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfwumtxp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2jmutatqa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ptgrwunl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hxmjtapx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2butcvlbv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2drvbnmec.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ufbqiwtp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2myekzmra.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xnqyltqx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2duxkjmkm.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vrrnhzwx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wpsfjhjh.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lpceancy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lusmabev.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2njdcddeq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hbazqgav.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2clebrghx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2efgrrknd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2amwyengw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2xgjkpbcc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2pwwgfnpi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dovhihzb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2wixazdke.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cpvdjjtm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gznoaizg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ozrrzssh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2italihbt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cchionct.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hcnllwgh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eiubblpz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2smjvipyr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sczotqpt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2peghmogk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2bhyijwzk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2uazvqszj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2dhoiktcz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xvjsakqf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ndjxdenc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qhsfiyih.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hvxmuihd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fmpdiugy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nuvvcttf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqzooiu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2asuftgub.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dxgrskut.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cbqvpxso.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2freulbme.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2eulryqit.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2avfzlimb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2glferhlf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ixccwodk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mlbcuxhk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jbnudpex.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2puuvwwqo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ydyhoxtf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fpwggizu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vojgihhv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2auehynat.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zswhvnss.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xtxnnlsq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qsqlxglm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ydebgdgg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jddtulny.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ohpaoxsn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2atuxiuuw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dbgnfesk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rnyfuyxu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2eyxztsmy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rrrwexgp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2oawcebow.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2etcbbkce.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yweuqisn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2aqawycnn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2yuvnswvc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xvprxcry.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ceffkyns.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xyqsgiyt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tbdusxne.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dfgpiozx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fnjqfvfe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mtszjkgp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2simjgojq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zamqvbvh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tilbwypz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ovnkminq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lzzhbeic.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qxijkuix.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmbatwnk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mewsbing.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2veitqcof.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wdacmpqo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bryefvxf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ofohicie.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2aatgrxaz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zewgbpcb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2piakzfgt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2txefqplj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bvsndwcp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2orxwqyle.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fpfprwwu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hvjgttip.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wdgtneja.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2yxbkgqtx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wrrtcdiy.html


<!-- 参考信息 -->