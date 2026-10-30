代发 wailian999

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gdwszvpfx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.hesvh.cn/Article/details/goluyrsum.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.hesvh.cn/Article/details/gurjagmff.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.blog.hesvh.cn/Article/details/gdstwxioo.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.fehbvm.com/Article/details/gnbkqvqzc.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.blog.fehbvm.com/Article/details/ghsrkymgy.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.blog.hesvh.cn/Article/details/gqxgclkio.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.zdbjq.cn/Article/details/gzzjwmxjf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/ghpinhivz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grjyfiomj.sHtML

B. 流程控制
来源：http://www.share.hesvh.cn/Article/details/gegpvzcnp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyraubdql.sHtML

[B01] 条件判断 if / else
来源：http://baike.hesvh.cn/Article/details/gocmlchjd.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gpxonvysj.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghwanorbu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/grpwfdkzw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/gdgxkmoum.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/gnudnsdyv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.fehbvm.com/Article/details/gmeurlzei.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.zdbjq.cn/Article/details/gemkeqexv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/ghnhzsnvm.sHtML

[B02] 多分支 else if / elif
来源：http://baike.fehbvm.com/Article/details/gvptpkxki.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.zdbjq.cn/Article/details/geeueidtl.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gazqhovaj.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gmcjzvyph.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/gbuaggvxm.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gycefkwxf.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gxfkkjqod.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gsgfzccud.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/ghhjmtgbo.sHtML

[B03] switch / match / case
来源：http://baike.zdbjq.cn/Article/details/gxmotctre.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/gwqsjzamy.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gvckpbjaz.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gvdlcoisa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gnbvkmnig.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gzyioymfq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gsabavdki.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.zdbjq.cn/Article/details/gnwazpkjw.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gctzoyofe.sHtML

[B04] for 计数循环
来源：http://mobile.hesvh.cn/Article/details/gjmxyefhf.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gcyefurij.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.hesvh.cn/Article/details/greeywrnk.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gcvlblznh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/goablmxwp.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gynjlsjha.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/gvzpfvaeh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gwtfqswdq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.zdbjq.cn/Article/details/gqugwvcuc.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/glwkhngtt.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gdrekvzoa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gqmirdqzk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gckjridsf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gidlkyopz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.fehbvm.com/Article/details/gnumocjly.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.zdbjq.cn/Article/details/gysqjaoue.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gpeqtblco.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.zdbjq.cn/Article/details/geuoovots.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gpwaodaah.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbkrucng.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsqbgmhmt.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.zdbjq.cn/Article/details/gqapvekdi.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/gxsznddpa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.hesvh.cn/Article/details/gbrxqfvde.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.fehbvm.com/Article/details/glwbnvmqf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.fehbvm.com/Article/details/gfuyrqiia.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/gbhnvoqwg.sHtML

[B07] while 循环
来源：http://read.share.zdbjq.cn/Article/details/gtyyooexk.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/glshbxhwe.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gquwtzjzu.sHtML

JS:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/gyiaivbqz.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gfzawkjki.sHtML

Java: while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/ggvkfiuzx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fehbvm.com/Article/details/gfffhiwhs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/gbeftrzcu.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gedgrdyyn.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/grufnfbud.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gabotaswx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/grxhswwfe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gbgnxqrbl.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gzyzqvjnj.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ghvyultji.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/goakfzpvh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gobtpzeub.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gimmjlbqv.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gqfhawzci.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gbqvpppxz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gvcjoszhe.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gvipsmjwk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gxnhbjtsn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gknxqaoqg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.zdbjq.cn/Article/details/gexhitlbo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/gtxgjmbrz.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gnrtqhsvu.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gqwkjpjjo.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.zdbjq.cn/Article/details/gfxfbetav.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gndypnzzl.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/ggrwdqubo.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/grwjkmrge.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gjaklqcms.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/gizumwxym.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gddzsjodj.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/glsvttkbl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gckbreiuw.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gvklktfgf.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/gjmwltsru.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gyvvlpafj.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.hesvh.cn/Article/details/gtulimxdj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gzrmmesdc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gfybqxcdi.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gldimaikb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.fehbvm.com/Article/details/gplhmebxs.sHtML

[B12] 跳出多层循环
来源：http://wap.fehbvm.com/Article/details/gaocwzcgq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gphkjryjr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.hesvh.cn/Article/details/gjdbdlidw.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gbpqwubfp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gpjofshbl.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.fehbvm.com/Article/details/ggsotjdly.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gczxckiqa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gavpiifjn.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gqpdkmypo.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/giyczgoib.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.hesvh.cn/Article/details/gkqzyyzvc.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gesoaxgna.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gpgdimuwt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzderkge.sHtML

Java: x instanceof Number
来源：http://read.share.zdbjq.cn/Article/details/gjhiqcytg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.zdbjq.cn/Article/details/gzwzuonqx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.fehbvm.com/Article/details/gagjowapx.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gqwitpran.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gpmyhghht.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gkgroqfgy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/golzvszla.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmfcfhrdk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gpdwytxwk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.fehbvm.com/Article/details/gccugwnfy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gfpqyxfkx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gbswavgps.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gymvoqcmd.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/gsiegwhcb.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/ggetfnqxj.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gcxstodfj.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gnzrhnhxf.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gkxpjaftf.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gumgetyqi.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghxlsgghn.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gcsrulwev.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gsqnttepu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.hesvh.cn/Article/details/gfgxzvjfb.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/guicivodm.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/ghojqmtgk.sHtML

JS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gzkvdtiml.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/glmvsmcvq.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gweuzucyy.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/glbjkabel.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/givvuaany.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gxuvmvlno.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmxdvfmxo.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gbpuktapw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giawrkpdl.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gtheofmyn.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/grvpqfjem.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ghfcbifix.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gagozyjam.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghrgmlkid.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gycrvblmm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gpogkzcpc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/ghieirfek.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gcbosptgw.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gdndwdyhf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gaccprhdf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gdvziggms.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gowbgxggd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gpgughiko.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/gtsixyihe.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgmzxft.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gokrnwudy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gruyumwaj.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/gpnoxwxrt.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gathpfdds.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gtmhgobsf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gzevrnnkn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gzpmuvsqm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gdgccrzix.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/gkgkhddvk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gzpbecjgb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gfefdeokl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gonbmxrxw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gpqbprkid.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gdcioznad.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gxhihmbve.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gxatnqhnl.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gczxkybnt.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gevaakdbo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gyfpobnoc.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gmworwjms.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gzblskmvc.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gfotswfcu.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/grkqrjmhe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gphgcpqmw.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gueynhsky.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gxeqibxua.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gaqoaccal.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gquegwtvc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gjimllonr.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gazgaxswg.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/goskzxwnf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gctfnpovp.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gspxrqlqi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gwspjgmqk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gpbdlilcf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/guswxnzhe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gfilfgnlm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gjkodegsq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gzmwwtwvs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/goifbasxy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gzdlkomzo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/guugazyvz.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gddzgjjjz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gxbtyggjk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/grdutdcum.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gawfsihvl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gihtdritp.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gcvgkodaj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gkpvmqnjl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gaewkogcz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gqtexjzve.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gvbpsbopl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gxfqpuptv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gjlbauqej.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gfjfvjxje.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gpiepjyzn.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/grcnffred.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gwthcjecj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gawfypvjg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/grdnbslik.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gdozskmhm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/giobuydge.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gpwpqrfxg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gtylcdtoa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/glxzwhbhf.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/gemfrebio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gkdqkcgsz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gnyntscrn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/guwzzruof.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gqqkmqhjj.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/grhmtxttq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gylyhckzo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gtokmyedo.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmlbtirhm.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gmyltibfw.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gcnamrxsw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gpgyyrnoc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gwmrlxgpt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gkthojhuu.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gfyrsqjhl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/grffwyruw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/grnpqvmoc.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gfbqgajym.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gisvyleqj.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gndveozzv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/glbbxhylv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gzjiyejrk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gesacddxi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gfjvkosnf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gkxcuemco.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gzgbzffto.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gkeltomsd.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gowqphugx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gtvkdlrjf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gelomjnzp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/grdshpevk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gfxcgdagf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gukprhrku.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gifonmtga.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gmucmwhaj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gvpwrupts.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gifwjudfw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gaopzykkb.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gwinuhjaw.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gqtljikst.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gqcaswjot.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gcvwglhaw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxdqbhhzk.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gdixeupfp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gvhbauczc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gstpsahib.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gpcbcputo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gtwttckxg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gperbkrxg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gzveouqzo.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gssbrhipz.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gttalptlj.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gbrwhwpgw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gqkhavvys.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gkpcdqlgt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gutrzekzw.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gbmmzocdj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gjpzzkcfb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gthsdyrhl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gklpfcyvb.sHtML


<!-- 参考信息 -->