代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngekibkz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxpetlzo.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlrvxvxj.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gxqkufdiy.sHtML

[A26] 类型转换总览
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceloymdv.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fanxiaobao.xyz/Article/details/gfocqikro.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqbankmn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmcwznmu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzeiudkg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzjotbut.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.fanxiaobao.xyz/Article/details/gogozypqb.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fanxiaobao.xyz/Article/details/gowwpraml.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/gagqmlewp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdwjqbhla.sHtML

B. 流程控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslmxwqnb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gejlsvycu.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkltouqhn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavdyluw.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbzfezmv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gvjuzhkow.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygwqkawe.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwnzzuta.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.fanxiaobao.xyz/Article/details/gftoslypa.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fanxiaobao.xyz/Article/details/gmegjgidt.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fanxiaobao.xyz/Article/details/gnoircecp.sHtML

[B02] 多分支 else if / elif
来源：http://3g.fanxiaobao.xyz/Article/details/gvuxdfpbk.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhulqexp.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtwvnnjc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyavzeypv.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fanxiaobao.xyz/Article/details/gvngeiqcw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjkxzyms.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpsybjjx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzdtizyg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/ggukytzze.sHtML

[B03] switch / match / case
来源：http://blog.fanxiaobao.xyz/Article/details/ghpmtjxhf.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fanxiaobao.xyz/Article/details/gysuftdnw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gumvrwwph.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gotrvmskl.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtjsrunm.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpfmjjvof.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gvixecxju.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczmdfzpc.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkdcuxji.sHtML

[B04] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnhcslkh.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/guasgcqnq.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwpfpmpq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbnfybesl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeyscwxb.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyjqgcdlt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fanxiaobao.xyz/Article/details/grwfjjpwt.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghsqmlum.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapbzittn.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gaghotsnv.sHtML

Py:   for item in arr: print(item)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhdhqbjg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhlgcmbb.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghzsnpgvc.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkawowlmc.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gckegcfxr.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.fanxiaobao.xyz/Article/details/gfqpanuim.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.fanxiaobao.xyz/Article/details/gywzzfxsb.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbwuarox.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.fanxiaobao.xyz/Article/details/geaerufgf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoewxjlb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkljqhlqq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmqlworb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwmiqzsy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gujvappup.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.fanxiaobao.xyz/Article/details/gldtmehgr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvhdcdcn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbndgpxei.sHtML

[B07] while 循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopxivxyo.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbmxnzyb.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlhfxcfk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczqybynh.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gklavfqda.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkydqocy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fanxiaobao.xyz/Article/details/glscvwpwp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnkwdumm.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfqvmuyw.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fanxiaobao.xyz/Article/details/gbbrjmhrl.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwgkuzgl.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gldvluyjz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxswphql.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fanxiaobao.xyz/Article/details/gszrmwsmb.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.fanxiaobao.xyz/Article/details/guvgldgon.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gikzsozhs.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fanxiaobao.xyz/Article/details/gzxdeflhm.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuoabemr.sHtML

[B09] break 与 continue
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqeehlpf.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsymlfjj.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffieospp.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsovrjojo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwfcitpk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjsnwkye.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudhlvrrr.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gmeeoajso.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwnxtpbea.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fanxiaobao.xyz/Article/details/glgdaethb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gstvucfua.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpjprvyo.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fanxiaobao.xyz/Article/details/grqnhipix.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyfyodrv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjwxwnyxy.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgwkantc.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixqeribl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsqpbhfx.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxmzbffd.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzxnpkyk.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqqxintr.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxxbkpln.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gsjbrcjwt.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdvgscy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrbzieox.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.fanxiaobao.xyz/Article/details/gxspeuhpq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/genbadeey.sHtML

[B12] 跳出多层循环
来源：http://3g.fanxiaobao.xyz/Article/details/gjdedmvoz.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjogdrte.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmwlmglz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gijillemg.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtvxjwtch.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfdmreim.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guudwlthr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fanxiaobao.xyz/Article/details/guglytocz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fanxiaobao.xyz/Article/details/ggxosmhwa.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouxnbhgd.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkvkupce.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfpyqmfms.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvieoqlig.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggluwikfu.sHtML

Java: x instanceof Number
来源：http://3g.fanxiaobao.xyz/Article/details/gznucknmr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gelgimhis.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgjlzsqx.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fanxiaobao.xyz/Article/details/giebpscxk.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gukpctsik.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngaxfcvb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsszjzfim.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghobywpuj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczatoogb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvywibmv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubehnzvp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkbiejlac.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gckglywqa.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/guzsiwirs.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfscetbm.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzuraqgf.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaqgxqjg.sHtML

TS:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gvyhnyixk.sHtML

Java: a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gsngouaov.sHtML

Go:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/grrzdkwcj.sHtML

Ruby: a && b || !c
来源：http://m.share.fanxiaobao.xyz/Article/details/glvuvcihb.sHtML

C#:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykaljisf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gxtnqeymp.sHtML

Py:   if not data: return
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsybarxq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfmtzgut.sHtML

JS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gzxrqgyrs.sHtML

TS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gnzmkzxuu.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/golgdvnoh.sHtML

Go:   if data == nil { return }
来源：http://mobile.fanxiaobao.xyz/Article/details/gettlcesz.sHtML

Ruby: return if data.nil?
来源：http://mobile.fanxiaobao.xyz/Article/details/gibiwuxvf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsjytnyi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gccmchodm.sHtML

C. 函数与作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gupxrlesv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdwzbuhq.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gyhqbwlvn.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gufiuboud.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gexyjcyku.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcwshhtru.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjuhsnxzh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdomgpxfd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gloaqxixc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fanxiaobao.xyz/Article/details/gaclodnnu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwchuizkf.sHtML

[C02] 默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/geugeugwo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdiwrcto.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghikptsap.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gotudalej.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhfivbaw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fanxiaobao.xyz/Article/details/gxhkmsynk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqllbymjg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapiignoz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gurlxjpjw.sHtML

[C03] 可变参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrrefcmb.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/gcyxiuwze.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxhgimyf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjcveoqt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gomzamhci.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksnnrksd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fanxiaobao.xyz/Article/details/grtziaxfz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fanxiaobao.xyz/Article/details/gitqidowp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fanxiaobao.xyz/Article/details/gthlvpxdw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwzpgaz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcwrkheo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fanxiaobao.xyz/Article/details/goagokpuv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsacwrsvx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/ghqfmdhlu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqralnhy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazydymba.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gmytqktne.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwueabizm.sHtML

[C05] 返回多个值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzczplaza.sHtML

Py:   return a, b
来源：http://read.share.fanxiaobao.xyz/Article/details/gidzyeitq.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gilttxluz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsubrozb.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkveyntfj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqerwsjc.sHtML

Go:   return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gdjzviagx.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gohiyrynx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/giqcdzsqo.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/genmzqxxc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/glrqtgpsd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gzqhccbrx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjexyofgp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbrfylka.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqnnihbp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gkctepprz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoikznue.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcvxmdsy.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsojpcnh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjykzjjpy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/grayjnfpm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/glccdhzch.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/gsuqhfguk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/galjdeybj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxkeewqc.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/glgpdhgok.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gglkhasel.sHtML

[C08] 闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzcgasal.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gxnlbpwbc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwgzvzth.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmzfkskr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvzjmvkn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gehifrspw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxcvurni.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gllnliqda.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqgrknrv.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gnqazydve.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyerutntb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gonatxxyd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxtwlhs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/grimyhjhk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gsyhqclnl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjndkxglj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtqgxpwoq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqcjhlrz.sHtML

[C10] 变量作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdsaaqlf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gnscramba.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fanxiaobao.xyz/Article/details/ghxsjbsfa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gkfleftvv.sHtML

TS:   同 JS
来源：http://mobile.fanxiaobao.xyz/Article/details/ggasujmaf.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gzemkkeoz.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gszfbiiiv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gnmjbckdr.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxdbvbtc.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjhzwfkf.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepbvzcwd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdvcqsgu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gnasvrksq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvndlylnb.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqfrlkgm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqutahci.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gacbzeadg.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gqwzbapyh.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fanxiaobao.xyz/Article/details/grspjtaht.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/gbiymcopl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gsboamkqt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdrfgjjy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzscyqwjj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/ggxvgthvv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfynkrsdb.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fanxiaobao.xyz/Article/details/guhiylxkp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpepppajn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/ggryhdvle.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gidietkfe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdpjdindn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griizupas.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjklbruhe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywxhmjg.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqezncmoq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gexiouzyw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gvbqyhynu.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/ganziffdk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqaoouiz.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gcgfqhexx.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsioilior.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdpwfxlqf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gquhqiiip.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmzfwudq.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwjdmpas.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjgzkhtn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/gwxxlocxu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gpmafsovi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggttsqhgv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjraaifqt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmapcyhwd.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gbxwmpnrp.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/guaooitsd.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyfejbub.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gnyfndgpw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbfixzuv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/ghswarxaa.sHtML


<!-- 参考信息 -->