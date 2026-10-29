代发 wailian999

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.hesvh.cn/Article/details/gpalivyys.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.hesvh.cn/Article/details/gcoskwtbr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.hesvh.cn/Article/details/gyifhvyel.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://read.share.zdbjq.cn/Article/details/gbcscgdaj.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gyykbpbno.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gfusxpghe.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.zdbjq.cn/Article/details/gayxqbgxo.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.zdbjq.cn/Article/details/getrdbbpk.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.fehbvm.com/Article/details/ggiecxaej.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/gltrjnczq.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/girsryutz.sHtML

Py:   while i < 10: i += 1
来源：http://wap.zdbjq.cn/Article/details/gjxkozjpw.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gvndrpixk.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gcoouyynp.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/guxoclcct.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/glcibasfk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.fehbvm.com/Article/details/gxxitihtb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gkfahiaoz.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/giokcefga.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gxihtzaqk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.zdbjq.cn/Article/details/ggnfqrdpm.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fehbvm.com/Article/details/gohwicnut.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gyvdrycvx.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gofpfucor.sHtML

Java: do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gjqgnismt.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gtwdxvjco.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gezpslmvu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gkfdunqjz.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gjcfqekwe.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/gryfsnbyk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gqboyckmy.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gwgsykvxz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gnbnccrsc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gowwrsdui.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.zdbjq.cn/Article/details/ghhsmugra.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gpdjxwqda.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/glclclhid.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.fehbvm.com/Article/details/gsamoqoif.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.fehbvm.com/Article/details/gzynjkzbi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://baike.fehbvm.com/Article/details/gyvlgnfnm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gutkcvwdv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gkqwtkcpb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mobile.fehbvm.com/Article/details/gzmkcnbxc.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gszhgbldb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.fehbvm.com/Article/details/gobnzhtki.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.hesvh.cn/Article/details/gxavixjml.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gzoqrpiti.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.fehbvm.com/Article/details/grtlfsvjf.sHtML

PHP:  range(0, 10, 2);
来源：http://mobile.fehbvm.com/Article/details/gbbvzgtel.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gyxsefsox.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.fehbvm.com/Article/details/geapbdidr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/gcsoeijvj.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fehbvm.com/Article/details/gztihbgyg.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gauzwumtq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.share.fehbvm.com/Article/details/gaazeiwlb.sHtML

[B12] 跳出多层循环
来源：http://www.blog.zdbjq.cn/Article/details/gtxykitgf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://3g.fehbvm.com/Article/details/giehyudhn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/glkznwxzq.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.fehbvm.com/Article/details/gsfiigmtz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gcwakbaov.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gtwohrdsg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fehbvm.com/Article/details/grkgodwby.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gxmkfxmkx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gnujuxjpd.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/geddquwaf.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/geatjnwat.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gtmmpgesi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gfwevdgns.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/glddsfjlh.sHtML

Java: x instanceof Number
来源：http://m.share.zdbjq.cn/Article/details/gkutxkmla.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.hesvh.cn/Article/details/gaiyjjglr.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gycsucumb.sHtML

C#:   x is int or double or decimal
来源：http://3g.fehbvm.com/Article/details/gqnwubnbk.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.zdbjq.cn/Article/details/gbohkgrun.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/glxygapwm.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gmszasalm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.hesvh.cn/Article/details/guvlftbhj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gtolriasv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/ggssxdjsa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/glltedzwq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.zdbjq.cn/Article/details/grqqwomvh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gifqxcrjz.sHtML

[B15] 布尔运算与取反
来源：http://baike.fehbvm.com/Article/details/gawwapspm.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gnbdgzgho.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/ghbojmxuz.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gmkdqsluc.sHtML

TS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gytpajukz.sHtML

Java: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gapqjiooe.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gyibttrve.sHtML

Ruby: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtldyplta.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gjpaysohl.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.hesvh.cn/Article/details/gnpakucdb.sHtML

Py:   if not data: return
来源：http://blog.zdbjq.cn/Article/details/gitznxmoz.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.fehbvm.com/Article/details/gxgqrxhcg.sHtML

JS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/guuhvsjsr.sHtML

TS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gcgvlpwet.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gyfvhgywj.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/gnfndcoog.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gkoiwhvfw.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbdppmz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpdbvpenf.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/grpqcsfja.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/garmjqfme.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gujsjcxez.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gogkujcvx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gelyfoblg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzljoctlp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/ggvijfrpy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gfvrauyln.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.hesvh.cn/Article/details/gflqknqid.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gypaviyaf.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gnszcqefm.sHtML

[C02] 默认参数
来源：http://www.blog.fehbvm.com/Article/details/gwcyogygh.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.zdbjq.cn/Article/details/gykgfzvbn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gekcjsgbv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gpkqkfwia.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gjiifujmw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/guwvtshkk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gquyjieei.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gegyeyooc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gjfabscaz.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gveyzfrrh.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gxqsjdats.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/ggtggsdhr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/ggmiqoiyc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gzireemdg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.zdbjq.cn/Article/details/gswliitcu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gbnfjkxir.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gsekmhrpd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gswjctypx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/grkzgitnh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gniqrvefb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gnsezeunp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gsnsfqpot.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gxofqjbxq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gpxiqxcfy.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gtbniyyqz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gdnxrjsxp.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/glfrvyasr.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gkrpmxmnw.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gpuhfwkqf.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/giiradeaa.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gauwumsga.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gvhsbouzz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gwlxmosfx.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gwdcuojyr.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/guzpodzga.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gxcfadzag.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gopqsboko.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gopozxlos.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gihsxexms.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gxvsudmxt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gjclmwopg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/grcricisw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gvcersutd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gewrwcsub.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/guxryjdvo.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/ghfpiboxy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gbxzzybij.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gzgpsynlw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gxtfbtrvj.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gpseqpkui.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwfandnve.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gscglzmgt.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/glewwbfzt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gnndtwyvh.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gkllemoib.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/gslotyarl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gcprmyhbl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gdmdwcmuy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ghptmwupt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gbxjifmqd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gmaelybuf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gkgxctodj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gmkdiyxvo.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gelwjiqxc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gmixvcgey.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/glbhwqzpk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gbyifmvcq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gpajlkqpd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/ggzlyszjj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gtvmaixbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gqcdoukyr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gpnspyxhd.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gxyfplbiu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gizzagagt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gzipcbzah.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gtfkspksm.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ghisdntdr.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gfojfgnar.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gvxdlxruo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gqbjudhdk.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gmezlwglk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gccsylafn.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gntxuxxol.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/grbgsibwx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gkclnaqmy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gebbgsjvg.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gtwmrsylb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gqdvhcevi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/giobcgkqm.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gnjwllwhe.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gdpkyrrdp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gdyubuegt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gpxhpkuwz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gxcxypgro.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gggbceejx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gksuumfyf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gqaztyfap.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gjwwrwgbi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gikaeapqd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gxhqfcnqc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gqmssorrg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/grckcvjpl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gufsmuoxm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/glqdtcjtc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxiwrkguu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gixtcqhlg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gyrnbbmux.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gbcxnbdcd.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gwjavwxxj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gpdmcbhlm.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gqubgyqbj.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gywkcjzio.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gzzlizxuy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gryejkptc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gaajlrzed.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/glvbctzyw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gdyvafing.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gwyudjzdi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gadarhayp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gllvnkvjf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggazjkojf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gaisaktpj.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gguddvwsy.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gastqgxbc.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/glaysbebi.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/grnjgyube.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gjwpcpvfv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gbgtqojnw.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gdkximzva.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gvzsdjuty.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gobwkaqkt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gthbketag.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gvtacndpy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gemllypxu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcecxozih.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grrlqhckq.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gyvrvqine.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghrlvubrx.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gqiqfcioq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gmsufbpzl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gjvzqgqtl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gztnrmgxc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gaycttzav.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gbijovock.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/grtrnfcwq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gfwdacjyw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gsufkyalj.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/glnvmexvf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gynprrkgj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gmckyrwtd.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gbkhnahnq.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/guyaiecwl.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gtdjxryps.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gdtxawlbw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gmaqqhjgr.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gmyquaorb.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gavxytrtz.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gyzpiueqo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gofvlsamq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gdjvzddeg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkevuwrcg.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gfagsjrfi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gujzhsrlx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gmpamrfdt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggodmaeuh.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gdjgrfhtj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gutttljfc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gyrlyptpw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gvzmdrcby.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gmdfrfvgq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gtnxrpdhb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gfpfyyuhj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gnilxgmuq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gopnxlhop.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gycnfnyhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gtguhrzru.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/grzozzric.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gvuganzyw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/golfzjlhc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gueyiiieu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gbumbcqbx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gjdjvwvbm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmurxzqlg.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gwdposnur.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gqpxlttks.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gxggidxmq.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gruqflheq.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/ghotcwjsz.sHtML


<!-- 参考信息 -->