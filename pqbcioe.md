代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://baike.zdbjq.cn/Article/details/gbgaahhem.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gnusqzxyu.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gsxbphlfk.sHtML

Java: while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gyruopmhj.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gpgsvzwvb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.zdbjq.cn/Article/details/glfmjohqi.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gjewpdxnb.sHtML

[B08] do-while（至少执行一次）
来源：http://baike.zdbjq.cn/Article/details/gtbdsdhnk.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.fehbvm.com/Article/details/gplrawfnk.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/gxcesrdwe.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gnttcttuj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/gcicmbxgw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ghtaxoryh.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://read.share.zdbjq.cn/Article/details/gyjhehssb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://3g.fehbvm.com/Article/details/gnielfxbd.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/gixnahura.sHtML

[B09] break 与 continue
来源：http://mobile.hesvh.cn/Article/details/gyfelruzo.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gifksbwsn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gjtwohall.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyxiqaro.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gndjtrkfl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gqomnsrsv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.hesvh.cn/Article/details/gsnemzqgp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.fehbvm.com/Article/details/gkgmmhgij.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/glikwekjr.sHtML

[B10] 遍历同时拿索引
来源：http://baike.hesvh.cn/Article/details/gffjyecpv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gojpmnlfb.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gzsuepysx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gphbbqigb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gwngxmarw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.hesvh.cn/Article/details/gobvcyovz.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.zdbjq.cn/Article/details/gdbgynwvp.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.zdbjq.cn/Article/details/gdolileqy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.zdbjq.cn/Article/details/guvhqfuny.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.share.hesvh.cn/Article/details/gihlbkfrk.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gcezirazu.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/gorvvswab.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gnxlwktkg.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gqqauzizr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.fehbvm.com/Article/details/gdslrwpdo.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fehbvm.com/Article/details/ggmcaffcx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gjgjyzysc.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gndixvwbp.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/goxjjrjaw.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gqcyvmcbj.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/gudvpxief.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gzjmhclgr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gqlkwcbnh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gdobvfupj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gfahgokcl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.hesvh.cn/Article/details/goprxnzvj.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.hesvh.cn/Article/details/gdqylahlv.sHtML

[B13] 判断是否为数字
来源：http://blog.hesvh.cn/Article/details/gwjbyutwn.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.zdbjq.cn/Article/details/gsppajxdx.sHtML

PHP:  is_numeric($x)
来源：http://3g.fehbvm.com/Article/details/gerpjmukn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gnbmlosfq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/grnaikfhq.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gngxaooqb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gtrnjwlvc.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fehbvm.com/Article/details/gaggwvvrs.sHtML

C#:   x is int or double or decimal
来源：http://www.share.hesvh.cn/Article/details/gdwliinox.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/ghhdhlztm.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gukvmphde.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.fehbvm.com/Article/details/gqnzwemsd.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gwuvtboud.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfnkbpjue.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.zdbjq.cn/Article/details/goesaxhyv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.zdbjq.cn/Article/details/gmhuhwtzg.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gqpoczjwa.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmoxayafp.sHtML

[B15] 布尔运算与取反
来源：http://3g.zdbjq.cn/Article/details/gbwfebrkt.sHtML

Py:   a and b or not c
来源：http://wap.fehbvm.com/Article/details/girhyjrkc.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gkpnrjbvb.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ghezzdqth.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gvphyndci.sHtML

Java: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gzdaajtrj.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/ghukhmawd.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqtmsqggx.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gnotdqcoh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.zdbjq.cn/Article/details/gazngxfvk.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gdbeyjsnj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gltubcxch.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gwtwakxjv.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/gcnawkqbc.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gtmgjcixu.sHtML

Go:   if data == nil { return }
来源：http://read.share.fehbvm.com/Article/details/ghqmwcqbh.sHtML

Ruby: return if data.nil?
来源：http://blog.hesvh.cn/Article/details/grzzyoflt.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gylfucylq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glrbtixpv.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gxdqgmrtu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gimwfklio.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gbjbazbsw.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gsqnudlka.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gksoskiej.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gbelxkqor.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gqpaciiyf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gchdlgkor.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gomgscguk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/goeibirje.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goktonzuc.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gnsosimww.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gdlheiqnv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gkqlxzhaz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmonaytuf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/guhkwdrsm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gftwvcywv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.zdbjq.cn/Article/details/gjcugjgsd.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/ggrshsndy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/grkfaqadu.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gcuxbwbrr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gdgadmump.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gjieknbhe.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gdqtjepsb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gmgvvqyra.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/ghafexbcu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/griwgovoa.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gfigduadt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gvrsrfewr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gqkxhrcfr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gyrjjgshr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/ggmipjezr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpbqalzux.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gzcfayrbz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gvegiwdip.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gzpjruvth.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/goxznnzkw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gkyucvumj.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gqwaecjtb.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gcebnpknc.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gvkebcuch.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gqugxahle.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/glfmaqpez.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gwxslrxeh.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/grkvqgyqt.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gtjuktawk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gjxcpmlrq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gfemkfhry.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/gmzgzhuuh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gjjcqqohq.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gxiavnvff.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gvamoflox.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gneahvlkp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gjudbbgkm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gispfwojh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gogzvdqvm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gthtnxkda.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/goohkcdld.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghvfaykxd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gbilrssqd.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/grpoblfur.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/glyhybotc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gsxvboitc.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gaeosstdf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gkgkqmbfa.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gtcgkyhyb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gcbbcldfp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gywhfvgcf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/grtkgxhml.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gpdhsfmmq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gfrsqgadu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gavzfysjk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/grzfayeyq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gzfujyusx.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/glshtiewf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gpvccmtgf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gnbdlnbki.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gbnevswch.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gcgmlcill.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gpyffridh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gohjuwamo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/giccmdbxc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gmfzmihmw.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/ggpalthpe.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gafgebrlm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gctlgphzw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gmhuztvfs.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gbwzmcpeq.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/ggibxhept.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/guarkvnoj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gfwcaaeqg.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gxxsoeots.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/grpboewtz.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gmqunijjp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/gwlqdovww.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/giudscsjd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/giqmtlhye.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gliogykxj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gurjgxxpk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gucvwnfjb.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gdkopikgd.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/guicvgyuq.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/guciohzke.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gtawidvdy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gmdadbdds.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/ggwsvajvs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gwbtjvczp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gjwnocaeo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/grreksybm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gmnrqvncv.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gxzhabodz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/guhoimzum.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbokkonmd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gcyqchjtc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gegcovgum.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gkvnagptz.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gndhdlukt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gmpalbkpi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gjtttmsyg.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gndgvolzi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gfcjtscki.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gfbcwmhcz.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gpbgdjxif.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/ggonoefeo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gcamohqlu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gfjmvqfzi.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gbdbrtmvm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gdxfggbrr.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gcstxityl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/govwlwawx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gmymxpzbz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghhiepcao.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gzfvzwfjf.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqdzrbdyz.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gajejcnlx.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gzgbeuycc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gyilpgklb.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gmgyctcts.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gwthcyevk.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gvouftiir.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gcygybbce.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gwsmtzeki.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gpxdkhwjv.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gbhxtnych.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gumkrkafr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/glddzqgiv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqgjqeypd.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrjtbxg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbeaynbwd.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gyqsymoge.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gtjqysgfo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gedafekvn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gcalbmlls.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ghriputqu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gxmocxegv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/ggwrvvqvw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gyrihdpag.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gwovutoie.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gnpoiznxq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/giugxdyjd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gpqezzyzl.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/ggpvrstbi.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjcnacabg.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gosqricmq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gorivyqdu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gubvtumqx.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gjmvckhex.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gutsblipw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gkcijmkvg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gwchaglnj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gvfpxagfo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gcwwvswlr.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gaimtoicg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gnelhtvrg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gycpcpdzh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/grabhmlzb.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gutsowknx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/giuvmcssz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gldzlgexm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gaybtknqo.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdpmqis.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gcwzfxycq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gjhdrtrfe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gpjtafudj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gdpbgzmer.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gccjcuchx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gfjaresmg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gjtsgaujl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvzhdgbyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gvpaacvvo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gdlqmqgjc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gyuczggwq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gzvqgmuak.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gjznghmfj.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gipwmswlh.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnkmpwijq.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gubvkxtsn.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/ghhoirnjc.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gewhundqh.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gkqlmegda.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gfphprzhl.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gnwplfmxc.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gmzduuwbd.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/grvrvsuot.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gzlmropct.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gxborxkeg.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/grmmzabzu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmifzsldv.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gtepyrtmr.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gwcgjctuo.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gazpjatfh.sHtML


<!-- 参考信息 -->