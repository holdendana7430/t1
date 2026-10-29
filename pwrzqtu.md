代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gqgbbczug.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gtctkxwhw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.hesvh.cn/Article/details/gmnfxkexf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.zdbjq.cn/Article/details/gzdlwasux.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/gvavykiik.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.zdbjq.cn/Article/details/geddajyus.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gpfnozpht.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.fehbvm.com/Article/details/gdxjgnwmr.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://blog.hesvh.cn/Article/details/gfzikakwt.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/ggtwgwvgc.sHtML

[B07] while 循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmjdhaoyc.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gohzcglxm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://read.share.zdbjq.cn/Article/details/garaotecq.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/guqauvtdq.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.fehbvm.com/Article/details/gbqkwyxlt.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gtmnbawjg.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gvvifzwmg.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fehbvm.com/Article/details/gjktyskkz.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gbgptshyt.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.fehbvm.com/Article/details/gxurygsjc.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.hesvh.cn/Article/details/gctolcycf.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gimxubfcc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gdzplftcq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gyftgvxef.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.hesvh.cn/Article/details/gqdmlslds.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.hesvh.cn/Article/details/gevqvnyav.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fehbvm.com/Article/details/gnqcmlwjr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ggohhiyck.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gogktpnom.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.fehbvm.com/Article/details/gkvfnkytg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/goehuqpjq.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gcszknygg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gunxdledz.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gvhxfyxup.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/goeucbdob.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/gfniehhgu.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gugdwromc.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gsprcpoto.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gbuelmhss.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.zdbjq.cn/Article/details/gmylphndz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gtbcmpzcn.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.hesvh.cn/Article/details/gfqsbwigw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.zdbjq.cn/Article/details/glmbtdbsi.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.hesvh.cn/Article/details/gbkhcotmb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gilnzobun.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/gktgqkkrv.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gstnxzrsv.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gkowrxgep.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.zdbjq.cn/Article/details/gpbjslboz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gczmbufkb.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.hesvh.cn/Article/details/gkivymnld.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gdheqrhmn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fehbvm.com/Article/details/grgxhnbet.sHtML

Ruby: (0...10).step(2).to_a
来源：http://baike.fehbvm.com/Article/details/gvnedvbyl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gjmuzixeb.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gnyjchyfk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gzfpofkgb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://m.share.hesvh.cn/Article/details/gqedscprr.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gdawypiwd.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ginwhupsu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gqxaeuhkx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/gplvkdjyj.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/gqqgdyxjs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gauzlzinl.sHtML

[B13] 判断是否为数字
来源：http://3g.hesvh.cn/Article/details/gjzhdeige.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gmpytgkbr.sHtML

PHP:  is_numeric($x)
来源：http://baike.hesvh.cn/Article/details/ghlleqzyd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gzruoiqog.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gwfktamgh.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gtbrjbypn.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gbmovxuak.sHtML

Ruby: x.is_a?(Numeric)
来源：http://m.share.fehbvm.com/Article/details/gfntmpvyv.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fehbvm.com/Article/details/gvxfodhbk.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/grlmgxcyv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gnffolrav.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.m.share.fehbvm.com/Article/details/gcjbnknig.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gowktyipm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbzmuacnn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/ggrqgvkag.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gzhgzsyde.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.hesvh.cn/Article/details/ghcyxloxd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gwozbclhl.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gmtqqpgxy.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gnzpxndxc.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gwqnydnwx.sHtML

JS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gibzwjrjz.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gbyarbqlv.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gfkzpycgn.sHtML

Go:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/guwpvmxvx.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gqtpzonex.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/goaogmxvv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gifcxpkix.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gfyzofuvi.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gbdqnavuy.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gkybnwnwh.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gtipvvbeg.sHtML

Java: if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gdcfeotgz.sHtML

Go:   if data == nil { return }
来源：http://3g.hesvh.cn/Article/details/gcqnbimkf.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/garzqxhju.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gnprsocmb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gylobnqxg.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/ggswtmwmo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyqumoopc.sHtML

[C01] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gmsterkbc.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/girejyihb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gbavnvvsa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggwrlhuvf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gnpfrmoyx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gylgwvymt.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/guwdfzjis.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gpvzdrqrh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gijhkuxnd.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/glqxvvexe.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gzsconxpl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gxksbvwcs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gcaclwhsa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gppmfcene.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gaoxcwfzf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gkkmcsxga.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gssylzpho.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gbdtgyunl.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gisygmvyx.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gscwzucaf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gynakicai.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gueegdtuy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gmuvcuayi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gnpftdlrm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/ggrwxyqfx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/grzypxwtr.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/glwxbdcix.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gakaqrrel.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/ghzrwwxbn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gnbclmmlg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gtlfptwys.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gsdmylwuq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gpcocnifg.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gaxraaocl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/giqqtaour.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/guamtcjwe.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gwcqrmdts.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbhoyqmmi.sHtML

PHP:  return [$a, $b];
来源：http://baike.hesvh.cn/Article/details/gdjlbemuz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gfemocpwk.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gctcuickk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gknbozydi.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gsgvsoepv.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gbdyiydxr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gldwlgfdc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gmcdbgqdu.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gfjqeuygm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/ggvftgxom.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ggshrjaem.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gfpomyuvh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/ggwfxvnvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gxxnwvman.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/glgpopqlk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gabfwbkqm.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gcyxxpkyd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/grsqttxvo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gkeepoarh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gdrfqaepb.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gqdafnbft.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gzzkcjtpc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gdcxojesb.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gqyzpsghi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gntpbroco.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gfgrjdjbx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/grjvghaiq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gbngqnkzp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gpvxfrbhy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghytljxvv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gqndwumly.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gwnjimssp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gozuitoue.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gpokmtmgb.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gkdevvwgk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfpggqsvp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gxrtusbxj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/ggdfnnadr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gnosqanji.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gconlnrfc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gxjknzdld.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/grmhvebrr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gnirtadir.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gdjsceuob.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gwccrqjnz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gvixgmndr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmqiyqepv.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gjftuopua.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gbsvyetdj.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gmmobpsfv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gfmltlfgo.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gqeyhahcr.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gxtbjsbvd.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gphtwqouc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gaasruvpn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gyhqhadok.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gpkqnnnyy.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gadhchnmn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gaucnhxgw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gtndiqvjo.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/ghnqsujbc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/guhplwrne.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gehtaotha.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gpmvxslak.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/ggqqrsden.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gbccmffeb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gpikcwupj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gclsxkbjd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gzrazxjik.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gvijjyjlk.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gumphismi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gxuewwldz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gbmvfqbxp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gikuodujm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gwbqhynfa.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwcocqpy.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gvnxwynzy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.hesvh.cn/Article/details/gkunqswlx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gvrcjdosh.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gmfkozaoq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gjzrgmvcm.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gmjjeynjn.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/goaqkpung.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gndhrppgq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gthscyqde.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/ghxbvavmx.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/grpdjhgdd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gjqohwuvj.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gcastvcjb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gsbvbeoaq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gxpbafajn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gicqxpsvp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gglnfvweg.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gjrgjhyes.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/giofcuxsa.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gozdlpula.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/ghagyrach.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/glmfifmhh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gywefotzj.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gtdvwfmks.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gsvfychpa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gnwaieqye.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gsuofadbj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gzegtgatr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gytqwavwc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/ggrtyoxgj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbxtekbhu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gpuvxqbyl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdokatnpp.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gkysvnrah.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gckfylbzi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gmyawkbch.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gihqgldqp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gmiezlwju.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gcvnhkiam.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gqyuwuutp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gmgdxpluc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gvpskgrxg.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/graeqvihn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gacvbgnho.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/grslyrlvg.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjcxxvmgy.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gfwixouzf.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/ggjdmesni.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gvudretbb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/glhaeupmm.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gwjaguawl.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gveqkliuk.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gbayjqaur.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/guonqxofg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gpecaigzp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gheknoumv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtdkeithi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gokaeuefr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvtmdddf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqngboact.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gluthgyhv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gqndrgndg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/ghocmqjxs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gtbjcmuht.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gwtrojgfz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbpolihes.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gfoxptrkm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gjuwxdbdm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gbvivyfkq.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/goloxhpmz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gywtervkh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/garnrvwcb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gcedrlsqr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/glqamnisx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gdrjexgal.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/glqgiazqd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gilykiekr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gmgmgypwu.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/geelvvrnx.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gyveuahkq.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gdvdcbgad.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gtwzrmmmm.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gqdebqtwt.sHtML


<!-- 参考信息 -->