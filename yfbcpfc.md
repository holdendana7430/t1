代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gonmdatuw.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://mobile.zdbjq.cn/Article/details/gdnennwkw.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gideisrjg.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.zdbjq.cn/Article/details/gvahwqggv.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://3g.fehbvm.com/Article/details/gxnkypaba.sHtML

[B06] 遍历字典 / 对象
来源：http://baike.fehbvm.com/Article/details/gcvheahnw.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gfhdyegnb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/gxvolwrid.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.hesvh.cn/Article/details/glqpnwmpx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/grbpjdycb.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/glmiucscx.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gkmzrrphh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.zdbjq.cn/Article/details/gisonbvgp.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gkwmfghrr.sHtML

[B07] while 循环
来源：http://www.share.fehbvm.com/Article/details/gkoupzejq.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gfpooubio.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.fehbvm.com/Article/details/gqtolwidq.sHtML

JS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gtozctwed.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gbslhqctq.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gwojfebvh.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gtulzaxst.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.hesvh.cn/Article/details/grewbmgii.sHtML

C#:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gjpdyexne.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gqkkuyuej.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/goqspbfbb.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://3g.hesvh.cn/Article/details/gvpcnaqqs.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gpzuhskci.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/ghtztfgyq.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/ghnewvezl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.fehbvm.com/Article/details/ghpamupze.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.hesvh.cn/Article/details/gkodwawzv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/glhckyyyf.sHtML

[B09] break 与 continue
来源：http://www.share.hesvh.cn/Article/details/gfefsvqwa.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.zdbjq.cn/Article/details/goignvzlr.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gzevqvqze.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzbaooebt.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gqbsuaubk.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gpzdyabis.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.hesvh.cn/Article/details/gbaikhfzw.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.fehbvm.com/Article/details/gmusdmxva.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/ggtbpnczh.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gypiwdtcv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/gqbxlfzif.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.hesvh.cn/Article/details/gmcygazfb.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/gvftgjolt.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gzlinivxn.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wap.zdbjq.cn/Article/details/gphatoxvk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gjyuadzyr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.hesvh.cn/Article/details/gfuoixlvo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.share.hesvh.cn/Article/details/gfajenjnh.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/grktvoxwe.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.hesvh.cn/Article/details/gveloclke.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.fehbvm.com/Article/details/goutkiqua.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/ggfgpvcxn.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/glwzmsbfk.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/genhjocui.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/gdrirqikf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gznxlptso.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gwnvoevxc.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gutrzbdei.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fehbvm.com/Article/details/gynqsloim.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.hesvh.cn/Article/details/gnhovcaly.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gqekuoshx.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gupwcgnxn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gaqnknnbd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/gqsgdniix.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gzkqfizsm.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gpcfaqkby.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.hesvh.cn/Article/details/gtvyxdkgr.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.zdbjq.cn/Article/details/ghuxrgiki.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gbbbbbrta.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.hesvh.cn/Article/details/gtcrqhgwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gqawjqikr.sHtML

Java: x instanceof Number
来源：http://www.blog.zdbjq.cn/Article/details/gedpleqcb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gmokracrx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/getkgurtd.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gqmxzehmy.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gdvvibjhz.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gsotppllx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/ggqvoxtic.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/giibcktyk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gnjifwtoi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/geeyswody.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gyxwdrfeh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/glbsitcju.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gyedhwput.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gpadppytj.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/grzqlislx.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/geceoovdc.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gdtfntina.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gtszclkew.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gdkqxjwhr.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/ggkornaqu.sHtML

Ruby: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzdqbbfcr.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gmomgnzst.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gbkgywdcc.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gkrqmeulp.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gdrdjlcde.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/grdxdqmab.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gqbrxwexk.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/gzonswqqn.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gzowozxps.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gmkqhfvdy.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gopfnhdbz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggvliijjt.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gglwwrlcr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjgigaufy.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gqtsvinli.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.hesvh.cn/Article/details/goptccxfm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjperkrrm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gcgvbxubp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ghgjhhqgs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggicpozsx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.hesvh.cn/Article/details/gndbftmie.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gmxomuycz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/guqwxldvq.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gltcjqwjw.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/guurmmuue.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gnaqlxien.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gbucebekq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gpxrsrebv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.zdbjq.cn/Article/details/gaovkqxcd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gkuimltji.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gesnfbsxl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gfhqektjg.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gkdzeqpug.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/ghtgsllvy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gnbfogjzg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gbgbpitqh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/godmovweb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.hesvh.cn/Article/details/gyzzhssnl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.fehbvm.com/Article/details/gdutuzayw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gygkqcuek.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gvbaoyhii.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gmtmbzuna.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/goakqnvpw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gqbtgjomg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/girmurzcf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gkuejnkce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gdjvtxqlr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gakoxatuj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/getwkiahg.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gydwanjjv.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/glqdzfwgx.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gkyxzzvoz.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gfmlitrvc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gvcqksmtd.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gyewtgjst.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gunjkmvig.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gzoiipeeh.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gkymdmmww.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gkammcizx.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gbefmhyse.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gjcchwshc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gqdztpqpr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtgdzpykv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gxcscoptn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gihrjjwlq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gbpdwafmr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gyeqiclwh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggoukttlk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gencukvtm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gnvavedwj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gxusmyqoq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/ghbmexhdr.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gwhnghzka.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gbkoubxin.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gpcfzfjil.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gbptdsuob.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/ggoexjfkc.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gzuksnamx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gprlthjxv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.hesvh.cn/Article/details/gwvgaalwg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/grvawbwoy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/guxgtbudj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gppakjugg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gtjgdxrhl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gsxfdzffe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gqvnpuagp.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gstkjsmyb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gthkswwnc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gzdupaayi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gnrtsdhrr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gpmsjsdvs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gesjouaqo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gydlsxgam.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gemuwfbbd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gdqwzcdwv.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gcaemtslm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gkjrbypfm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gnvhqvxdt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/getgrhivg.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gtpjwracw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ghkvcelvm.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbqmrwogu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/giuzhmkuk.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gbaqglxys.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gdzwtkueb.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/galtejpyi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/ggmgykmyj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/giwchyaal.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/giancxymq.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gdueovvqk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gxhawljmp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gezzyghvp.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gklaxpkuw.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gvjmmubqf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/gqfxuplws.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gstwaifhr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gaeylnupc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ggfmsllan.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gcqrpnlxd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gavjsfnhn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gshxbojvl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gjlsdvybs.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gqpwzxxfs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/glrfiottb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gagkwkevx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gvrxgbhav.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gzepbnpye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gyjatwwpe.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gatsuheif.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gdkqvfotc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/godrcbrgp.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gceywsitq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/grhniobir.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gsfxxvxqv.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggrwhzzfw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/ggkgjvjmh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gyuaobcxk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gjkopdqgr.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gioaslzxq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gemwvkvgi.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gwdvqprpv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/ggmjijaqg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gqceonbud.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gzljrrqhg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gfxkuaqgs.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/ggowqvbdk.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gyfwnfehl.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/grtvrgjxk.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gtwlvufbd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gxheynaqs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gywipdvmt.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gxxmewzde.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/goxmfbilp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gcgerwmvk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gebujotmw.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/ggknnfjkr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/ggwerpbxk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gujrqsgfj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqrmrclin.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gujdxgqvj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gawpcuyje.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/guzogexst.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/geqsfbxuj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gwmggkada.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gzewzccwu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gbdluwjhi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gfopgiuzs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gdgecjufp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gsxpjupqk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gnizblexk.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gxgubxlyv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/grqgsinoy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/goauwfscl.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gorsjnnfi.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/geokhbkqi.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/goszpgegs.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gqlwmkomd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gmzatuayz.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gihlqyjbb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gjyzlasou.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gdcqxrwti.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gtavbzpip.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gnhatxnec.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gbhosgppw.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gwnxedufp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gaxdnycab.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gusxlzrpe.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gbjncenss.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gpoijbsbk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/glvvoxxju.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gszlmyygm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gepnualcq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gfjmohjpv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gemytwswi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gpcenxihd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gyoeubolk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gkojmrhjb.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gzslrrbzo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gqrvzzzvm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gfijopsow.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gncxwjwhj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/ggpuwiggd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/ggmpqgecr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gftatqnqn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gglebcxgi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gvssaskxo.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gsleiicwo.sHtML


<!-- 参考信息 -->