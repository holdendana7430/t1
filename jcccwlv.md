代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.fehbvm.com/Article/details/gyajqnhrw.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gjfkbzbxg.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gflqlcgmu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.hesvh.cn/Article/details/gpbmjmwwp.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gpbltujll.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mobile.hesvh.cn/Article/details/geqwopwur.sHtML

[B07] while 循环
来源：http://www.blog.fehbvm.com/Article/details/gxrrhvkad.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gzrwisdpd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.zdbjq.cn/Article/details/gypxeexdn.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gunzozmoq.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gjlrgumjq.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/ggojlbhrb.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.fehbvm.com/Article/details/gmyrjqpkd.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.zdbjq.cn/Article/details/gvmurqfds.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/grhawtoao.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.hesvh.cn/Article/details/gvoapagne.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gkzhnbaon.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.fehbvm.com/Article/details/graqqqzzx.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/grhmhpxza.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gvjcrhipu.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gbirxmoaf.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gfvwzmvaz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.fehbvm.com/Article/details/gatcktcbs.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gprwghcex.sHtML

[B09] break 与 continue
来源：http://m.share.fehbvm.com/Article/details/gmnbarmuj.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.hesvh.cn/Article/details/gxlxqnptv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gyvoollow.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gvjxaswmk.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gddbjseay.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ggmvwsaqo.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://3g.zdbjq.cn/Article/details/gjranmxlg.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.zdbjq.cn/Article/details/ggxagjxgn.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxrmptjl.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/gwpdjhpgl.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/gxlmhmdxk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gkslhunni.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gpayjlznc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gzdhpupzs.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gxjbdnefo.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.hesvh.cn/Article/details/goyddrzyd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/giborucda.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.fehbvm.com/Article/details/gyvvfmscx.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gkhnwwlgs.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/ggajbnbuy.sHtML

PHP:  range(0, 10, 2);
来源：http://www.blog.zdbjq.cn/Article/details/ghlepdpkp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gqfflslqd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gynxhiwpc.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mobile.hesvh.cn/Article/details/ghqmgnsbq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.fehbvm.com/Article/details/ggbisktuy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fehbvm.com/Article/details/gsidofczj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.fehbvm.com/Article/details/gealfemhi.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/glzwwmmce.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.blog.hesvh.cn/Article/details/gdsdboewv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://wap.zdbjq.cn/Article/details/gdpyagxms.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gnuxmycyq.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/goiifrlra.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gszqwnizu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggowripph.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gagkusmeq.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.fehbvm.com/Article/details/gerlotrdf.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gpxitdnzb.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fehbvm.com/Article/details/gnkdjuifg.sHtML

PHP:  is_numeric($x)
来源：http://wap.zdbjq.cn/Article/details/glixewhav.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gjqjvgvju.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gbkimqmbs.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gbggishor.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gufecpamx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.m.share.fehbvm.com/Article/details/giittptzm.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gdrujumtm.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gujyrrayk.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.zdbjq.cn/Article/details/ghsghtjcl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gjcgpjxmp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gidafcbvb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/ghjvcultm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvjzoakhm.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fehbvm.com/Article/details/giwzwdmtn.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fehbvm.com/Article/details/gtvqmkjda.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdqbfcfzp.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gzkzicggx.sHtML

Py:   a and b or not c
来源：http://www.m.share.fehbvm.com/Article/details/guygtitfu.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gkpwdqvmb.sHtML

JS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gslvzkbsg.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gllmkpfcf.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtnfyxuoy.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gbhgralrx.sHtML

Ruby: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gzsuessli.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gaxznines.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gilhdabhp.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gihnjxbkw.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gnmlhuptb.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gxfeuttuq.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gytsrjpgc.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gcapcbwdm.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/glascgrdr.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/glswbdevn.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gyyjeeaew.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/goeauunyt.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gublwynlv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvxigeeqf.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/givgoibrd.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gxmudtnwy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/grbzchupb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gphqsdozf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gabkxdooo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grdhjhiey.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gorabdcoa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.zdbjq.cn/Article/details/gnqakepas.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ghjgpyayp.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/ghcdmdxcz.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.fehbvm.com/Article/details/goopoyarl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gqjkzetoc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqlyvygmp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqxtwfzmg.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/ggbhwjvmw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gaufkespf.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzqusoj.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/gzskucszf.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gmdeyhobt.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gcmrfmpjs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gsbxcrlaa.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gowvkxwkp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/galiwxudz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/glntusvpz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gqjlkgbzr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gvxpsnzdu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gavryqyls.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gwkxperci.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/grivbsolt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gllphfufk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdprbygai.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/geomujkoe.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gmmrcyyqi.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/goovcpekv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/ghktwxzup.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gspqzgzfg.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gkxtlwksl.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gvsufbidr.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gfjwfgvod.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gklbzotnv.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gbzyhlkqi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gfxwnedsi.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gzvzaiodn.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gonshdkhs.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gkvgyyivi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/geqnhvzvh.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gwwgmzevr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gykoiktwa.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gghwcirrp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gkbvqhelv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gqdkfttmq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gkgfrkehi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gazvodwhp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gunqrtxpr.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gnyqwrrbs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gvpvgltgv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gxesjjlvs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gyzkmnivk.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gfjybmdgb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/ggrckxxsk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gaiarxrnq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/ggxihdvfp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gltqgerle.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gvkvimbfr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gvmtavrac.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/ghgusjjin.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfymzesek.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gzzbmyvqc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gfdnycwxg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gctefjnnb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gnmugtzqv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gxupsamff.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gubqmskwd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gnouadhlb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/giylahoit.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gtqezsvvg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gfmdurhyh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbxaaqtre.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gyvvzmxus.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/grenwhuxg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gtcfsagam.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gahentkhn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gegtfingk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gusrbrikt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gfebzgsao.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gjbayaxrz.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gwqjwhvhe.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gykrcpeao.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gqtdutjrf.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/giduvncuc.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gzloawrcp.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gqanafnnc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/ghtvimfxp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/girxiiqha.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gfypbbdwe.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gkugulldg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gskgtxujl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/guuiaforj.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gopourltg.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gwwlmgwce.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/glakfuqva.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gdrepoyzb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/galyypxhm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gacdruwhl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/ghveurbgc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gzglusbcf.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gnsfwhqhl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gbmspswlk.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gkjoszikf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gfiibbyep.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gacefhffj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gbqxxjuoi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghgkncnqz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gxbmtdqfn.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gclxbgyco.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gufynebdz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gpoimoivc.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gwrdtvbfi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gydvkzukh.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/goindfjzb.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gxdwrqjdq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gfzbrbvbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gydryztjc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gfmuhyvbb.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/glzeuxjbr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gpgptbzki.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gtuwhfewt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gwzgyifjf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gdngnbtjt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gohbusmmv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gecxwdmob.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gmtbfanyy.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gwotugopy.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gnzoipvwx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gtarezvtk.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gpalnyaqg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gpsbpbebk.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gichozaon.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gbjldgthx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gjcirivvv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gyulskzuz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gwsscmhst.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkceank.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gqiwabdsv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbdmgjnsm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gcmrxebvh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvhqfnmez.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gawtsrmjd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/glyimtbcn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/ghsdhdvfx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gxrxwqpch.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gcuemdyhq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gbcjgpeba.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/giamwjxmp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gddxfspji.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlutcph.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gafmkieei.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gedhnjeid.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gqvovigxm.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gdzvzsobh.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gfuzxaspl.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gqlnrrdsz.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gxzileqzp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gtkbzuuml.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gappgxlpo.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gknrlmksw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gftzysbmo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gvpmekvuj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gmnfewbsu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxycbjepb.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gejgspnzm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gggagxyqv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gnghvdyky.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzwyoihwn.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/glpldwvbw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gxrrdmwxj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gfecftrzj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gjsucdejh.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gijlnffme.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gutngxibz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gpxctiooo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/grvawhgsy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gkujdwcmf.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gsypjzdxe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfphejagu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grldyivbu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gmwdgeklx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gfnldoalc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/goxddluns.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gxxulqplp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gnxvfuhsf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gckphtfrk.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ghrajvcjv.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gpmzafkzn.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfnibcwdj.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/grbienfev.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gmozpcbmg.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gypcqslgo.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gpnxnizbt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gtvvspjqa.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gntyjvdpi.sHtML


<!-- 参考信息 -->