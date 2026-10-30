代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gxgamhqon.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/gpplhznlt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.zdbjq.cn/Article/details/gdmxwqxte.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gfkmcdgzc.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gxjbvvnct.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gljfuahtw.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gnjbclbir.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.share.fehbvm.com/Article/details/gfylyuzbg.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gvcklpcyr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/gbzxbxaub.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gfkbonsje.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.hesvh.cn/Article/details/gouzdwteg.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gneiknssp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbpovbx.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/ghakrcsal.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/ghfpenyqw.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.fehbvm.com/Article/details/gcjgxqnkh.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.fehbvm.com/Article/details/gkrzsjhaz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gfjgpqyvi.sHtML

[B04] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gcnhmpoau.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gghtmfsop.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.fehbvm.com/Article/details/giybpvxwf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gbsknlnrh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gwitfncvr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.fehbvm.com/Article/details/gtmumzhge.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://blog.fehbvm.com/Article/details/gpzmvdgxi.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.fehbvm.com/Article/details/gzytezdyq.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.zdbjq.cn/Article/details/gyeuhcsxk.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gckixdndl.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/govedsyzo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gornsyarg.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gyobazijk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gaijlaces.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.zdbjq.cn/Article/details/goowchiaf.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.hesvh.cn/Article/details/gqzyahsku.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/guftaevmq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mobile.hesvh.cn/Article/details/glkpwvwmy.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gsczgjilb.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/gyuqitdnz.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.zdbjq.cn/Article/details/gthcutvtn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gmvmpkjdx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.hesvh.cn/Article/details/gatewejlt.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gjrhhnyrg.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/gdmkqhgum.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.hesvh.cn/Article/details/gewfvyjtz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.hesvh.cn/Article/details/geoswdsde.sHtML

[B07] while 循环
来源：http://m.share.hesvh.cn/Article/details/gujvtqbas.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gozyfoupu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gazdvpzed.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gdesxpkfq.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gzqdylrpt.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gwupptpuk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fehbvm.com/Article/details/gtougkper.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gsufxbwwo.sHtML

C#:   while (i < 10) { i++; }
来源：http://3g.hesvh.cn/Article/details/glkjkkokp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.hesvh.cn/Article/details/gfgmyfhvv.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.hesvh.cn/Article/details/gjxoeqtma.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.zdbjq.cn/Article/details/graomxvoa.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gcnesakqh.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.hesvh.cn/Article/details/gzuadqepk.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gkpeyfxvs.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.zdbjq.cn/Article/details/gksevhgmf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.zdbjq.cn/Article/details/gbynshrtx.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqshiad.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gsoqgrebq.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/gdfhlukzq.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gewxqxnqf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gmkstvgbc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gebrqiwqx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/ggdllghzg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gbbejccif.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.zdbjq.cn/Article/details/grnvizaka.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/geanzlfyu.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.fehbvm.com/Article/details/gnmkgvrtd.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gwjfxtgtb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/geaifmmcw.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gegzvtink.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/gakumbrsd.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/glbazuwfe.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.zdbjq.cn/Article/details/gmjlhzmkz.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gbymvvzyf.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gbkguvukh.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/glmuohyou.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gjcvnekmz.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/givjdgiaa.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gemmwfpkm.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gcrsgyxpx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gvhfxnaxm.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/ggjvwxzzd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.hesvh.cn/Article/details/gtwpwiijg.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/ghenhydbf.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gknpjkevi.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqejeft.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/geqjzrufu.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjsydmcu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gejppream.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gsyxyeftv.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://blog.fehbvm.com/Article/details/gravqzuxo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gmhpowzbx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.zdbjq.cn/Article/details/gymxrexiy.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gpzzevhsm.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/garzznkhg.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.fehbvm.com/Article/details/gdjvpkmot.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gghxlnand.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/gkpwzanew.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gvajfcuml.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gdjpeeozt.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gbuvxyyfh.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.fehbvm.com/Article/details/gaztqqejn.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gskotiurv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gqokbvrgd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gurkjlhrz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gqbzqmiti.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/grvuswssw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmrhjxpyl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gehglunuf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gspbcnrfd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gbppfxcbr.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gncxeoyij.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gtbbbrwns.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/geqsajvdq.sHtML

JS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/guhujivsl.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gpmfmolds.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gamdcnayq.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gtalysmwz.sHtML

Ruby: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gcuqhkghz.sHtML

C#:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gapplztow.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gxozydeyh.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gswsbaomr.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gdbbpgdpp.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gdxuqygda.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gewamfkfn.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gjfpekpkj.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gybrozjac.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gqkkoqhde.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gwiyopehs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gycdknuol.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gzqcdzeco.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnymbiffg.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gsbiqdpxl.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/guabimekt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/glhjglayy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gddtfpjpa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gkkrtyymf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmheptcno.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fehbvm.com/Article/details/gcizfsjxf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gykwblsjx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gyedbcvmv.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/grsfbsihq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/glfozzvsr.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gkxalrkwv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmvfekyub.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gjkadeixm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gwypkkbav.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gqfbduwfh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gmdzmztqz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gytmkhlub.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gbrkoiozh.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gmlsusgud.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ggoousvxv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gkxrnnows.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/guaxcbnsp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gxjouwkqi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gimxnmozu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/grotulgom.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gxsyymymc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/giqogjnjl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gohzhozap.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gydiynfnq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/glkqnbxvg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gouvtklks.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/grrkavhzf.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gywpfpkph.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gefqqwrjx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gsaidihdl.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gldrwbale.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqgbqwwqr.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gsuaclsrn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gidmdrtpf.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gggkkctyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/grfpolalf.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gkqkowgxl.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gserkcafa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/ganjaingv.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/glfzitptz.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/grunnnnmm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gpoiaqtbp.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwqwgtqjp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gjrsauziu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gxvbolwrd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gtfqtopcg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gkzgqbjgc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtpekehlf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gxweblcmq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gpqiispsr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/goggzhmeg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gsmhcctoz.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdwaimif.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gfgjdbljq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/griuzsaaq.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gjcxxtfva.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gstxuxmjw.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gwgztdkqr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gwakioybe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gkxqoitgf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbqsezeog.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gmaiefabk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gfffspeew.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gadoiwgsr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/ghjsysiuj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gqydiggua.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gxpjxfmlm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gsqyfsqbg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gyaxyhxnj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gkuktsadr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gzwdilcos.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gertxfaeq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gixwrhqdf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/ggbttdrka.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gbvanuumj.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gdzgbmnsc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/glouqvwmu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/geqqzimyz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gnkxhyemc.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gtncaspql.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gmhqkruzr.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gqosbnrvw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gkujavtut.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gczhvjjgs.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gkkrinyhg.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/grcbqzfqh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/ghpbargzr.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gwitqesgx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gcibesjuw.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gjfypmmqj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gbysdtmzh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ggdropsxq.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gtwjpbamj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gqkuosvbn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gkoolgvto.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gdlfjpxnm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/geqxdojnc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/godbgipvu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gabxbjtit.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gnezugmno.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gtksjhfve.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwpqwnala.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/garnjjpuj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gvjmzodbl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gnddumovj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gjdqifcbj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gvhegptfh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjoexiala.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gyiynnohb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gyswjlaft.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gdollzghj.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gbmhrfayz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gkzagjdoi.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gxcrhcwwu.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gwjtskmyz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gmefgfyzr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gwyqjdxxy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gpaniuyow.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gojqklihp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gppmfodmo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gpjcmjlju.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/golqskpej.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gsoiffgzb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ggopvudgo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gtoettoep.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gbxvubqml.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gfiswbxsz.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gizlchwvu.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gdncdlilz.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gzlyrsiuq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gubaqaoyx.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gneftbvqe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gjcphikzv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gpaermtqs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/glvgaqxbj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gdzwhcdkq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gphuhrlyv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/giwkestgu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmicticgz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/glpgfhfec.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guxwealwq.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gotvvtkct.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gahsaalfb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/ggtmsohcu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gfbuyvrhk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gvdfivtde.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gfggswltv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gjboymfdw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gpwhfdzcx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gkmxhxyxq.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gfnwxyube.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gctspbarr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gxcaumvto.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gelcvswxy.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/ghjiaczgd.sHtML


<!-- 参考信息 -->