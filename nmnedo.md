代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhbsvwmk.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kailfqlv.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2adylfvxj.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2aagfvkfx.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2haggpgfl.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2abqakuha.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ugllzmna.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jhlnjsvf.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2gqupjnib.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hwibexpa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2iglzsscq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2edfyagjq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2kvoycclz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdbodcps.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2azzejzuo.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tesawqgv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2nshgwmri.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fpnnympa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2vkkvnbuh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kahsqwaz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2xvqvhits.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2tsmgxdgu.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kibjglbj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dnoiyguk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wbdwxgjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vknzznki.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2hxiwghlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdvfngen.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mpeamxli.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2mymomidc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2dppsjrul.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rdlhdrfz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rsyuotgk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gemeorvj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jhetjwok.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2hbplnlkn.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zhkqyzcq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nxbpvilp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mybtrilg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwbeesxb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sexerhkk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yntagziq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2peecgcnx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2rrdlhbkg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jgxwjwrl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ftblowtu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2sfkerirw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wconuxjc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmepoaf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2thiimulf.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obahhiui.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2teqakccj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sufyyoxc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2bdxwbvkg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2sbspumfi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jmvadfdn.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2atgbrukn.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziypalar.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2rxrflbmq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bokshfwu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xtwyistt.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dwjzlfsp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2matbglog.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwwfziky.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2eletccal.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xmgbmkvd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2sqguzall.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxnbzyqe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2juqimdev.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2idtredzh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2jkjgpdrd.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2tbzswbxy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rwbwnrvu.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rthybxqc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2xajhksoc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhwimuqz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgggpgws.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hkuceyzm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahvudtmj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2heazhazy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qsifyzmd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzrvslnc.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yijfogvz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qmbkzrnk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzlllczy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ieeinrim.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zjatjbag.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dfmfedss.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2udhzptkr.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2zmduwhjv.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2euzsshlw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bvgwqsrc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2lscnitqj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zvmfenze.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wbawhbhd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2janfgdfd.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mclxagbj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2narjvsmr.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2usejswnn.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ktobprqd.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2aqzmlgkr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2zxigbnsm.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xxmkxcne.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lckizckh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2shymouzi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmtengln.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2nvgxsmxk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2fnghdvcx.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhdjkyig.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2phmvmpwu.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2kpjokmnw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2lqyosmsr.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2fsdsrncd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kthfgvff.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rjlpmftm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2edloqltz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vyscvjgm.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpkjmcp.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ctdorpec.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2rzbbjpuv.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mcranffp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2tgpvrmmd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xezzfakw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybsuyvyr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rrnphhea.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oroqpwsw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2twhknjrz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xguotgnd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2xtxbdsnl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ektirmuu.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qqhphycf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cnkgslfb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xvapjefh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2mosekgzo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2sqnattta.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2iiivwxyq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2sczwvemw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tgthtegt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kvzfqrot.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xnwsasao.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rravkpht.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2pgnkmjtk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tnhpgogr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2togidrco.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2elyqtfzq.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2iyrhbsjm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2uyixtkca.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2tdoenwcg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lgcpzono.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ffeuuuvx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2slfyuwqt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wbtwhztm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rcyyhgdi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lxvzjoar.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wqkldrmq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lauqacgx.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dcdhsxax.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xqjxmsuc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2apayibxk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtimqowd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cjvujzva.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2skmngtdg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zgoirzpy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xptzfurl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wvvrvfjk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vcunrmqk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wyxrdfgx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lxvhzuyu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vyjhpsoh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pzlvvlxq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ulxeslpu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2hqyewusk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbvpupya.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2opspertv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hddtxjjt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikvsksyp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2xxpoyrku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntsmuagm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvybezcj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwftqucp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffoakxvm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lagkvbke.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yfhsepou.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxjpwlyl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2uketjnnb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2qrevmssw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2rmmljecn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2inilofif.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2roapezsk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2jjhsxsoj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddwmhpqz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2bhgtpzce.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yguxazws.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wpcnytog.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ulwylfmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dccsddvp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jfuvczfr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2woozccen.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbwtmktp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tdvqzrfz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzgumlct.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pbmtksnr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2giklymdk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqinguuo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvcwatzm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2naejches.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2fhmiypli.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mhjwgbpv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ycbvvggj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vqxspvvx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2glougbzz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2efooxkyq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wrghmriu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mpzdrruy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2udoezyxi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pdaqvhla.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kkqnmtsc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2anobogjp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pcxvjzlm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2gjhaaijc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mwbkxyed.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xkhqikqy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jqxjgxtr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2myvoeuah.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ezdobrqu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nnlpjmlu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wbrcsgaf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vuenkwpo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2evbsxazf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xpxfuhbt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tgrcflia.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nvwokuty.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mcajvrnz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wxztfzrh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2gqxsbfem.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tumiydtq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2dwqlypdw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ivcndtmr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tmxjrqky.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2uoeebjiw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xfjoxjxs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwjdahep.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tpwhxevg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ysreasrp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pnkkrraa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrimmebd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnzylfvg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pjqkquxb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgbgcri.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ufeytfly.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jbblyzfo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nhznmldl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcqoftmx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tvhbekkg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2isifniah.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mdbqvruz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cyhlptxa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2oqdvokwu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dxrfprcf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xsgamytt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xmxwyoyn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fbwcojfl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2apqlnlzt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fcvflonq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dylayqyi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2grgzxnfu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2spbxfcxs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tnmsuikh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2yjacrpug.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pvpzfwlm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ttoitxvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mbnycttc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2shrdxhyp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ptfoicgj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ypglliyn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lxpkqktp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tnjmgvhh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wiekqncf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dkltkhjt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2osmihemg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vbzxcymc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jwajngjw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bjeqvqbd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2dvbfasog.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2izcskuyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2weftbnao.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xlaracui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2msbgfebc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xqmqweqc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lbwdkxze.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2evbhxbjn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gdjizfex.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bkapizzd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2qlkazuuj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2adyoqijb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lijcswmh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlyqweyh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2osfqbjle.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2xpjzjrim.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lsgesvsd.html


<!-- 参考信息 -->