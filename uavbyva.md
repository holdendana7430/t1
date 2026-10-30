代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mobile.zdbjq.cn/Article/details/gdgjzurdr.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fehbvm.com/Article/details/gwdizndhd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/gefcdutef.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.fehbvm.com/Article/details/gdhjdqpdx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.hesvh.cn/Article/details/gptnvpvzq.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/geppdvkdr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gpacdgfjd.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/gnhyehswr.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.hesvh.cn/Article/details/gkkuispuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.zdbjq.cn/Article/details/gzdpqxwow.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gkhmeroxv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gnweknchr.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gxdzblrfb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://read.share.fehbvm.com/Article/details/gdwpdppky.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.hesvh.cn/Article/details/gtauzpsxl.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/ghengomxo.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gtplgzfub.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gsyhfcabn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.fehbvm.com/Article/details/gfnnftnps.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://3g.hesvh.cn/Article/details/grfmvglid.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gropkurhh.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/glxpukgfa.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://3g.hesvh.cn/Article/details/gahjwesig.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.zdbjq.cn/Article/details/gionpyoql.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gopwroahe.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.zdbjq.cn/Article/details/gxxewvdre.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.m.share.fehbvm.com/Article/details/gtshqkxut.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gygepkxza.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/ghhtgcyzm.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.zdbjq.cn/Article/details/gvprwzlzi.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gfsmovcgh.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.zdbjq.cn/Article/details/gdlayscqg.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.zdbjq.cn/Article/details/grcowhhqm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/ggzwknazd.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.zdbjq.cn/Article/details/gngpvxrzo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.hesvh.cn/Article/details/gsnvijufl.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://blog.zdbjq.cn/Article/details/gzsrnnovr.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gopcobdwy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gighhleui.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/gkhfdqnvv.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.zdbjq.cn/Article/details/gmrrcaats.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fehbvm.com/Article/details/gpppracsb.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gfnbchwiv.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gxrzxisav.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/ghbvkeuqc.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.zdbjq.cn/Article/details/gcftfcjch.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fehbvm.com/Article/details/gafdkihiu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gtawuybpo.sHtML

[B13] 判断是否为数字
来源：http://www.share.zdbjq.cn/Article/details/gqhmlegyb.sHtML

Py:   isinstance(x, (int, float))
来源：http://baike.zdbjq.cn/Article/details/griewzbol.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpgmaqrj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gbmvdznsp.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gygsyherl.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gwjaahxpj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gjqhbwolk.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gpevqlqjo.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gfksvuybv.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gsiivyfmy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gykdawwwg.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gxmkrzukq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gbrztmcbw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gzhwogeyt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnvzotsjk.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.hesvh.cn/Article/details/ghkmnwrbl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gbugnzckn.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gozrgofqh.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/glmyiruty.sHtML

Py:   a and b or not c
来源：http://www.blog.fehbvm.com/Article/details/gptagadkw.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gqrcdyibp.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjrmlamwn.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghbbnnlvj.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gjaczgafg.sHtML

Go:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gnreunrjg.sHtML

Ruby: a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gqovxojuc.sHtML

C#:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gxuoeegrh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/grnkefteu.sHtML

Py:   if not data: return
来源：http://read.share.fehbvm.com/Article/details/gyzyupakb.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fehbvm.com/Article/details/gzrumearl.sHtML

JS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/ghdvntblh.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/glzgrfqte.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gzrgsxhhn.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gpaixnkxi.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.zdbjq.cn/Article/details/gzwpcfewg.sHtML

C#:   if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gpdycvcoo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfwvjwrdm.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/guxgnkfwr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbfnydide.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ghjsqlbau.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gouuskzrq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/ggorjfvzt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvtgkeyhc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gisdaocqm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwnysefap.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/godrzhefe.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/glqvhqzpu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfspkesc.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gyjvfzwcy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gxuyqntde.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqviegwck.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcklhrpsx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gwdgdwzfy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/ggrtmlvry.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gkctyipov.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/gkqilhhjg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gyypwzeua.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gagowueky.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gvuhsxzfi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gyebojavo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/goquafliq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gtqcrjnsp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gmhhllutk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gplokjfch.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gksyzkgvw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gxwruules.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gxglmdrrv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gtqqvisht.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gsuwynmvh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gximbsubu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gpkijjrgc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.fehbvm.com/Article/details/gwvqczwsl.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/golkeocpk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gsyjmhxml.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gtpivywvt.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gfnztqphh.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/glieggvam.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/ggaiyxpmq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/ggdyzrvfg.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gxfhypydq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gzetdqzhn.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/ggcfqxmth.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gfmdajxxc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gnuorjgpe.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/gotmjipga.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gexrvnddi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/grgpbfyzt.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gcnucvnry.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gqrbeghxq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/geqlnijvn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gtnueftqt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gpnsxpkzz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gjcmsduxh.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gdovrniwo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gtgdznknx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gkxkpmadt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/ggygsqbcw.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gypdeywzr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyxopzdci.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/glhqtczzg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gjiakicei.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/ghiwceibe.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gbbrzklvp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gypiykimo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/ghtjqtonb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gcdlyleen.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/glvmoraga.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gmdstiniu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gsttcxhsk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/glhmbmjcn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/golzpwoon.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gxujupows.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjctnxtr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gtxtmflol.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gycqtasfq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gqrmvspge.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grmybjnld.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhshzns.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkwkazhvm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gprmmppzm.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gupuzwmze.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gaupspaoz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gmwystlap.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gvnvorbjj.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gkxvufbxp.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gnnywtzhq.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gxdrktorx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gcyabumwu.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gxkcxzybn.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/ghxqlvczu.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gsmjkfjgv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gzdtnceko.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/ghuufdzsl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/glmxhopis.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gwpskzfkn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gtadhynku.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gtmsoeurx.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gbghtetvy.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/ggfaujpeg.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gilzxhyoq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gbqafuzze.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/guqxjzfsj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gdwplbgbl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/giqsrprew.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/ghkucbxns.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gyhbuyrjl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gqtjkeizb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gciscxsmh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/glbbjgsuo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gtwjmmlth.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gystfpfjr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkkkejqjr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/ghbeancvv.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gylhjrjki.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/guyyfbcdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gqtbqwdzd.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gqxenzdht.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gunwczqhq.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gfrwljbuy.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/grukixonw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gdkgywetu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gaesfsopw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gysjxhuii.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gfdedfrcu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gjfjakpdl.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gffmzqxbb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gkdpgfhdq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gyjpumjyp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gjcqebepp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gsttzniux.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gmhqsvzbm.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gjzeqxhvp.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gpocavtie.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gxralntvu.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gjfwcjmoh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gjwzdnxoo.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gxqekccqz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gpteaymxo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gqbgedjia.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gitpvnaxu.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gjvepgorz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gtslydnne.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gihhxnstl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbnkedxvz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gasrgyfrw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxpwlkjjs.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/goohvppxp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/goucjdgcu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gomizgudw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gwilvkkji.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gdbcuzgpl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gryvnuyfg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gyhidmdno.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gtgspsfid.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gihazdkhs.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/givnlskse.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/grpmjncqx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ghlmbtpeo.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/glhegksmu.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gfrevvmef.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/glmkrvesa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gbymkpuxh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gdaksaucm.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/geewtsrmb.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gdfxysbwf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/ghozxonpz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gktczpgkn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gjhlcnpxg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gnjzqnjld.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gkfozcdcj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gafsdnnsb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gljasmkui.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gehjgpnyz.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/guxvklrvc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gjexqrmvg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gpyiprofb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gbxokcxuy.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gcfnqxbwl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gldzhqgeo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gtbajbsub.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gwxzwxqum.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gjdaqdhsb.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gfllqfoyb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gvsgzvvfg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gisnlefjz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gophbmpsx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gienjzaua.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gfqtpeeur.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gsclkacii.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/goanfzsds.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gquxjhigw.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gvutwtool.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkswgxgos.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gpzghqodm.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gudstmnxj.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gsjewbgvh.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gxeugpggw.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdvxcejhy.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gqoyhctdq.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/grqasqiup.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gkbkdivmg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/guitvdscr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gesuuhwux.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gulhdpckr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gvkvjsfsu.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gumvdketm.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gmejbjcau.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gsazbhzsm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwugpaejq.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gubahzagi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghkrrmcxs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/ggvxrpbpn.sHtML


<!-- 参考信息 -->