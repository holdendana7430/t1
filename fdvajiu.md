代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gcypkpjsj.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmbvtsx.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpiwoxzcp.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjmclrze.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqpgfjxp.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gwbiqjtlf.sHtML

JS:   do { i++; } while (i < 10);
来源：http://baike.fanxiaobao.xyz/Article/details/gytenwdyj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrsbwbfz.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmrpiiwl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdbateeu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvhkpjbp.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwofogsit.sHtML

[B09] break 与 continue
来源：http://baike.fanxiaobao.xyz/Article/details/glpnrmxmw.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbxsjbnz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqkavnfji.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giugllnjx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfukhgjdo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkjodnlf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjamxunf.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gvazidgte.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjydcbxqa.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fanxiaobao.xyz/Article/details/glhssxuwq.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.fanxiaobao.xyz/Article/details/guavmorvd.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxmftngm.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fanxiaobao.xyz/Article/details/gyisywphb.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.fanxiaobao.xyz/Article/details/gainpsjvp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvysktqt.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wap.fanxiaobao.xyz/Article/details/gzqilhitb.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmkiakfo.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqyugtdw.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnufysewk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuyfpeug.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfslvlrgq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfldfwcnq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgzjrdmx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggigwrzxd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqywmnmy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gsvixvutw.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtrdijjt.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpattjmb.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fanxiaobao.xyz/Article/details/gxuasjnfq.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.fanxiaobao.xyz/Article/details/gqxxzgjkk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdcpskmu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvubksqf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gnpbemmvx.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxfufcwhp.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkxqzgur.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlckmawo.sHtML

[B13] 判断是否为数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gljvbqcbe.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graogmaxn.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyneytkt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaprafbi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdizojwcc.sHtML

Java: x instanceof Number
来源：http://wap.fanxiaobao.xyz/Article/details/gtaarpmki.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fanxiaobao.xyz/Article/details/geinmhvet.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fanxiaobao.xyz/Article/details/gyvghnyih.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlgrevtj.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fanxiaobao.xyz/Article/details/gownccbnx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gzkhwncck.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fanxiaobao.xyz/Article/details/gsmbuxbwl.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnthjsrtv.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkwxrkhwo.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgsfwsow.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgkfeiez.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocoqrfjv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqxhcwnr.sHtML

[B15] 布尔运算与取反
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbbtclye.sHtML

Py:   a and b or not c
来源：http://blog.fanxiaobao.xyz/Article/details/gujhtypip.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fanxiaobao.xyz/Article/details/gafyfurnd.sHtML

JS:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/goeeuqzqc.sHtML

TS:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gzcllibll.sHtML

Java: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqezoiuoh.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gwfijvbmj.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxnrkysj.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/gyczacfqm.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.fanxiaobao.xyz/Article/details/ghgpiuldm.sHtML

Py:   if not data: return
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquhxeqyf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbzgpfpd.sHtML

JS:   if (!data) return;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtaffhka.sHtML

TS:   if (!data) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/guhtlgeml.sHtML

Java: if (data == null) return;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaexlfur.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlquubxy.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsynfpje.sHtML

C#:   if (data == null) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbapbvqw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjmjvliz.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsmxhckz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhpzguum.sHtML

[C01] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnldnxpmf.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gtxibfugq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gduwczmjq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefuxybfs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimytsdq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvhaktgk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjxuswsd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fanxiaobao.xyz/Article/details/giuhuxssp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghinikrhy.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gbkrxcyqs.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gunsjqrzq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjulicmmh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxozrhccx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqcrxqmj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqfamrle.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfdbolqi.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbzmupsp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/gpwbjrzxv.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gyzedekay.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fanxiaobao.xyz/Article/details/gifikllka.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/gigdetcvg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/grqlfadwc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gaahnlrkz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxndcve.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdjuroya.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmkpzedhy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpexuwsxh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbonguki.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofptumdh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqjyhivp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfsyntmct.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gemokviqy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gspplhlpo.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.fanxiaobao.xyz/Article/details/goodxstva.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggqzrumkn.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gijduwcjj.sHtML

[C05] 返回多个值
来源：http://baike.fanxiaobao.xyz/Article/details/gtcawjudp.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrriisdi.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdfwxxyc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gxtczfhhl.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gusqnezmf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/goaipxwrf.sHtML

Go:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gngyphpqe.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gicpaiaju.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmgytmdu.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gludrzjdo.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gcomghueu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/gyaiqmjiv.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumcummt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtotfcwyc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gmqddxruz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gknajssed.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtehmfaeo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gucsqmzxj.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdkumwbb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gpwioycrg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gdycvbqwu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxknepopn.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopraawjt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbchxqhvn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/gejkpzirt.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/giucfpjat.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgcsuhct.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gybcytcnk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzygsadl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ganxoelvl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganakmxjv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbabuqjx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnlswhib.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeigmdjo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fanxiaobao.xyz/Article/details/goburjlhv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrvgpywq.sHtML

[C09] 递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkwyeija.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjsttssu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gaoiepewy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyhjsunp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitljlutn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gllcajqbx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/gynjzowjm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghhhqsmmz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gxpjjqmvf.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcgopoph.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fanxiaobao.xyz/Article/details/gkmhznxxp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtqcygsi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gnczlfzcv.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuutgyzk.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcewfmiag.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgmrzvo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gptvodswi.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gucovafcw.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfznpsof.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuvxcquf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gbgtzlrnx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/grymogiff.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktyqfkdi.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaysobhz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwldpjgv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkiquzri.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/ggvnmysbe.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoqadlwv.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/glqofbefh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvupezmyw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/ghnrkxuyc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxexzlsht.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisbvamaf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmcahond.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcwnkmzb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwsrrghw.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gqsjnvmaq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghozwdaeq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqlulhvw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbenbgv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gloaobdmi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpymjrus.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gmicfvkty.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gztkfdywj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gsqwiqdqh.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcjwzsjh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/ggykrvmbb.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvkfsbmn.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gwzwiaqve.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmqnostw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghcnutifx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhnkeook.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gyhmezvdi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/gpbtniyco.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghidoanld.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmakfwqn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpgendpi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grqpckvxs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyeiuoslh.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gctashzju.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhtoeizw.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/gycjtlamg.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrjxpiar.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmgxwgup.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gwnpxtbmf.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvtdebqd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gemmpnflx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/gvqcypqiv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjwmkkjtl.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fanxiaobao.xyz/Article/details/gxbctujca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/gyyokaedj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glkreljzn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfougxqvq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmbaschc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grwrfswjb.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/geuykpfqp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gatkdjzcp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gimnaglhk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/glihjuenx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdydaldya.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsczbfdk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtotjoycn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfizyohk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqqdmkys.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gjinrcscz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcautbft.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gptcrhbyh.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/genidnqkx.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gkumpoafk.sHtML

Java: list.add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazidyqom.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgkebcfn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdictwii.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdestonnm.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsfleritu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpptlejsu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gfxarrsjy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtpkdflo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gjuxzlxro.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmpwnjg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gypgokgxw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gshvbudwp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gliirynei.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gwvcmsyeg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhoybgaz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjouhlvty.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gmzrfpdiu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcypphsz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gconsbgmf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwbrlxiu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/guhbjluri.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgnaoppq.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdczcpri.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gorxtdylp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnjlmpwz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gjwpnojvo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcexhamz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzdckbcf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gikhddvok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlaxnjjt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfssizvdx.sHtML

[D06] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gorghmkwg.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gepzctmfw.sHtML

PHP:  count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfjipnwy.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvsprpvg.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gablxsrdq.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/grfxudani.sHtML

Go:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzyvzvjd.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwwovwem.sHtML

C#:   list.Count;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrsgpwgv.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gslmpgzre.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrfrzuqt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcttbqfo.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gimznhfpz.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhmpwny.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieymlbno.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnfossny.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajyokbk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gioxyjove.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grclbhqrq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnaffseo.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxvrgzqt.sHtML


<!-- 参考信息 -->