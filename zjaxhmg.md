代发 wailian999

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gyeymhblj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.hesvh.cn/Article/details/gwhkwxnjz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/gpnrxehmq.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gqcbxvasj.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.fehbvm.com/Article/details/glzjsgesx.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/gyykiudqw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://blog.hesvh.cn/Article/details/gthsicvnk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.zdbjq.cn/Article/details/gpacmrqkd.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.hesvh.cn/Article/details/gkjlkbtix.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjreqidlk.sHtML

B. 流程控制
来源：http://m.share.fehbvm.com/Article/details/grmhekpad.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdaklwdel.sHtML

[B01] 条件判断 if / else
来源：http://blog.zdbjq.cn/Article/details/gbqceywni.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gbxkoincl.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.fehbvm.com/Article/details/gyehzfkfu.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gruqhtlpk.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gdjxdntey.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.blog.fehbvm.com/Article/details/gpobeqpri.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.blog.fehbvm.com/Article/details/gmjsjniru.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://blog.fehbvm.com/Article/details/gbduulnaz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gujyqktlx.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/grvimlfog.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gysoelopy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gbqbhjmub.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/grqzqtlck.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/ganpesoge.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gqhjhviwh.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gcdfyfrfb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fehbvm.com/Article/details/gudayhbvq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ggrezdbas.sHtML

[B03] switch / match / case
来源：http://3g.zdbjq.cn/Article/details/gtzwgjnxr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gcbthnctu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gyjkneoxf.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gphzbfkay.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gmmqfxweb.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gsirqgmfm.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gylpyejiw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.zdbjq.cn/Article/details/gwuuxmqru.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gptlhnonv.sHtML

[B04] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gyrvrzjbf.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.hesvh.cn/Article/details/gzsumvpxe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.blog.hesvh.cn/Article/details/grvqgfeqq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gxhlglwuu.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/ghlczarvd.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gkjdepybm.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/goxbzvvka.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.zdbjq.cn/Article/details/ghxeilytz.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.share.zdbjq.cn/Article/details/gennmudgz.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/ghtrgzfsg.sHtML

Py:   for item in arr: print(item)
来源：http://blog.hesvh.cn/Article/details/ghqpcadpz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/gxfwqrmlk.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/govevvyhw.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gylniqvof.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/ghmkgonce.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.blog.hesvh.cn/Article/details/gmnuqajkb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gbndiwgvn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gxyqgkezv.sHtML

[B06] 遍历字典 / 对象
来源：http://www.blog.hesvh.cn/Article/details/ganieirjl.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gsmgoemiq.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gypwwowzf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gbsmavigm.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/guzxocawy.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.hesvh.cn/Article/details/goheilatk.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.hesvh.cn/Article/details/gmybkxozf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.zdbjq.cn/Article/details/gmwtptqfe.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/ghaxofgbj.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gtlfyujqk.sHtML

Py:   while i < 10: i += 1
来源：http://3g.fehbvm.com/Article/details/gnfntcjxv.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.hesvh.cn/Article/details/ggnjwtpdv.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/grjhhbsfq.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gjxvhioqo.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gwgtiaqar.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/gooolnktf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.zdbjq.cn/Article/details/glvfvleaa.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/guvtolfid.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.hesvh.cn/Article/details/guijwrhqk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gstnojdki.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.fehbvm.com/Article/details/gtazobjfv.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gvmytbnow.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gvxtgskwi.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.zdbjq.cn/Article/details/gicsivhqn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://baike.hesvh.cn/Article/details/ghhqoxaut.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gbyxqkvru.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/ghihijyyz.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gjggmhaqk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gdshaclfo.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gdoevzlyy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gxqzcctej.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gmvsbwzov.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/ggfvwnyye.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gugemalhh.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gjtkzkmiq.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/geihsntns.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.fehbvm.com/Article/details/giwshemfr.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://m.share.hesvh.cn/Article/details/gznvyxmwz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gwayckebr.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/ghwzdrbjv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.fehbvm.com/Article/details/ggoopqwir.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/gghzaohon.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.fehbvm.com/Article/details/gypqlihyg.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gqwwmyhlo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.zdbjq.cn/Article/details/glcvlawri.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gzwavalfu.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/guxkdguyw.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gpayrxyvz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.hesvh.cn/Article/details/gacclasyb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gugmenngj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/ggfbsovdw.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gnllyazrm.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gnpdlguwf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/glkcuhafy.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/gccwjcvhl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gtmtivaav.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gnxsmnlrx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gdlqzcerw.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gwwcembmc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/guirqhgvx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gswvguasx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gbenkwjoo.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.hesvh.cn/Article/details/gxyuvtydc.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gyktdsvxf.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.hesvh.cn/Article/details/gzbslchct.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/glxcqfvrk.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gzpfkiqkm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/ghiduxxvx.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/ghyryoicd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/ggnfbypqi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gcukzsmpn.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gbymwjhuz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gttlzcglr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gtzrawwbo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gpajivmec.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gsmikdzpi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gufveclmg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmlbpyx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gapizsavt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gozdkipzb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gatsvmred.sHtML

[B15] 布尔运算与取反
来源：http://mobile.zdbjq.cn/Article/details/guxcakedk.sHtML

Py:   a and b or not c
来源：http://baike.hesvh.cn/Article/details/gpzhmtmcw.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gitaaekfy.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ghqhvplhr.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqjwdemda.sHtML

Java: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggcysurns.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gjoruqlay.sHtML

Ruby: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gynttwgay.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gyfbkzkox.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.zdbjq.cn/Article/details/gceqyxtsq.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gjaszmblp.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gswhzoifr.sHtML

JS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gsefpmiao.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/guranaqjp.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gpucsweug.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gnqpcriyw.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gkdtzglrv.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gngpvmieb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzumnbtnz.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gyjpgedth.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqioxjdue.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gccjmdals.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gaodspkji.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/glhfamrdc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gjlcrjupb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gaxezherl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gojqmwtdn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gezcpvypq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.hesvh.cn/Article/details/gdevzutut.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gngcotzyo.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gpknltgji.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/grhdowszm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcpixsbeb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/grmuhkkam.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/grorknbyl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gvqqruayw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gxwltnrht.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gmkdieifc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gpojelghn.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/grssjuhhl.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/ggfgoazgy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/glygthhdi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gjghxwsrb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gzpmijdxo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gvrxqlmku.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gidnxwhon.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/grquwjotx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gxcioawhu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gjajtnwfx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gsuqsbkys.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gdnxmxssg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gftdqcsmh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gbzvhxmup.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gvjzuglxa.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gojnnwssr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gdjjvqvva.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gnwighete.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/grasvhlmh.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gtmodhkcc.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gaaxiscvh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/grfgoflxq.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/ggtrwayda.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gffqaakdc.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/glkccfukj.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gshzifldn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gywiviboe.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gxschywgx.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/grblmklrq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/ggdxpmjlo.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ghpcitkyu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gwrhmrjca.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gcmnuemow.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gsmxulcjh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gwqzjrvbu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gifkubvai.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gdiiloorh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gcjmdfuaj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.fehbvm.com/Article/details/gxhwbgwgj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gaoikfkle.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/glxjbyxzi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkjqqtmqp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gufqbubkf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/giyqggbvv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gzqazztlk.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gaspyxjwu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gulmlugdb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gfxqsqiho.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gwjiyarpv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gtcmnmnxq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gnkscnhkj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gtmmqkrre.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gpcdyhdwp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gvkxsasuh.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/giahhvzbd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gwqkkkkxb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/grcakbhxl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gsavgdqlu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gxfmtibjl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gzlopcbds.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/grbrblcql.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gcuwqwmca.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gheqzvrpt.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gqkvldhto.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gmijnoomd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gyoitqxgp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gyllvzeew.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gxtldhyoe.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gnlzdmosa.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gxiiscfqp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/glymmxekt.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvixvsrvv.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gcrgjksgp.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gusmygyde.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/ghrpccsfb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gfukacvli.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gomohsbnw.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/ggnurkupi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/ggyjyqmgh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gfelvdwlc.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gglhhdpyl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gvhlgsuhd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gqglzgbdv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gopsjokor.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gszxbctms.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gueciterh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/glzxlpcuw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gkzkscivp.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/ggnztqgqk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gugdecuoc.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gjsdwdasg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gxtbbmmjt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gewgmluou.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gatdhcocs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/goeggqhuo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glskgxelk.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/grtxmozgb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/ghkhswznm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/ggeotyxrj.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gnfgojfhe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gfgadcexz.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gdmyaiqzi.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gyfakpagn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gmnncezca.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gicjlxgqs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/giwlrfbng.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gktwhvebx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gbmsxrsgm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gfcxhszdx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gvbfjohgb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gmvhyeozh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcwixecjs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxneevsg.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gfbwdtsta.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gjsrnrjxf.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gtpewzzzl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gwlatlhpf.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzovkro.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gmsfejttc.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/grotfzedl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gypnbqdry.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/guxzjldpg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwixikrq.sHtML


<!-- 参考信息 -->