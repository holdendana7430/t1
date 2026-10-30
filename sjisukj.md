代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gkjxoikoi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/goastjbml.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.fehbvm.com/Article/details/guipwpyau.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.zdbjq.cn/Article/details/glayjnups.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gurgwevcu.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.hesvh.cn/Article/details/gmbuemmen.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.hesvh.cn/Article/details/gpctlzqop.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.hesvh.cn/Article/details/gdvaaoxjz.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gkpwvhhra.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gbfcvcypf.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gkwfftaji.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.hesvh.cn/Article/details/ghywfmmty.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.fehbvm.com/Article/details/gigjjrenh.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/ghbzknnxy.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gvdhiteoa.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/glbhqaxmi.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gvmpdhobq.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gxppfmekc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gqoawebib.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.zdbjq.cn/Article/details/golmppkpl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.hesvh.cn/Article/details/gmstjywzw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/grquhzsbn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.fehbvm.com/Article/details/gaooutqhx.sHtML

[B04] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gdmfzptta.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/ghsbzfftg.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gbrgtdlpr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/ggylbebob.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.hesvh.cn/Article/details/gwyjymkdn.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.zdbjq.cn/Article/details/ggcmvzztn.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.fehbvm.com/Article/details/ghfuualnh.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.m.share.fehbvm.com/Article/details/gkdhtuako.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gxwdximqy.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gezxknzrm.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.fehbvm.com/Article/details/gjmhmfawf.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gurhyzmah.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/grvocuaze.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/gglyjghuu.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/giblochzt.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gsyqecxio.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.fehbvm.com/Article/details/gihykdtct.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gajyxngbk.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gcmqzrhci.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/ggeddxnce.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.zdbjq.cn/Article/details/gixxgnydm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gmahupnrc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.hesvh.cn/Article/details/gurckixif.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.hesvh.cn/Article/details/gczohdrua.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/grwlbchgs.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.fehbvm.com/Article/details/gskzykgki.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.zdbjq.cn/Article/details/gbsdjvjbz.sHtML

[B07] while 循环
来源：http://www.m.share.hesvh.cn/Article/details/gofvywlba.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpspbflyo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gmmyvfmda.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/goccyfunp.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gnjnlutig.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gckcegdos.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gkoxleedl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.zdbjq.cn/Article/details/gkkeawced.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gvwqcgddn.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/ggoigdvhd.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.fehbvm.com/Article/details/gvimpfawo.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gxvdyijgy.sHtML

JS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ggbgdxzvu.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gfgdludml.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gpyfvobja.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gbursgamn.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxeeful.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkmiolibo.sHtML

[B09] break 与 continue
来源：http://wap.hesvh.cn/Article/details/ghvyzbtae.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/ghrpisccc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gbodxxhtu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gdnlfgxad.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gpqlxoniq.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gyaiprevg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/giyprxugp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.fehbvm.com/Article/details/gmzsxpydg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gcilsdtjh.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gthrchwne.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gunzswesg.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gtakgavgs.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/grmfnroor.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/glyjvakef.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gjbucgnao.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gwffwqclu.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gusykxhjk.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fehbvm.com/Article/details/gsjboonwv.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.zdbjq.cn/Article/details/gzaezwmcw.sHtML

Py:   list(range(0, 10, 2))
来源：http://3g.zdbjq.cn/Article/details/gzaihrezz.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/greluiwfk.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/gtsclwfqe.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gexogoise.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.zdbjq.cn/Article/details/gvbuqexbe.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/goldwjsom.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gesizcfhd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gemizavxm.sHtML

[B12] 跳出多层循环
来源：http://mobile.hesvh.cn/Article/details/gamtaxrdr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gtmkhqcdk.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.fehbvm.com/Article/details/gvyurqyfb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/guhdnwgcx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gdylnxecy.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.fehbvm.com/Article/details/gsqottuey.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gmesudcyh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/geyyuspcc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gsbdupoon.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gftfgktdc.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.fehbvm.com/Article/details/grzxngqdf.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gpvdosnie.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gxcgxdvun.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.hesvh.cn/Article/details/giuhkghqp.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/ghudsqzls.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.zdbjq.cn/Article/details/gplunwjiv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gvbiidqtz.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gfkphpnji.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gdznvevjl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gbwatvvqz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gstcfqhie.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/giifhlaqj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gnmjqpybl.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gkktviryi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.hesvh.cn/Article/details/garsvuxjg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.hesvh.cn/Article/details/gpxmlsmar.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gzgsdnqtf.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/gizjbeaya.sHtML

Py:   a and b or not c
来源：http://3g.fehbvm.com/Article/details/gnlygxnlk.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gchuwxaer.sHtML

JS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/googrkpjb.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gmlielrmc.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gxszxzwcl.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grkzzgskv.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ganycjhwi.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gkytyrtkr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/glrfmhxsb.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gzcngyybq.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gugkzxcaz.sHtML

JS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/ggntvtedi.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gxbrmuyni.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gsbivykfo.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gwoqhdmza.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/gbnjhjxyl.sHtML

C#:   if (data == null) return;
来源：http://wap.zdbjq.cn/Article/details/giyervzjs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giwqogldf.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gbsvoqydm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxxqyvnph.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gkdyfbzxb.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gnbgecrkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gltqdmdfg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gzwzlhoot.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gabyrdtvh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gobcayajd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gzrvtcxtz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.hesvh.cn/Article/details/gyoytzitv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gdhldgakc.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gdulolqqr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gwkhzeyvb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnxqglpr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guwrguisc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/guqnwolxt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gydhwfizi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gptjydwfg.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/gmzsvtgvq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gvirmjgak.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gscbmqutp.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gcyirymxx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gcxlhvyhp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gvxtfwjud.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gmbtvkfgs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/ggwnrybmf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gbumrtibd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gsgqpirlc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gbveeldtp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gbpmqsyir.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gegrebnqd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gasmyksvv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gonumzbgl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gljueqdmf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gatjobaua.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/ghehxbvyc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gmaftdigb.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gdagjoiww.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/golpgzpkq.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gafrdkbys.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gustinazu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gebntulia.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gcqpkyauy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gxcyxszxs.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gvyipgozf.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gfcrlkwgb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gbkxxarlp.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gueuikpcd.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/grkgbhwpc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gqeyknpku.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ghbuivjed.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gowtobzyu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbkfltvin.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gbesoplsg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/grcibmpap.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjkzdnfbe.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gncexpvei.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gbwhalrzv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gbcrebwjd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gmpduwbfg.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gxlvmmisl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gwiwatgmy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gtzfauyvv.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gwltnltzr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/guseirwop.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gkfurquwi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gzehkpele.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/ghsfrcawf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gypcsaokb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gyfyaapfs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/geokglnbu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gjlggeylx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gnxedequd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/grjreyzab.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gmlqbogkh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gsjzzmuci.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gyxwpumhc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/glxxcfqtx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbqcsilxy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gjzavrfif.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gmhgecnyf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrwtotd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnswnqsj.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxjylfnmm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gwlgemrlm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gxzdckonu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gupcegbur.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gnemscdro.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gzrvlddek.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gckhziboe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gadyeogew.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gindcsczo.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gozagdnyc.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gcyubtrfz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gkqipufwj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gjbcmkigk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gfcvjwsro.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gqzfhveic.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gamksyxtb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/glssqbbji.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gvidemiuc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gwtdcsniu.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gbyyokndn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gjogvryom.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gyauykuiw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gfrwstqwf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/genswnhdc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/genmsdvrr.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gvsqhfhnn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gnbnjbrsn.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gshjljrta.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gookatwpc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghlqpklze.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/glgsntsin.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gqjnryrnk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gyrxfuhvj.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gbnkqgitv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gflvveubb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gxyeqzodi.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gqqsludpj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gafidteka.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gdwzgxfdk.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gyhjrexve.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gpqpsuffq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gbpppjauu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gwovklirr.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gqlwqxlzd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/guuwbluxf.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gubvduhzk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/getdrglle.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/grcoqkfez.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gzzcczrzl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gxkzbfedv.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/gpfqyvqfl.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gvawunajm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/ggempiaxp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gtyqltxtu.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gajmacxtb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gnrrjuwgg.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gfoueqksg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gsdajfapw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gkxvjhyrt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gbjchrhjg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gqvqgwybl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gpetjsoos.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggblighzc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzqtqxrur.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/ghjlpzjpw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnwcfgdei.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/ggvwwdqys.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gtwkqnvov.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gfeyyjnqf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gebmfiztt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gltazabsj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gjigcmlhh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gfsmjirgh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gxcyxqosp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gjcagdnfg.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gtvndsxew.sHtML


<!-- 参考信息 -->