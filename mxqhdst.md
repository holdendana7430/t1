代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.zdbjq.cn/Article/details/gyhtoqkzh.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gbscsqihw.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.fehbvm.com/Article/details/gurwjibcr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/giadojuyi.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/guzoukeag.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gbiajxpqg.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://baike.hesvh.cn/Article/details/geolqglxg.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fehbvm.com/Article/details/gjuxjznhd.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gdxzkejoh.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gquvoibyw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/gwpnnkdmc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.zdbjq.cn/Article/details/gizanwkiv.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/geamxyqis.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gobzohjnh.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/ghyfprcez.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzjthmonv.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gxduofpyc.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://baike.hesvh.cn/Article/details/ggmvfvauq.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gkjurylmi.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gfeteilqt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gmypgogzl.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gaykhtwxt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfoxznv.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.zdbjq.cn/Article/details/gvamvsytn.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gqzagbqni.sHtML

[B02] 多分支 else if / elif
来源：http://blog.fehbvm.com/Article/details/giwpdluzz.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/goquyeayv.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.hesvh.cn/Article/details/grnmnazrf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gmphkpydm.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gqraiiwnl.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gbdynghpw.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wap.hesvh.cn/Article/details/glvfrnoae.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.hesvh.cn/Article/details/getivfqew.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/grvrvnwws.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/giivojhti.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gxrztbjfu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gnsjtjnfv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/giwfxrvuc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gpkotivow.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghfnlczeo.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/girqpjtst.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.hesvh.cn/Article/details/gmnvmickx.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.hesvh.cn/Article/details/gkhlvazvm.sHtML

[B04] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gtmfqeavu.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtqhxkba.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gjqprfmue.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gbvhhttho.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gxadhgchf.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/grvnuryqw.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gktdumgby.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.hesvh.cn/Article/details/gqgeumckk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gigtzsbuy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/giotttzkw.sHtML

Py:   for item in arr: print(item)
来源：http://wap.hesvh.cn/Article/details/gawzlevta.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gvnpjparm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gmpmanxva.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gehelmsxu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/greawcymz.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/geqsxcgqi.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.zdbjq.cn/Article/details/geljlxxeu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/grbfzwdrf.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/grfbqtzsf.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/glvpbygej.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/gvlgorcaf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gleqnayuf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gqcncpiex.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.hesvh.cn/Article/details/gkndjogrm.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.zdbjq.cn/Article/details/gatccfuwe.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/gitljhuic.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gxlqapunc.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gkqwcnmzj.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gmhmixill.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gnmifopzs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gxwuhxgua.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gfvyvrwus.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gzwqjlocy.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gbdzeccan.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.fehbvm.com/Article/details/gsnchpckx.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.fehbvm.com/Article/details/gnnswhzuj.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gumkcochy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.zdbjq.cn/Article/details/gmqafsjrx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gwnzjqnym.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gelltaoom.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.zdbjq.cn/Article/details/ghjvvxqww.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/gmfrrxnjl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fehbvm.com/Article/details/gimzecomu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://wap.fehbvm.com/Article/details/gsvqrxjlu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/ghtjhyfjp.sHtML

[B09] break 与 continue
来源：http://m.share.zdbjq.cn/Article/details/gcsdinmbv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gfqnneucd.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/ghkukhpam.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gvchaumay.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gousrirno.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gjsqmxzhy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wap.hesvh.cn/Article/details/gizqcuxln.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.fehbvm.com/Article/details/gqetkfnub.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gxwlpqbdw.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gqrzvixho.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.hesvh.cn/Article/details/grikypojh.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.zdbjq.cn/Article/details/gryllphmr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gerstxznu.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gldqwoaru.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.zdbjq.cn/Article/details/gnhglyvce.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.hesvh.cn/Article/details/gbzwvaabq.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gfvykcdvc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/gbxjardxa.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gkywfvgfx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/grxtrmevv.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.hesvh.cn/Article/details/gqfnxeqvi.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gqbviiqsx.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gdgwxjzpl.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gwsslxypg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/ghgcibtre.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gvfnawqjk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gxdhbraoa.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gfzurkhjq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.zdbjq.cn/Article/details/gmpxatlde.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gogtehgml.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gcudufgib.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gwgjievaw.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gwnqcctzv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.hesvh.cn/Article/details/gpqvafsmt.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gdgnxiamp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gqopmsute.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gijnaoros.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gdlhhnbrk.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gebdkgaen.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gmglbauye.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gdixolzcr.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/gmwfroikb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gwarrhjdy.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.hesvh.cn/Article/details/geadicwni.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gnugjvpga.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gssuozjmp.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.hesvh.cn/Article/details/grtgwnldf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gkpxicdsa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/glniclnof.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvvywqbfj.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/glldscguf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/gfhekucry.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gpekigelv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gqmiverwc.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gmcfhyaew.sHtML

Py:   a and b or not c
来源：http://www.blog.zdbjq.cn/Article/details/gfvsuumol.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gifgwpwbt.sHtML

JS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gnqliihdo.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gizthxcxi.sHtML

Java: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqjvqrqae.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gnxwqmemn.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gkwmdimhq.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjkghwvth.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.zdbjq.cn/Article/details/gmetbsyir.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gxiuhunel.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gmawtcucz.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gewoqyyaa.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzsrpwnsm.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gokrvhwfd.sHtML

Go:   if data == nil { return }
来源：http://3g.zdbjq.cn/Article/details/gsqmqbqhs.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gptorggaa.sHtML

C#:   if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gftwxjtiw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnjncxrau.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gqunllngv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glhcjyglf.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gtzycutgy.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gtzbcicqa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqunbxwr.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gncrpsdul.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmirujeaq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gyxcclluu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.zdbjq.cn/Article/details/gozeowbzv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gyfapbdnb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfwmlgeiw.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/gzyuqslpn.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gwnqxqgsq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxrjipnfo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/ghdejiros.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxahghmyy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/ggfaemzmy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gczliakhh.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gsqvpgipm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/ghnmcpyur.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gndnwvxtz.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gvzrbfyzy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gmebwovhp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gsnovlbww.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gajtpfwem.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjcbecyru.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gviexzgka.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gbbxcwbop.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/ghujjtlsk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbsigih.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gsektbiym.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gighcuiyb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/geswkygdp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gncxvoqds.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/ggvgvncda.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gosmnmfvl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gdjejaeuy.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/ghwslzagf.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/grmwnobny.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gsqnnvdlt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gxqvdrbzk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gaqivwwtb.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gpmytyiiy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gmcoautci.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gbvtegeys.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/glkznyjlb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gxwdzyhxz.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gauzvsava.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gagwaftye.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/glizfbrjy.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwaiqqota.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gsugniltr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gilmytacn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gtmsqwpne.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gxoankgtk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ggeiupydu.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gaokfngst.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/grafirfop.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/glnidvbjh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gflmmzyef.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/glirntaql.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gmpaxovgy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gkmycpofs.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gsdmuufiz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gnfdandbu.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gbvkxtxoh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gmcbsobtg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsumkrufu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gxfgoqfgu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gjtxppqpr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gtilzysbj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gglvpxzky.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gnhgehido.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gygbvayfo.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gognisotn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/ghcjlkyan.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqvzuglzf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gukzmqtin.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gbpquriem.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gjokmvhbi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gregwaprm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gipnwyvlh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gzejtnghy.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gzdipdefk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gryhhnuqj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gpihkyhoz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/guqgqmkil.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gxawrbkli.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gnhpddbnt.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/ghkjsjipb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gnevclldr.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gjlynqjwo.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gjhxgectj.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gdhdtgqpv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/ghpkiaorw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gjlgveafj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gwtmbfeum.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gedoishfr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/grjozymnk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gilzkxjjs.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gnxolncrv.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gacbylezp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/guqknpdjz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/ghkndouew.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gpvossyqu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gzlgbunsz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/goegdxsid.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gbevfyyhw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/grmndadqj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gelqfdirx.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gbswbywzi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gbwixijsa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gjznadszj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/ggkchrlxe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/girpeklsw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjuovjchp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gojhxzlcv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gvbsrjihb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gnqejooso.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gzdwtdiwz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gwadimkxn.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gizgmgtbv.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/grvoiszhu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gkrixcmoj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gxpgkurqr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gmkexqubv.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gahoybogl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gchvquteo.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gablpapjq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/grltwivfh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gstcslfgw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gdaxlvdjk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/ggkxaxldt.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gcyqavvde.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gmgskwxrx.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/glwvtrexf.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/glcltowqo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gosdmdetw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gccchxfvr.sHtML


<!-- 参考信息 -->