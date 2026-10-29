代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/ghvmjkkqv.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gtcfksuwt.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnqfvgi.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.hesvh.cn/Article/details/gsevefwqh.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gufgadsyl.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gzxqaicqj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.hesvh.cn/Article/details/gfszyeydc.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://3g.fehbvm.com/Article/details/ghirzubrg.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gbwaaykkb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/glclyfmem.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gnkvyetrt.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.fehbvm.com/Article/details/gaarvqpyx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gvhdzbsky.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fehbvm.com/Article/details/ghgxqaskv.sHtML

[B03] switch / match / case
来源：http://blog.fehbvm.com/Article/details/geqefbzwq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fehbvm.com/Article/details/gcheadwsz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gfqrsxzql.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/guxbdfirj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gypgsikhg.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/gwhyyejso.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.fehbvm.com/Article/details/gksdlfopi.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.hesvh.cn/Article/details/gmjakdqoo.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://m.share.hesvh.cn/Article/details/guzubrffd.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gjuomglye.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.fehbvm.com/Article/details/galhbnava.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.zdbjq.cn/Article/details/gfrlsdezh.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gyfpjosvy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gcnrxvegk.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gkiufbxju.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gwdtzjmff.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gmclsdaql.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.hesvh.cn/Article/details/gsxzjphxz.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gjlunhisj.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.fehbvm.com/Article/details/gkpktfuhn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gmtumpfuv.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gtbrnunry.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/guhfugbbr.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.hesvh.cn/Article/details/gxzptzmyo.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://m.share.zdbjq.cn/Article/details/gvsagskew.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gbbdayljo.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fehbvm.com/Article/details/gfucxcioz.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gfjpxoxdy.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://mobile.zdbjq.cn/Article/details/gboxkndtn.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.hesvh.cn/Article/details/ghzsauoyu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gatrqhtyn.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/gzfyexxnm.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/gwndjquqn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gbrhcsawo.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://baike.hesvh.cn/Article/details/gphzysuzt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gwiyarhsf.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gtqnzbspg.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gfurdlhzu.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gpkczzwvc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/ghugsmiso.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gnramnwzj.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gcljrhhhl.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.hesvh.cn/Article/details/gyrbihwen.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gwtbwppuy.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gxfluxxje.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gtyokrflt.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gpyzvwhgv.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gmlodcbgl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gqvtilftr.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gipsmmbzs.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gmjvjvzie.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gcighpjnc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.hesvh.cn/Article/details/gjnxrfnly.sHtML

C#:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gdlsjtvhf.sHtML

[B09] break 与 continue
来源：http://www.m.share.zdbjq.cn/Article/details/gmbhkikar.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gkrhrwiwi.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/gzigpysek.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gzmxexald.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gpbfjrgok.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gskmgfzjv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/giospzred.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://m.share.zdbjq.cn/Article/details/gfalqzvzk.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gclohwwih.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gcukzgcfg.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.blog.zdbjq.cn/Article/details/ghoxnpzbv.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gomgefavp.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gzwdabtlw.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gocexzwts.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gkynggxtn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gftrqrcsf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gkvpkpmzs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gholsunku.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gvwgulbuy.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.fehbvm.com/Article/details/gjymxnxiv.sHtML

PHP:  range(0, 10, 2);
来源：http://baike.fehbvm.com/Article/details/gfwhyfelg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gapxgikcp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.fehbvm.com/Article/details/gznjykjdk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.zdbjq.cn/Article/details/gorvcmtxg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.zdbjq.cn/Article/details/gyifytjnh.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.fehbvm.com/Article/details/gsatrqrzc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.zdbjq.cn/Article/details/gtdfadmbq.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/guhxhbmlk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.hesvh.cn/Article/details/grbxzjgqr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.hesvh.cn/Article/details/gvtqkaodx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/grxdvdysf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gfqhjtuph.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ggwozblsk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/ggrgzcuif.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.hesvh.cn/Article/details/gwplhplnq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/garjxqjsu.sHtML

[B13] 判断是否为数字
来源：http://baike.hesvh.cn/Article/details/gizauulva.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.share.fehbvm.com/Article/details/gcwcprwyo.sHtML

PHP:  is_numeric($x)
来源：http://3g.hesvh.cn/Article/details/gdkpvvect.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gwkvgqrlt.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/giqbaubup.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gevsuglru.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gulpcswaj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/ggdkbbkol.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gdcyftioq.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gogtxamea.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gciidgaxh.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.hesvh.cn/Article/details/gwcrfffne.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gojpcgedu.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/ghcqospwe.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gspjvgsrf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gctaiktal.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gumpliyds.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gabaiiwcl.sHtML

[B15] 布尔运算与取反
来源：http://3g.hesvh.cn/Article/details/grhttrnaf.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/gdhafifqd.sHtML

PHP:  $a && $b || !$c
来源：http://3g.zdbjq.cn/Article/details/gmnptbyiv.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/ggrrwibbl.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtuewaunr.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gxruykulw.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gymaclagj.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gzmjlhsax.sHtML

C#:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gueyowqft.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/ggzqtmjts.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/goxkwomph.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.zdbjq.cn/Article/details/gocbwdlsi.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/glfdxafvs.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/guyttijsz.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gijbvehwm.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gurorqomu.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/gdnasdgsn.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/grunrjmij.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guhorbnlk.sHtML

C. 函数与作用域
来源：http://mobile.fehbvm.com/Article/details/gtxgesxtv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvfzlfahp.sHtML

[C01] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gxijkfvkq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gydxhcuck.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghplwamki.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrtfbdac.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghxysftks.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gfurezput.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gonvqefwc.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/giawvghze.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grznzhrsl.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gnbvhehjs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/ghsneeull.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/grabzgqhu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpkxisgip.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/govljlfky.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gkgtgazda.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/ggxghushu.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gpwfvoofd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gyfhkreyt.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gxohxnbyi.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/giubjzhbx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gicvvjpiy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gptbcknyi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/geeyhnxyt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gtkaptqul.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gmrvjvrho.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gfinpiysu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gkooitqdi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gftojtxdl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gcbrtjbhe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/gporkbhep.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gvdqrgkrh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/gccnrcdce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gscwjjxbu.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/goikwlclo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gziwzvyky.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gqexetyzr.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gpkzihbbj.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gmbmzixnp.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gfwoeubdy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/glcqkvnhq.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gfvvfdlcs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gbmzttwky.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gwqorharc.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gktwckqzr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gevzkevjr.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gjmgbmldd.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gogecctar.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/goyprfdlu.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gvgbdwhqy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gzwsahusl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gkfqxeqzk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gbxzvfazt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gtpqxvsfy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gigvtlnox.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gzncvhtkq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gitjyedfk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gtybdbuha.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gbdnvmaxv.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gaocyjjpk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gklvmnxda.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gzjtbmoco.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gudbcmggo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gzdcpsiao.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/ghcacicdm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gootkqkbp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gtkadazsf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gxscfyehs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gsjaqkxbg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gqgjqlszj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gqlgtqfxw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gblhqtylf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gbmenipjx.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/glvkyvrtn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpwinlmvo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gqhqxthbn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gckpxaeup.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gclzyhjyu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gskirncva.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/ganmmkkwn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gvsmagcuo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gwgbszbhl.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gtlshnaif.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gzttkeych.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gdtwkirlz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gttaduwak.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gxfgojhwo.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ghdnofnyb.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/glvyphkzy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gjvpdudfy.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gttprtqno.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gpozzhttp.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gzmqdqerb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gxzxemuuf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gfztsvwnj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/glbnvrzlu.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gejhlfjjo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gubsxraao.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gqnbjajmk.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gbixedycx.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/grhxxqznx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gwfnkqynn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gsztgirzj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gyjtgwqli.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gaizbvprq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gynurcqbt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gloxhdtav.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gmkzfzisd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gzogrzrnh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gupkwqnjx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gdovmvfqm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gvcpnkdvz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gnehgmbio.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/glvwxdvyb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gzjmyioen.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gbcmlqipb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gbehciftq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/greafodyn.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/galyfqpgt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gumgfweuy.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gxzdwaprx.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/giglyroot.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gzvlzxdly.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gwfffzenl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqguccyc.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gnmvdhtow.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gtqduyuyx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gyvpewtmo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/goxrqjhav.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gkwihvytw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gyoiickqw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwintuq.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/giffmpcmz.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gkyjphgrb.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gdpwioimv.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gxqjlaubi.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gikkbdref.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gcmgsdufa.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gagkgkcez.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gopppgwlu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/giukdtjdv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjuixrxva.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/glokkipda.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gngcuhgsj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gcqqarzfz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geokoxjao.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gpavunrei.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gunbmokkg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gehissenl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gmauplgsf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gdbtqeuny.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gbtdhdxpi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/giapdpkmy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gdnphmjrm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gqyjengey.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/glgbohgbb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/goceqvdxf.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gtzywoifu.sHtML


<!-- 参考信息 -->