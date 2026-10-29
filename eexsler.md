代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.zdbjq.cn/Article/details/gnbwyhdxz.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gtihcutcd.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.fehbvm.com/Article/details/ghpadtroy.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/grllflrcy.sHtML

[A26] 类型转换总览
来源：http://www.share.fehbvm.com/Article/details/gehyrjghj.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://m.share.fehbvm.com/Article/details/giousnubo.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gfsypjbat.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.hesvh.cn/Article/details/gbnknghuc.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.hesvh.cn/Article/details/gsnwjwtgv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gvcfffzxu.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.m.share.fehbvm.com/Article/details/gicqmxabt.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/ggjmrszxo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://blog.hesvh.cn/Article/details/gktbbndkb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpiqbxqft.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gashbtjnf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbttkycll.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gkoqgzuzl.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gpnaxkmyd.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzidfwtfz.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/grozowssr.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gvghyfjzs.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gymkizeri.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gvxebahcr.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.fehbvm.com/Article/details/gzjuqvtqz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/grgynrovh.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/guvnafqnb.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.hesvh.cn/Article/details/gcehitvcj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.hesvh.cn/Article/details/gabgnuzpn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gkbcjxnkk.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/glanfissa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.hesvh.cn/Article/details/gzjmgkawr.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gffacsgww.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gxkgbuhpp.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gbfczotee.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gzwiuuszb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.hesvh.cn/Article/details/gqjayzocm.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://read.share.hesvh.cn/Article/details/gxdxtxsjp.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gnqvktuyv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/ghnxgoujz.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/glnopizdx.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.zdbjq.cn/Article/details/gvfjmuqvu.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.fehbvm.com/Article/details/gvsxrpkfm.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gcnvscuol.sHtML

[B04] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gwkkownrl.sHtML

Py:   for i in range(10): print(i)
来源：http://www.share.hesvh.cn/Article/details/gkhgbwpvx.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/giwfscawj.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/gntavluuc.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.fehbvm.com/Article/details/grhjuouyc.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.hesvh.cn/Article/details/gixlyenwa.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.fehbvm.com/Article/details/gdjnuehlq.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gqzvogiju.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gsfurvygc.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gfgvtzsoy.sHtML

Py:   for item in arr: print(item)
来源：http://read.share.fehbvm.com/Article/details/gszjznodn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.blog.hesvh.cn/Article/details/grfdjlyga.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gypdkcfab.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.share.hesvh.cn/Article/details/gpwxyumsw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.hesvh.cn/Article/details/gcebchdcg.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://read.share.fehbvm.com/Article/details/gsnqtlgtf.sHtML

Ruby: arr.each { |item| puts item }
来源：http://wap.hesvh.cn/Article/details/gxsivklsu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gofdofcai.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.zdbjq.cn/Article/details/goaqsqejt.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.blog.hesvh.cn/Article/details/gusmhtgef.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/ghcluxeme.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/gkipekwwx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/ggmdhzwnz.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gppwwckpi.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.hesvh.cn/Article/details/gurljtjvp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.fehbvm.com/Article/details/gqzvlzxjk.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.share.fehbvm.com/Article/details/guojrhqet.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gatmqlsiu.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gzcmjqnpp.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.hesvh.cn/Article/details/giaxjuwft.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.fehbvm.com/Article/details/giwjdgloj.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gwlvbrlyi.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gyqwuftio.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gtiysdnux.sHtML

Ruby: while i < 10; i += 1; end
来源：http://read.share.hesvh.cn/Article/details/gndtsdogl.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gycmuxear.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gtdkpznwf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.fehbvm.com/Article/details/gqlfmvdyv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gakllpdvi.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gheblluwn.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gbgcvogxv.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gegsawlje.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/ggtmzimzi.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/geyyzmrce.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gmjqybcdo.sHtML

[B09] break 与 continue
来源：http://read.share.fehbvm.com/Article/details/gdxspahfj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.zdbjq.cn/Article/details/gsaqaeraz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gtwngzzdr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gfnlddglk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcajiysln.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/gurqipynq.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.fehbvm.com/Article/details/gsnkeyxam.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gmiqhzrbg.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/guxpttsqn.sHtML

[B10] 遍历同时拿索引
来源：http://mobile.zdbjq.cn/Article/details/gznpcwnmt.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gugxxayru.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gcacvwies.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/guskcginb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gikbegpgs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/giuxviasw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gpjporqrk.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.hesvh.cn/Article/details/gvyjdhzyb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gzrixlilq.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gkxjdscht.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.hesvh.cn/Article/details/gdjvyhhlm.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.zdbjq.cn/Article/details/gmxhzomsw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/gjljgkqgl.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gzauuamvh.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/garrxpgeh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.m.share.hesvh.cn/Article/details/gmnikkgdl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gofzbfioy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/gbakaydld.sHtML

[B12] 跳出多层循环
来源：http://wap.zdbjq.cn/Article/details/grqynltjm.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gvshbduke.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gxhypkxlo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gnwvnzrhp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gbytsfikj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gxjlckdoq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/guzgwiwil.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gppskhbkm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gckysgelm.sHtML

[B13] 判断是否为数字
来源：http://read.share.zdbjq.cn/Article/details/gwbweynra.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gdxjpwfay.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gtjcaskfr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gnjvhgbtf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gfrdoryrx.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gnedktmov.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.zdbjq.cn/Article/details/gtktzpzpo.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gmfdmdjyk.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gzhnyfvoy.sHtML

[B14] 判断值是否在集合内
来源：http://wap.zdbjq.cn/Article/details/ggtggsqkq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gpkrdnwoe.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/gxrfucttm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gsalhniyf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gtyhceocv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggomdqyel.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/gwjidwcdq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gjuurxebf.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gyykdhpju.sHtML

[B15] 布尔运算与取反
来源：http://read.share.zdbjq.cn/Article/details/gpffbgtmk.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gkoogybuo.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gebozbuej.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/getqtamtr.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gribnvanf.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gplyzfsqe.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gauxhiwik.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gmacgrapr.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gurivrdtn.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gsgcbtpkg.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/gollmnvav.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gfqxjpyeu.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gzzwckfeh.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/glsydbqwg.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/ggqtazngx.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/gvteypgdi.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/ggyhlarpu.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gqbhkmnoy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gejuvsfez.sHtML

C. 函数与作用域
来源：http://www.share.fehbvm.com/Article/details/gqodqxxxl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghtigikpv.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gfwhdywcf.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gqygbhzto.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gsbjedtgz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcedacclj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtcylodxr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gxxixbvpe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gesghcfvu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gjqqcvlys.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gevwhuacv.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gedhuzlkb.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/grhvkpxiy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/glexbxnjh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmpqankff.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gazvhfnfe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gmvynyhks.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gfqatdicb.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gdxzzqzvl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gsvttdqsk.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gkairigiz.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/ghldogkor.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gslxxecwd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gxpaxqlcp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gnzyygpjb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gdkcxmeii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/glgwxjkqs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gcueqzxtz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/goepnvqts.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gfzlekqvs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gkiarppcd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.zdbjq.cn/Article/details/gvaglnlqf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvhmrfbum.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gppucfete.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gijiycyax.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fehbvm.com/Article/details/gzuqtufao.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gulyukism.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gkwxfmnfp.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gaarqjzxh.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gblfqltki.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gxrfkomjv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gwphnkarg.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/geylxxfph.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gbagjwvin.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/grifbopjv.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gikfcpcjs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gincrsjnj.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gtpmdvqnn.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gofgmulrh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gsxcxuxve.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/ghdpbqqxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gitxfpynd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggyfliqdr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gaahentcb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gdpeexipc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gbuyougmr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gwllbklih.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/glvipwnoj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gnyebstyt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/ghqudtzjc.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gzauivgdk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gduyyajab.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/ggaltevwh.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gtayzbbeo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/ghemmquwa.sHtML

[C08] 闭包
来源：http://wap.hesvh.cn/Article/details/glgkqaaba.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gropvkcvs.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gqmafdwvf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gepnbuowu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gmxnznnmc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gcrguklap.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gzgylbxid.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gbfwqlxpw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gprmnnoun.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gwjjlafrz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/glckzheuy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gogypegpv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gysefbasu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gygyodxnq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gkmlkrqdo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gagfysncl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/glhsepjcs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gvqzafqos.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gufzylsyb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gqbavyjcc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gofejwrqo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/glbjdolhl.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gzmomszzt.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gysnopjah.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvdwcljgb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gkyrzkyjd.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gfxtgpnhe.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/glgmcejbs.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gyddrfoom.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gjxuyaaoi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gybfuvwyt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gagnrnapi.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gdaurzkff.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gljlywemh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/grkpoxczz.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ggbzjinkk.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gqltcrwgc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gbkhkymys.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gnlfrmtsu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/grekkaksr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gzbuvtcjz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gmcodzzgm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gjbjdfcbn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gkhtyyypr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/ghpmgendf.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gpmhukjjh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/godgixfeo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsykhwfzc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/ghgqpsmoe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkaxqizmh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gjaagnzqm.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/glivlnkxh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gczdnkptj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gsgyqigcp.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gauexhngk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gfttzodou.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gtpzjkhxb.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gvabfddtq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gjfgyawbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/glulhiiev.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gdyhuuoep.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gypppulgk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/ghrthdwjy.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/ggojsiryy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gzwjufavs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gkgukptjx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gmutfxvij.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gnpmqhdyh.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gajxzplmj.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gdrdhrxqi.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gkqaneptm.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/ggxtabuif.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gwysbelbh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/ghsmnrdch.sHtML


<!-- 参考信息 -->