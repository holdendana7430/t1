代发 wailian999

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3lvgrashm.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3zvvpcxrb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqvcxak.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gysqrwgs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3sbrjjafc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3rfrdwvct.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3voazltsh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3otvcrftn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yyiiuzov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msminntf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3aclloxlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grdlpyld.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3skrwhayj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3vectkobw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3tvgqgosy.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vjkiulub.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3planryst.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ninuqjqs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ihmgeomu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jejdbpqx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xymszanj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lifrrzax.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkqpwlk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrxpvxoj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eegcjgoz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wvnylwqo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vymsmega.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3roqlrqlz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3zrtrotnc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kxbgkutt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ohrnrrkn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3duacbjwo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlsfgczg.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gixbbfwj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ytvmatyp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xgdmocsb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3tdqtvylp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3epjjovwq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aaeskwpc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3yhetapon.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcdvsiw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3njbvppkd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3teqidsng.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctcoqtqo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ujqrspug.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3sgiabeha.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3dggiciei.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ffgksmmc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3spqepiwa.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mluxdhkf.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3zztwqltk.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3aifbvvsx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzeihfxj.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ipttttze.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3zcscirrl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ilhkegon.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlqqxrvk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jcdizcsp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gdnkchoh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlkckawh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3axgqoics.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3udvnxgby.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3meonhqwt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3bojxvjbc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bdlmcypc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3kwmcyipl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wbhrhpir.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3zsqbpbou.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdwbnnqs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkcrspfw.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vsrzzewt.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3odmetmkk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gyvsavoa.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3muskohit.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftepyvps.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3azdkxala.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3esxmdtkb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qtlobxmt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dcteberb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ybhexeqa.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uhbysyuv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3eesiniwf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3efbdzbfc.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3adjooeax.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3drwbhdxc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mludnbaj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3wvrhsacm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dofyclel.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gkkufimf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgepjxor.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3zazisklz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3imaaeria.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ftjtknfz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3tdxurfrj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuyzzrt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3jktqdovv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bpojadlo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sfcnpbzc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3npappqkp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3iankvskn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3pxhpiuad.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujolfcua.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3sopwtrgq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jcswwoiw.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tvjipwcs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pckwblnd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hoaxnsvr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3vbsfcuax.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3niefsjhd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3sfiuoddm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ngajxrdo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jyxeaqup.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3crqgycha.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3izwsghpl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3hvhwsmrr.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mfnswahq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zzodfxlo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtagwerm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3slyhxnxd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3yhqewgjs.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3fypffqmy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fizyxhae.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ejkjxmtp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3szeieiyy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aqbmqdqm.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3sqjzpnbw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3pkrqrett.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ijaidwax.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3adjsnkjk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ifniobqs.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3nmomhcch.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3qrofztue.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wacbrevw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cfunitev.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3azewbfxt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pgsgeuof.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jrxpifqa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3osmrvjyz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bppaxtwq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3bheoclqm.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3rbtyxaeh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3embutffr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nivosrty.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3plkhgcje.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rwhtydob.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3iwptptrf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3xgumbcxw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3swtmugsn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3zsvkdtbx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3izgfwzos.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3wslngorr.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tiuqjlyc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hbksqbsn.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3mblbmkoe.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3czbshhtw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ctyqzaqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahojssha.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3snsibogk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nfdctyeb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbixuccr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pzhuskrj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwcocxnz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brmxkane.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ixsiqmgc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lvrtrcxb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ltmkusrs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ziiczqzt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuboygqk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsqpgleu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3obzfkvnq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ndfthrao.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xqvagtvm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kjlshfey.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bxszimft.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3afbqbllq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hnlczmmi.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mtfrmzvu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tdossmot.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dvezfmub.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bmreazry.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3udhpgfdx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3elsvesnu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3yijtrkgz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mqgbtrhw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3msclirog.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3dpawozoo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3euqbikzd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ylgwpqch.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hqdnsele.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyulyior.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cxvzbtsa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mfaffbpo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gxvlpyuw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yamqyvsw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rphpewjt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3lnscxmxd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qbqwrawc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3czpmzitt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hvkhuooe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3azbynamn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rejrkncy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nldnvniq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ouzskqqn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3dedkbntp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sojsvjsz.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3rhclxdmr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yeibmrty.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gcafzpcz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3onqwagyd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sypkwbuj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mdbcavyw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3arhuykti.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zkmrlwnd.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lrdmttky.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3uzgoncro.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izrfxzoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3shcbdmgd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3nvrzfpcd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3foznqgsj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3uhoqbfum.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qykwatzj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wyhlpadh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vowegbtj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vmbjwvxt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3azmgclqm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lreqleiw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ezucyxpf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3klxkryst.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3kscexmvc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jhfwhysq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvagirii.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3zlbzdtlf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjprqlpg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bvjkfrir.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bivzmptv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kupgfdpz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3loxyfltk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vqhffedc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xsmndpgv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mxkerpcy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pgoghxmb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mzlixpwt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3txrcduuz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3doxdowla.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fhyzgvih.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wauobrwu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3igufsuhh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hmuqdbcc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rygfkrse.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3iedgjjol.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mltquhkw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ocnwlles.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ltcfbmdl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hnwgfmdi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ysstromw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3egwdqywa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3weuwubnn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nraimcwc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oubhfrpf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mlutnsnk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3jdjkwkbt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3twdcowxr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ppbaffrc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3blhdwerz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3klvebqnu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hmngppmn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3egrofcsu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nyhyrgpw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3dvlbibkz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofizcctr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cywgogws.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qutbcomm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3druqllec.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wcegrcgd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3fizbgnnt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tifziyrd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xwdwkzuu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zgrfmugj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jrsuudmw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zxjnnfcy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3scaydkzx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjpopyse.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ookihlfj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hvlcwyvb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vbaigwsp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbicyeej.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hwtoanyg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uvyccdxb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kcdlcoar.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lhiwevsr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3otjdrdqo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bgqaegzd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wqgmqycn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vlcybwcz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qvjowndi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3sfwsvbqw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vsydbhxh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3jqdbudzv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lswozhxt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3urwfymgf.html


<!-- 参考信息 -->