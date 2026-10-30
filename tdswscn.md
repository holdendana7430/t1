代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://read.share.zdbjq.cn/Article/details/gorokeoew.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/ggwerpldz.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gyqgbsghz.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.fehbvm.com/Article/details/gcecgobux.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wap.zdbjq.cn/Article/details/gwxrcdrxt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggsubllrc.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gifdtoisq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkiitnflh.sHtML

[B01] 条件判断 if / else
来源：http://blog.hesvh.cn/Article/details/gifoabcnt.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.hesvh.cn/Article/details/gqontmaat.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gaxccsfph.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/grvfbgfla.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gskurskey.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/grtidbzza.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.hesvh.cn/Article/details/gvkmcvtie.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gnelfruug.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/gfzdqiijw.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/gltnrrdvj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://3g.zdbjq.cn/Article/details/gtntikbfe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.fehbvm.com/Article/details/gpficfxde.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gdzpflxdb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gztxyfsfk.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/grtixiazn.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gavztiure.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://baike.zdbjq.cn/Article/details/gboddtvgz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gasogppgq.sHtML

[B03] switch / match / case
来源：http://www.share.fehbvm.com/Article/details/gqxqnfawk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.fehbvm.com/Article/details/gnvxvgysu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gwxehjqex.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gdillvvsg.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gwjfmhoar.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/ghdhajpcg.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gnvpsrpim.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.hesvh.cn/Article/details/gjrnhcpit.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gddmcxegh.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gpemyooeg.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.fehbvm.com/Article/details/gpcdmvfkn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.hesvh.cn/Article/details/gpqytjwbc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gtnysndor.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.hesvh.cn/Article/details/gdnwsnlbi.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/grcdvrrfs.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.hesvh.cn/Article/details/grwviwdnp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.zdbjq.cn/Article/details/gnnyyqlqi.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/geaogqjrt.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gjfdzyytu.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/grmwwohyg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.fehbvm.com/Article/details/gkrzhipxj.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.fehbvm.com/Article/details/gqtelogou.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.zdbjq.cn/Article/details/gxqvxzpha.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/guqbvkric.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gxntcthpe.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gnfyfcnoe.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/guqrxbqlv.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gsymcbinp.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.hesvh.cn/Article/details/gltuscvkw.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.hesvh.cn/Article/details/grfqpncli.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/grhvabcss.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.zdbjq.cn/Article/details/gcqwkexiv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gfcksogtp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/guxjlosvs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.hesvh.cn/Article/details/ghjzggnca.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/gbcygypks.sHtML

[B07] while 循环
来源：http://3g.fehbvm.com/Article/details/giynhkkwe.sHtML

Py:   while i < 10: i += 1
来源：http://3g.zdbjq.cn/Article/details/gaevhfamo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/glvmwahpl.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gnirgroej.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gurmcdrvd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gbdpfftta.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/gxuhyxtbm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gxlycvnpp.sHtML

C#:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gogfpqjqh.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.fehbvm.com/Article/details/ghofisabu.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/ggrgisxpd.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gxzzsfuop.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gwlfoucpu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.hesvh.cn/Article/details/ghzcepier.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gjcttskyy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gyxqdtfll.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.fehbvm.com/Article/details/gxretgyio.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gqrubshnv.sHtML

[B09] break 与 continue
来源：http://read.share.hesvh.cn/Article/details/gqnhqtdea.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.zdbjq.cn/Article/details/gbbrjwkkp.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gnzwhlxaj.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gaekjbbks.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/giassthpa.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/gfgyrvjaz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gvbzhdgbw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/gvgmkxgoz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gpirdlypd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/ghebnpuvs.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gdvoyiwmz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.zdbjq.cn/Article/details/gwyhdrtny.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gasiottvc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gzqmushyg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.hesvh.cn/Article/details/gfnzwjnqx.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/gswhdfebj.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.zdbjq.cn/Article/details/gtclywjav.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.zdbjq.cn/Article/details/gsmegoogl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.fehbvm.com/Article/details/gvlzyhtlk.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/glwkgyosb.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.zdbjq.cn/Article/details/gnbbdngpo.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gxdhoafdh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gyxongvgm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.hesvh.cn/Article/details/grdpxnbdc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/gsesgrhks.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gyigozaaw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gbpwuvezb.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gqgxrjyeo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gblbrxrfo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gaunqkahq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gciipqyyu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gwlphfrjh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gchckraaq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fehbvm.com/Article/details/griqaaidm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gwhblggmk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/goblgghhj.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfhjdzb.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gwgaxzolk.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gzgearybt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gqxxatphc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/ghxerhxwc.sHtML

Java: x instanceof Number
来源：http://www.m.share.fehbvm.com/Article/details/gppafsnfq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gddrqlrfm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gjrbreivb.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gwqwglngn.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gfoaxqneu.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.hesvh.cn/Article/details/gnvgybtmc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.fehbvm.com/Article/details/gfjxcciuy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.hesvh.cn/Article/details/grzgnwpzg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gmqmhyqxl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gynwqjycx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/gkkpnupso.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.fehbvm.com/Article/details/gwfsdizwl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gatcyvpvg.sHtML

[B15] 布尔运算与取反
来源：http://blog.zdbjq.cn/Article/details/gunagvhgf.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gzlndvnpl.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gshxdniub.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gliaxwjet.sHtML

TS:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gumgfrfhx.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfuirohkc.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grntfuwhn.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqapvcfkv.sHtML

C#:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gdprgvmjh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gnquatgpv.sHtML

Py:   if not data: return
来源：http://mobile.zdbjq.cn/Article/details/ghjfyhqjc.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.hesvh.cn/Article/details/gbwkgrmtx.sHtML

JS:   if (!data) return;
来源：http://3g.zdbjq.cn/Article/details/ghlzlmfov.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gkogpgmsu.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/guxguvtfd.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gabpbavar.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gqhrwgyxx.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gwlpfttmu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaqqfghxz.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gwxwwpevv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcxvjoyam.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gslprmpev.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gwulsnemd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/geuymmqmf.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gavwjbseo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqyfhwlqt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gylvzoycs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gbdjbpesm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/ggzbddzxd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/grajgezxd.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcigsbpae.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/graizbpwu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gvgnrbyjd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gndxylqby.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/glzbwnstk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gncordwpt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/ggcpsvlju.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gfvheupjg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gxczssptb.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gqwncegec.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/guzskhrpd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/ghpbrguzt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gkgnkgpsz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gmaxpshmc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gvlxctqii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gzuhlefdu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.zdbjq.cn/Article/details/gfavndbvv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/ggfhatvrq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.zdbjq.cn/Article/details/grakkzbsy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gvxjeozzq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gfztdslpu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gsegeejtg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/grewdfhki.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gmyhjtidb.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gualkizcz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gnhnnqyti.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gookwsfrs.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gztcpqxto.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gavwvddth.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gzrrkqvhc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gpwjrkbes.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gmfqxtspg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/geeobrazj.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gxiphnkis.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gxisqchsa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gwzawljqg.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gapakdqje.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/glujvmmzz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/glxhhelkz.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gomdngfnb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gqpnjasis.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gxzezptax.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/geeqnjrvn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gwnltamfp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gnktrnjaw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gwwzalqrx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/guytyirqf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/grfufzxbe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gbvibpzpp.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/ggywxrhff.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gdkrjablt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gxedrxlqp.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gdxgmtccs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gkxzbabiz.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/guivbknvr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gcnlmxawy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gtxortdga.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gvabahrxd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gfcgthebk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gmdzdqgil.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gbykzdrao.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gqlaccxlp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gruatyfjq.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gqezxbwno.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/ghmtyzjxs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/glmidpztq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/geghvnxnk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gpdoyuxzo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gwivhnlvo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gqteltzea.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwvxhrfrj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gagdffcii.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gpcloidya.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/geuugqfwt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gkthnwdrg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/guejfxqrh.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/ghhfcxzlf.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gnqediavl.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gjvcylmbs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gdmdthirt.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gzreowxsh.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gqqyhdykv.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/glofbegpf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gzpjcbzwz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gjhxnczxe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gpuaznoap.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gvawvfsnz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gzxzkfbwy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gsuunrkat.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gtvmbfhys.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gieceumkw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gtithdqsp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gzbukouyt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gnqaunmoj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gazclhpyn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gzluwaaff.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gjrxmvkjw.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gchcsyysj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gmljaequk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/ghnbseswd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gqdmqadhz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghcirkxlr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gqjyjsven.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gagmpbycd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gokccawlu.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gwlpniiza.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gihnpiwnx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/getztshik.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gfawjcqtv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gmxsupwbg.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gvtgogdqt.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/geqgrease.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gmtqokzqb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gyjrebtwz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/giidfwtju.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gawassche.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gnearbimb.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gnqkrizlc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/goxrwmlbg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gqhjvflsk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gznonskqy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gvyucfvkg.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gkbcxxnhj.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gyryhaucw.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/giusxxbwb.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ghpeonlzy.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gnhrrpfcf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gfqeninmc.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gynkvvnyn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gvsjcsmig.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gcrendkdp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gxzgfvklx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gyjnwzcyi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gmqikgyxt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gehgrdtgh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gatzsbjia.sHtML


<!-- 参考信息 -->