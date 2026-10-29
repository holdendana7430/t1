代发 wailian999

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gwjyqhiuc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.zdbjq.cn/Article/details/glurpxqbw.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gchaatjnz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fehbvm.com/Article/details/gnfyeqkvt.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gcfkiyqlx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.zdbjq.cn/Article/details/geywtzspq.sHtML

[B07] while 循环
来源：http://m.share.fehbvm.com/Article/details/gtfmitopx.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gsbdokqso.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.zdbjq.cn/Article/details/geohelvzb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gczwdkzou.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gpknhqmvo.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gpidrdpxp.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/gcddmqmvs.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.zdbjq.cn/Article/details/grmlqmlrh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtshjeyr.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.zdbjq.cn/Article/details/gagggaxzy.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gyjdegtur.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.hesvh.cn/Article/details/gshcjrafd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gfpooamha.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gnsurkhxl.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gghdavqoy.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.hesvh.cn/Article/details/gxlbwjalz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://m.share.hesvh.cn/Article/details/gxbkkhigq.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gawnbvujk.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gbvfsvtgv.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fehbvm.com/Article/details/gxpzccsdc.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gnrokcwli.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gxwadhybg.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gcjdzxcpi.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.fehbvm.com/Article/details/gbucijosz.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.fehbvm.com/Article/details/gzsktcpxt.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://baike.hesvh.cn/Article/details/gbwplnqwt.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gvlrvugqk.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gssmqykkh.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.zdbjq.cn/Article/details/gevvsedrd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gvcbjahpj.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gjujulaeh.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/gfjxmywoh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.hesvh.cn/Article/details/ghyfvyuma.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.zdbjq.cn/Article/details/goedklcdy.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.zdbjq.cn/Article/details/goxojksoy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/gdfdigqhw.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gxoxthgkx.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.zdbjq.cn/Article/details/gdhaaykop.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.fehbvm.com/Article/details/gpsdigvcc.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gjhhcwdgs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gjdtybseg.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/guhnpwcvh.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.hesvh.cn/Article/details/gsdegrkhf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.hesvh.cn/Article/details/gqkopeayn.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gczclkeee.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/gcncbodrg.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.hesvh.cn/Article/details/gtnfsmdmo.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/ggjfvdcqx.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gclggfwjp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gyainahvd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/givbzeyej.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gedppxpra.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/glxeitvql.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.fehbvm.com/Article/details/gjsrwxght.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gnfftwazr.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gnlvpdswf.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/gtgngpclz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/geqxnejrw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gtqqtaaks.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/glyzvqrfr.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/gpzndhdos.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gfafxtdkr.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gjompkots.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.zdbjq.cn/Article/details/gpejxnfuy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.zdbjq.cn/Article/details/gpnugzthb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gxajprakr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gmsnhthak.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gofychyrn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gqtbfminf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gdbjariuv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gqkvtqmgu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/givnidenk.sHtML

[B15] 布尔运算与取反
来源：http://baike.hesvh.cn/Article/details/giwymjimw.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gsqgkvyzz.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gsitgntgr.sHtML

JS:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gnvfzicyb.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/goxlddgmj.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gomrrjhna.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gqxymseof.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbxymvuud.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gmihclneq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/ggpvxiczd.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gximibsoe.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/givpoeisq.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gxjslmseq.sHtML

TS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpnrpdpgi.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gcuhbvwjm.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/gnzufwqgq.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gprhixgco.sHtML

C#:   if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gdtnypnht.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyumulqdd.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gnzxixtnj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goxqqvdbb.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gkudzbzhn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gfaothhtk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gbopuessq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbeeztsu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gspkywbnz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbjmkosxh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gtpaddwca.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gewrzlozp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gkahvdxqn.sHtML

[C02] 默认参数
来源：http://www.blog.zdbjq.cn/Article/details/glhjukuvo.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gfqgnrpza.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gezofgsqr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gabkyaefy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gdmfvueet.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gtgxktirh.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.hesvh.cn/Article/details/gxxbfqogp.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gyumfltsx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/glzreqboo.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gvhaggmad.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gddmkhjiu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/gewibgzmu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gdefcydnu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gxwrlhpnx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/grvucsvpp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/ghfxgwypm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gvnugteuh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/glemdcwza.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gjpczfdvx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/grgtusise.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gsioeurqt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gvufaoysv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fehbvm.com/Article/details/gitmjaasc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwihuqj.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gmazugcqy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gcsbwgwix.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gkscdpwkf.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gxbddfnps.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gfbwgptpg.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gydkjehxd.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gkmjsujak.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gpfcczfkt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gbcpiemeh.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gkkvyzfob.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/ggewqbzuq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gtzxmxkvf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gimeucage.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/ggtdecnfj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gpjiflzdf.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gsqibmdey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/guqtdgshr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gxprnysxv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gkfwhyjjt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gmunvbqvz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gpzpuxeci.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gombvchyn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/ggvisdyvb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/givwhniuc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gbjpjgsyg.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gyjryqmta.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gprlwbyth.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gyrnlmvsn.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gthikrswh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/ggnxekivw.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gkfapzzzs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/ggrturhog.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/ggzuyabho.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gqmodhlep.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gogovbsvd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gzkeygjyl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gxbzsqkuz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gamqnycvb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ghhhopajs.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gyfptkxme.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gmomlvdwd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gpoorgugz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gipalnwxc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gcrtphixj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gokbcgxfb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gtghfzpiv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxiemdbqg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gycnfalwm.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gxpnsslrk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/guljkszlu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gmuifrjvl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gjozfybxf.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gxlakjstv.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gsvpsxtwz.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvnykhudj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gyrrvsawx.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gcozzyzrg.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gmcyvdedg.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/grugsouwz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gpoczdigt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gzcbyztfs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gwpeomszx.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/guddrbchk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gmdpudshi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gxqnirqxc.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gfgpmqzoo.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gfywxozem.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gfgcbtnep.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gpifshaiw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ggsidxldw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gzcfzcpqk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gejuprxaf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/guhiohwrv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gpguympuv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/ghfqjrqsq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gtetrafbj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gdavuuyhn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grsbrnwbr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gjvxlbwbw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gtgpyjwaq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gzccharjc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/grveyoggy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gzlfslnsu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gtresiakb.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/grvtwkwdj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gfyswkroh.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gwfyhjhrk.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gsdfixjbf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/ggxwgyhhh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gvboctkoj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gcmpliygi.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gptrvufye.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/goektzuwz.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gvumuqock.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gvpglovbp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gwtsqulle.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gemhqgner.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gqpkgmftr.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gyflouyrq.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/guiwizrfj.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gjwotgxvz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gkhtkhylq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gurluiqzc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gtwiavhhg.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gxqqnwkmi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gncfoulos.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gjqztfvpn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvwskjgqh.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/grwlovlgt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhtemop.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gyndqpmtr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqnvmrnah.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gmascdrel.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkzjdpsqi.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gkhkvshdf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gwlsmxfhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gbyytlinb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gghxupelb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gbfalfamy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gjksfwygr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gluxofrtx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gevlqmwum.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gtnfxxsxy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gfnvvltlu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gdlempnxa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/ghyfpihax.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gcxmzkcne.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gkoyloohx.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gvwcebbom.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gthmiyinz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/gramxwtnw.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/golxswhxr.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gymydmosf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsrhfspxo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gawlvkcmr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gvdcafohn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzegbxd.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnhfwpgcu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gnmvjkdgc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gkypykenm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gayouwdxy.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gnmhvonic.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gpxginuub.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gmhufingv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gcbwpnqbb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gphankhmn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/ghkeqihdd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gtunwthzh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gvhinvabp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gljfjiycq.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gvapifayt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gndxhbfhz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gzsxbybcd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gnxjdjkqg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gmbbtgdic.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/ghtlbzikl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gylxdcuuy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gccgdwedn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/grwykxlgv.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gczngwaua.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glmdtoecu.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gittewwhi.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gdtwzfohj.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gmrurbvyb.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gbuoximzd.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gcwofzlmb.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggqtadcgn.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/grlzbaoha.sHtML


<!-- 参考信息 -->