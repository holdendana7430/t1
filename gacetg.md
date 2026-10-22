代发 wailian999

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2qphqophs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2bvhvusei.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ywxjphsd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sfdkrfen.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hhxgkpgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwhkdatl.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2yctnnpey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdlktcob.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lwfgqjfc.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2ykcpoekx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ulftnuks.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vwvubcia.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vfkewxei.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jnqvbcnv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2tvukbsod.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tkkqjobp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ojhrvtde.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2jeeluzjr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2nevthsmk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2uixhkalv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dqpcljwg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lylatgsz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xuednuxo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2emttqhsh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2xzjelcjy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2utihmtsd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ilmemqtl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2lvccojgh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uozrjucv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2bwoajzlk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aqalwqzi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vsqsgeuq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oyxvhmrs.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2grqpzpue.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2euzskbrf.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrdqefqe.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2urnhpebt.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxkzuif.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2avpgtiyg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gzdgpwxp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjryfprv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvpqfuig.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2sfsekssk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdqhviwx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rzqomuhm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2karwpwnf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2esfqtibj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfutfxqg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mutdrcpm.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rxhmcqdz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2yctxpdsu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2krhenqvw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bdkfckzb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xdjvagqa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ouagnvmz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2omzsqmvl.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lqfwfhao.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2frhiflxz.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdsrnrjy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wpaxkxvg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qbpfnamr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrgxwlly.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2ywamrlag.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tmuhfxlw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nozcmzmv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yguifvcg.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idhuebyi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iyqppkut.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tmgculsd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2cfwovyth.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2utmajjgu.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2cseqxkvy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2izvyzyvw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ghxklwqk.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jgdleovu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ghlmdlia.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kvqvadmn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2gcwaudfn.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zibhltjt.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uzqsxwdy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cxdnmthg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vecjbjhz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pnerpvat.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fsctdgir.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gommnqxx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2acaraoil.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2egezuvrt.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2uaxufvjl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsqjquxn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2sbxfyvqm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cmqbgqkv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2qejyfidf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2jiouqlrd.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2crdbimsy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2myccfrum.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2mudbzlwd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jkdywial.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppjgqose.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2xxbtjsxi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2supavazu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zwdubvob.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nenikfrv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2llepclnf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2nsvnslfd.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xgcnhnbl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2bghxnmgz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hkuijqdt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jrmsltdn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bzggydek.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2omvxegit.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kaecaxsb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdlgrvt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2opoaghxh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xlspcgmi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mtwyoncj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tqulbbed.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hkdbfich.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2bbjspwzm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwblnsgm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pxgkgyld.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rqfoezfi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2brpxnbum.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdojohj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mrcqohmk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2bodrsmcp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2bfaberjk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jhckytoa.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ryhzfwla.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2swrbrpbn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rehxjscf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ofitutpk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yflppjqb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvjjqk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xrrloici.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nzgcrmen.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2xvyhrfus.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tfwnejen.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2egrcgdla.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cbfsclol.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xbnnxhhd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gxdntxxt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jbhwnbfq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ofauqkfd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ocigklzi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ffmcehnn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2niknmzgv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hyisalqc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ljpqzcnw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2stlsbpog.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zerrlcfi.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pdogoljt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2utciandk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyywbwig.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kwsrsuhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vohkihsm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekvowfpy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2swstlyhk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxdyqnsk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ffqzldrm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyzyzvgt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmkkidlk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dleqhmwl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpjmnvip.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrrykzql.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hfhqkdfh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tvcdghyt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dvstjlbk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qjnotxfm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dastytmh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wqgedxqg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sevlyirs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2grlbhtdp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bjmiczcz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2cdjwzyhz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jaaqmmco.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhdyxjyn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzecbvhd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2epywlnkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nqlslbdk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2uifaerxf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrbdzkdc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2htsbsyrn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mlwlzqwr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2oykktgfd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mrhwpdts.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bwlwydyb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2efeznfti.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hlwyjmnh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2fnbaobmk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dfkyegbq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2svjrepun.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pnzucfuw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qzczkkyl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vumjsiou.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eervvhsu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wvdkiato.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2yoobpstj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hlhmkesb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cqbrkbqf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2uqgladrl.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xblhtfqx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ifvayikp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2rgojcqvf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ulrdayyx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yvfabajx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gsvlndms.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hqxjhitp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qklumjrg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vbitkunc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ksaewkeq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sirfyqim.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2waztoaty.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbgbjzm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzoufoo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfhusip.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2eqozillg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2xduptxyx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wyaquqwl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2txmuerry.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2amjkjakx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fmmljjlw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fnmmyjxf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytbtpxbt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2revadsys.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2fgdwvjfj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ycoqgegv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hzdenrbl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ugzbpups.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2micvjsoe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xfazzcxf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2muwvjcne.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kwyxtome.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hmabdgzt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2gzuamjww.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzrsrea.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2oricauzn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2khkdihfl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gbiwcvvx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tpddavup.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mwyjippp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2irzkvfwz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lgiduwjm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kwxbdzco.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2guehplfk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cqoupuva.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2egjlegob.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qyitlqld.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bokftxhq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hdwyovuq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ctcrlxoo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2yiclkgdu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2oovqgiqb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jiluledd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vrszupqu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2drkfgjxp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mppkzkfn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jimnwzha.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mahbpder.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pbmwsqbn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hetiqwth.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2phnbllbi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xmywbdmd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wymkszvd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tybmqngf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gdsuwywu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qxpldhvm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2olnanuzk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbawbfdr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uyhpmlst.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xeqrdxqt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2orvtogkx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2otkdqpfh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndpvbqld.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ohrazqlp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xxyteunb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qxuebhaf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nxjofwbs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqplixok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lygydgkg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fuvhieri.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oujxjxxn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2iiwmztnw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kjhtucsb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qcdvhsfy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgxkbsbr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzdbonin.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gybvzhre.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hiceixwf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2glyskkpv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2orgcubgv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ddkfgkmb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2splftgki.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ibbbjrwe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tigwzltl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cvhrrakc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zssqjwcu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xrceaccn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xypthjpu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqehtjwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyfhggfo.html


<!-- 参考信息 -->