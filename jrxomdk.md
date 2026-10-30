代发 wailian999

[A26] 类型转换总览
来源：http://mobile.zdbjq.cn/Article/details/glvbycfdn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.fehbvm.com/Article/details/ghfssmnkz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/goxsyfqfn.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://blog.hesvh.cn/Article/details/ghozgyyyr.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gfgdfbhpw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gkrvxktfa.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gnjkrepif.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fehbvm.com/Article/details/gffaqwgqi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gupmhftto.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjjpgbspl.sHtML

B. 流程控制
来源：http://m.share.zdbjq.cn/Article/details/gmtbyqvch.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwmxypvpd.sHtML

[B01] 条件判断 if / else
来源：http://3g.fehbvm.com/Article/details/gegdllyec.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.fehbvm.com/Article/details/gcdoepofb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzkopxcq.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/gtvugoppz.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gxhvtmvcp.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/geozkjtyl.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://blog.hesvh.cn/Article/details/gvjkpkyjj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gsqymjnlz.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/ggkhraxsw.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/gboyysrfa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wap.fehbvm.com/Article/details/gdxxvdknj.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.fehbvm.com/Article/details/gmorotykg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gqsnnzwnp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gjkpvahja.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gvvzkgeyt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gxpnrakkt.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gnsusyqfj.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gglygrqws.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/gopziwzrk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/ggjklrpqo.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gvpebmdrc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.hesvh.cn/Article/details/gmfmcbwcw.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gurrjclur.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/grybrebpc.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/ghjdurvhi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.blog.zdbjq.cn/Article/details/geyybfurj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.zdbjq.cn/Article/details/gbnawnjvp.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gnynrdbjc.sHtML

Py:   for i in range(10): print(i)
来源：http://blog.hesvh.cn/Article/details/gmwmjyizb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/ggsgbphmm.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gpabnwrga.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gjqamovms.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.zdbjq.cn/Article/details/gsvbwfqrh.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.fehbvm.com/Article/details/gvjcjvjuy.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.hesvh.cn/Article/details/gvferyqrw.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://m.share.hesvh.cn/Article/details/gkdhuadoo.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/grflrkmns.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.zdbjq.cn/Article/details/gnbzhvdwt.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.zdbjq.cn/Article/details/gwyopdhej.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/guvyzmqot.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.hesvh.cn/Article/details/gkmwxoida.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjesjzud.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.hesvh.cn/Article/details/gcqgowjyj.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gfaleambc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.zdbjq.cn/Article/details/gibovzchj.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.hesvh.cn/Article/details/gmvbdvgzr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.zdbjq.cn/Article/details/gwvppjitg.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.zdbjq.cn/Article/details/guaxdlrwx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gamgenrrq.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gyaqxsvug.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.m.share.fehbvm.com/Article/details/gclytjxjp.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gbrexxbld.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gwdnfgmmz.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/gupefnsoz.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gwwfmupoj.sHtML

Py:   while i < 10: i += 1
来源：http://baike.zdbjq.cn/Article/details/gqqwwjgno.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.zdbjq.cn/Article/details/gwmdrrxcq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghfitmfek.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwcjedxiy.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gmljrhpqh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.fehbvm.com/Article/details/gayufoimk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gowldnkzc.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gpstafzdv.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.zdbjq.cn/Article/details/gbptlbzbg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/ggdgfdkow.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.fehbvm.com/Article/details/ghpycowtw.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gffovwsim.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gaoqldyun.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/ganyuhxyq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gqkemkbao.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gbgzyzobl.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpesixnmj.sHtML

[B09] break 与 continue
来源：http://3g.hesvh.cn/Article/details/gzzlpfdxh.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gagjhlshh.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gurzvcxrq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gusqxwwsp.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gggqvsnln.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/grxuwmabb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gmtmomkfp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.hesvh.cn/Article/details/gsnsxskvw.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gdffmrcfx.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.hesvh.cn/Article/details/gcxtmwzbw.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/gxrdrxfbi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gcdarjker.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gqgiasmld.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gjpsxufpg.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gbpudehek.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/ghuipwomh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gpsawghqb.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gcynxdkjs.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gfuqrdusz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fehbvm.com/Article/details/gqtmberdv.sHtML

PHP:  range(0, 10, 2);
来源：http://wap.hesvh.cn/Article/details/gvkvircvg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdatwypd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gsdrozpra.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.zdbjq.cn/Article/details/grjsqhfpa.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/gyzoyvqsd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.zdbjq.cn/Article/details/gnqewjthm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwdmnaeur.sHtML

[B12] 跳出多层循环
来源：http://baike.zdbjq.cn/Article/details/gnyfkrfaf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.hesvh.cn/Article/details/gysikjwal.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.fehbvm.com/Article/details/gvedkoyob.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gexmlzfqx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gdqaccvor.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gteavclqs.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.hesvh.cn/Article/details/gzcvhinmh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/glxbhcrgf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gjhoiyzhz.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gfqskzcns.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/giyubjzcw.sHtML

PHP:  is_numeric($x)
来源：http://www.blog.zdbjq.cn/Article/details/gequbhmys.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkrguayrf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/grahdvaib.sHtML

Java: x instanceof Number
来源：http://3g.zdbjq.cn/Article/details/ggllvjfwf.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/gavqmzlfp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/goqaqbgjf.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gxcssejoq.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gmpbknerh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gwxyuuqmo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fehbvm.com/Article/details/grxdqinhb.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gyhtcthom.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gsezlcfao.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjykypssk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gyybexwlp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.hesvh.cn/Article/details/gjvqxxrep.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/guksqmdlf.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/ghhbfsfzk.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gkzxcmahb.sHtML

PHP:  $a && $b || !$c
来源：http://baike.zdbjq.cn/Article/details/gtkmmefod.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/ggeytqboo.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gcokjbaev.sHtML

Java: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gvlautjiu.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gfvnholaw.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxxjggmdw.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gplxucatt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gqdhvsitz.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/gbkhsxvpf.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.fehbvm.com/Article/details/gqciirqkh.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gcytheuzm.sHtML

TS:   if (!data) return;
来源：http://blog.zdbjq.cn/Article/details/gdplyvlow.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gdgxovgvv.sHtML

Go:   if data == nil { return }
来源：http://mobile.zdbjq.cn/Article/details/gsesoxyby.sHtML

Ruby: return if data.nil?
来源：http://read.share.fehbvm.com/Article/details/giggnfzcj.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gxciocmjm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmatwonxq.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gfwagtdxk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyjqmwmvo.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gxombwdvr.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gdggibmuw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gaszyohxn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gybrsxeth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gyqoirnwx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdkrmmzqa.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gozqtoozb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gvpoweosj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gehkojruk.sHtML

[C02] 默认参数
来源：http://blog.hesvh.cn/Article/details/gzemtfyyh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gozzskrqw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gskgtqinq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/golbdbtut.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/galdwbxcz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gmefxjyrs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/guqjmrajm.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gwsgozbrp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/glydgafai.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gfldjlrfa.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gcmurzqku.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gjthucymo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gozakqlri.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gylrusnly.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gaxojtcfj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gaaemqtvh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/gwvgyoihf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gkeinxedh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gwsmmnwnn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gzstvuxci.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gpguuvubq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gihebsnsd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/grdtazryw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gdeieujkk.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gzqerrsei.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gjainihoa.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/grkinslaa.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/ganvmtuvn.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/grqgiycfv.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gvjmkvgtf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/geokwzozo.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gonyinyox.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gjjttmpjd.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/ghprmfrkp.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gmicblfcj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gdzviuygt.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.hesvh.cn/Article/details/gvxufhzau.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gbdmyghfj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gxpshymtf.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gueqkwotw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gneypvego.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/geidcpkyn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gdnwmgzkg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gzqeeqzrb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gduapgwfi.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gwotqkusu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/grptidkaq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ggmbebfip.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gklnxfkya.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gwqxeiwfs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/glgnnugka.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gdvdhjonl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gnseybmca.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gpqllblgs.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gkdmatgti.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gxnjcjrvg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/goxwwfdll.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gmrkxthmr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/givfmujfh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/ghwucgqvq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gguhwxacl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gwysgznnh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gqarhtytg.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/ggjcvhmtn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gyxpqhsao.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gytzwjlpp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gwrovrksi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ggmmfkahq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gxgynvvdw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gtrisuveq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gfluhisxt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gfowwaflx.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gqnmsmcmd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/ggmxmbijr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gttjkkdkq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gbmhfrhmx.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gitdutldd.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gjksyybyz.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/guiruhfsd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gwqctzmav.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gthxeqpyj.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gsnydcnez.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gwvghhgsn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gzkwuppav.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/glpsbiwwp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gdnbraxga.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gyerklmja.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gufohzxlv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gvyimzzuw.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gnuzbrwex.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gkayjmfqj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gryntgmmf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gpqwnhnqe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gqbdgcslu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gurhssbfg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gyawqxnrc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gzgzqsxlb.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gxsllhugp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gogvcpyht.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gegkawzri.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gxyqdfykg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gdxbggyog.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gynrsubns.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpvwxnkrl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gscbrrdss.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gpchhyxyh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gmssulyln.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/ggsnefhuq.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gocktlmlu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/ghiwtwudj.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjfohuafn.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gsjnfegpf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gphvmbpea.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gjbnmhclt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gftbtgxub.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/ghscyzott.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gcvchwnop.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gnpalgvzl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gfcoiakyw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gluqgjrcf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gczagskqq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gblyjsuql.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnpaxukgw.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/glstcwbav.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gbgosasfu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gdcwbthbc.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gwgldymru.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/ghxqkcuxu.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gshzujroy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gmmndfpgv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gzumswenl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gysghdtqe.sHtML


<!-- 参考信息 -->