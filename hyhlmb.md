代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wyzdyaxn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kqduoyrb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2oyombcik.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2szmxsvbv.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2grrsldye.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ruhyaupu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2xuyeuwix.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxtsxrz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zjcxgfzq.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kqnvuvil.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nxcsnycw.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2cbrtxtrj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dglddxen.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hiqxwbeg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ofkfkfpi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2bwqqtgvz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2msetpver.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxttdqjv.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvsxdxs.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gianygoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mpxbcmwl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bafxdeos.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2sbrhamay.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dobduidm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qvbzcdsk.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rxystsde.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjxtdsnz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2onrspqpt.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2qkihjekm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2izmmvesh.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wyowbycu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyzeniln.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pcnynuxc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bauohohj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2kysghrew.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2scdiojvf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jpvlghsv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrdcztry.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2surnhbwy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kaampqfq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufbqddkt.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bzhgrfip.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ofgombwr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rxjloqis.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2oomnbqtn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2mzriuuvg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gmsdcaod.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2bdpuwnas.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bufwgynw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyljcxmb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2intqitxk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sriyamps.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiztcnmv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fngzcabq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kwlbqkeu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2heevovty.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2ysxkoggw.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2mwiymixf.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2uwdtwltf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2viydpiug.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2pbglvlhf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wuvexvkq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hxylgbju.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wfaxgiit.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2izdhnemv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2sqdirpod.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gnzmdhmo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bdowdxne.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2axxhuzgv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lxtivkbn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pprtvrjy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vstujiwx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2usevuyig.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrunieyy.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jareypce.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yxyrxexl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ogdtgcwp.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2xbapnyum.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuebnqd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fkgteuip.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mltuyqtf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ydxjlefw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2grtsiarg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2kwdavxri.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2iqrcmqgl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmbbrxsb.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2wemheevs.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2anlzjwvb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sahreahq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2zbjgsxoa.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qljtnmdr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2txckqjpo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2knvnpzjz.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2nypfacdp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2mblcpmws.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2twybfjbb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ajnybnke.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ljuxrxcp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2htqysflv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mapakfix.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqoepix.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fahssbag.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2gbklscmw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2sldfnncg.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aqwlpbof.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2akoeskrs.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2jqncrskn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsnpvhjd.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2orsolpbn.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2bpagotsr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2igeilgvs.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tnytbdxt.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2uvwhdfsr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ozpymzqk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rbtrfccu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqulhoz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogumfxda.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqcfpyj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hljuyufc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2mkngacfq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qgzoavze.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2anbbicsf.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gkxjyjjb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xvzluiwj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2keqptazq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2muhcezbl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wnnruydh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ckmzwvna.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kyxksqfx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fqddngfg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ndarxlkb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mhtquxxj.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tatmmwhw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpsrsjwv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lcobxvwr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ufmtapgu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2woobsbxf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hgxsygal.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rmhdieup.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2msjicmoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gibgciel.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2plulznif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbdlowmp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2eghbchzl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kswzgqrl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oohrldvp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovtjahax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ehthtjnu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncqplysg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lzcsystx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykiknioa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swzqwolr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ogoreehf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ykkusufo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmfhgdrt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nhatsiuv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ifunocbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2swbvnxvr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nnuitsnk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nuphamea.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2uegpbina.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2xyoojkoc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vfkoapzt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ohgokqfk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnywka.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2msgfncqx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwcsxxsw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2johzfzkg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tblopuvn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ovhfttnf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cihckvzj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2pimdkenj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2onuxrzhf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2insnbwid.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fpbrnmmb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2fjgxshef.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2frzxkowi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jttchrlu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjokzkjh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2wokgaxel.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tgotxsot.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oxngrlcc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2eaypqgfs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dujfhtzz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2heewubfb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2baevdgxs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nvkgjhhk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kqjazvmp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lukygyws.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2lrgtsrvn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gfwbplnp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sbhwkudk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2izrdqrtu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wvvbjomy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nstoqixn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bvnawpcp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mmlfvvgu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2clbijozy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wivnhbzq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2svjfhlle.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2izdmrqkt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jroqulds.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ziyqahlp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wrmcrndk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ccqxneaw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2uxfkniwj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qvcnbera.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2emtobbdp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2omgycmiv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tlrymuxu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwmitjmt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cgqezcqa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2iwvmverz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tntvnfsc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2plvfzaxv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2tucxtlck.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fezczhjq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ctcyewyh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qpuiruyl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aoczixhe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkytmvjz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2nyxucybl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fidiptcd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zibtvble.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vawdtrtf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hwsvergm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kcoomhgx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fdjuezrp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bpzlcyim.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cumxzphd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pkplxucj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tlyttpii.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sclpukcu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ppxhwmqs.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jarvqnkn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwgyxze.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2milewrdy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nagcgigi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pzquyhwr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2exjvfhns.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2acevmzsf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lxhgjjda.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ankjvifu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2uglakznl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fvxlsidp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ekbhjocz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ldenpsqb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mlzquxgu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2yytqulyv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2sxdsomxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2suxilbrl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cfsmlaow.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2myesprvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qapruvvb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ztssxfkl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jukununw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpfsnkai.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wowlmxkz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bkpmoash.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2tgbpqiwr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2oeqeowup.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2gfftpxgz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2idjgjoqr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mkauawjk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zicvejqk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2szpkscwt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2muxcptde.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2frwfvgkk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hegbwmzt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vkkgylpr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zwbeprkr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2untwrzfc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovgjetyf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxccltxq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ltayejnt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mvwgrzan.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tikkrmgg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ayjslhzl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lhbdvous.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2urkssmds.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2btpgnqsj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zwfkobpl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mynyfrvj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyikokgo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gninrxcq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ehyicjlj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2njjrlzau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sclnasop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2sfvgruet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lozjmutn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dvyelkgy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jxxegvno.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2khrejfhm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qnvdutpr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tzkweztc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fyflxzmm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mrwfgjnx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vngliaiv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2usrqyzrr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2mbbmnemf.html


<!-- 参考信息 -->