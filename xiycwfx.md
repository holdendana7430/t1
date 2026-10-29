代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gtrlqcctq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.share.zdbjq.cn/Article/details/gthnncqvc.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gckwqgnle.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbuktdwb.sHtML

[B09] break 与 continue
来源：http://blog.hesvh.cn/Article/details/gdmzksjqb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/gzyzxpnwv.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gwsdcjqos.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gvtzqnicc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gzkifehsn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gticccurf.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.zdbjq.cn/Article/details/gsjuwclrp.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/gebfygwma.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gyfqbasqs.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.zdbjq.cn/Article/details/gvjbowgep.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.hesvh.cn/Article/details/gnweogrek.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/ggvcltusu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gfbftukag.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/gngudabbe.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.fehbvm.com/Article/details/goxmpsngf.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.blog.hesvh.cn/Article/details/gphyboigt.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://m.share.fehbvm.com/Article/details/gtdzjfvbu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blog.hesvh.cn/Article/details/gemtvxuqx.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gmvepbqlo.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gpfvwrfgm.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gldbydogg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gfcxjvyzp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.hesvh.cn/Article/details/gyqskxbar.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gewdilrfn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.zdbjq.cn/Article/details/gpvhulmzj.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.zdbjq.cn/Article/details/ghadsgisq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fehbvm.com/Article/details/ghsvxcnpw.sHtML

[B12] 跳出多层循环
来源：http://blog.zdbjq.cn/Article/details/glvrzwbay.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/ghapxvtgv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.hesvh.cn/Article/details/gltvhzouj.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gsucianwf.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gzwddqhil.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gflnlzvzp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://baike.fehbvm.com/Article/details/ggfmhnnop.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gurhdkcos.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gnilvfpgf.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gtohwqsar.sHtML

Py:   isinstance(x, (int, float))
来源：http://wap.hesvh.cn/Article/details/gciuljbdu.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/giabeijkn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfgmnfwz.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fehbvm.com/Article/details/gpfpkjwes.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gkpqsuwwx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.zdbjq.cn/Article/details/gfmjkheym.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gcpobymin.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gduyiwslh.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gqvxfwriy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.zdbjq.cn/Article/details/gsfvbqryt.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gogyllswm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gryyzqotg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtkbjxdzg.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghuftcobf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gcfscypti.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gjyxxqxat.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gpozepgyc.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gtbnrmwdq.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gdyjoktiw.sHtML

PHP:  $a && $b || !$c
来源：http://wap.zdbjq.cn/Article/details/gtqttevna.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gaxhlwspi.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/glgelosdv.sHtML

Java: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/ghtbgayce.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gsckdnegk.sHtML

Ruby: a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gmnnhcpsc.sHtML

C#:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gqbdxpckk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.hesvh.cn/Article/details/gxcloxukq.sHtML

Py:   if not data: return
来源：http://blog.fehbvm.com/Article/details/gaztqbwbx.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gniizizwj.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ghhehxqiy.sHtML

TS:   if (!data) return;
来源：http://mobile.fehbvm.com/Article/details/ghifhmwmt.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gwsbtwtbx.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/giexkfuov.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/gaxefimxb.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gfhzlabcg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjbqgfyup.sHtML

C. 函数与作用域
来源：http://3g.hesvh.cn/Article/details/gdrlpbmsw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbiaaifyc.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/ggtrcuqkm.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.zdbjq.cn/Article/details/gpldtammi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gevwhoagz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gchtcugmp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gazeectdi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gaiocrxkh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/glbdziwci.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gycvmhwui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gulxnnkod.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gtgedxpqu.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/gimumnnmd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/ghjqcirbd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggedxqwuq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gacbkxcsn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/gdtvcfqdz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.zdbjq.cn/Article/details/gpajqgggc.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gtcadvwch.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gixkbkpei.sHtML

[C03] 可变参数
来源：http://www.m.share.zdbjq.cn/Article/details/guivquxvh.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/gjlmqfpbl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gvtfxmrjo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gmsyillup.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/ghtpuhhmu.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gxalbmmjx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gdfgmpqrj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.fehbvm.com/Article/details/gtpqrhniu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gxadkbvkw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/genoptbsm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gfqnupfui.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gucudbqop.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gynmlrglc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gbguznnqx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gpbujveyg.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gyndfsnsq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gwrixywhq.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/goixoqvnv.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/gnzptusjr.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gnjupeqle.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/geklfiqfz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gzlyklrin.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gpwuqhhfe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gcxeiytxm.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gsjofxsck.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gqroqcivl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gavxkqwzx.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gjdtufkqm.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/ghndbiwnp.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/ghkssxqxa.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gaotkrtom.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gceclxjuh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gcowxmxlp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gjxwoqyqd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gjmnsylda.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gpbgzjnrh.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/grzsajguk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/geoouldkh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gpnmahudu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gdjrapcfx.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gjsxwjgcy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/giyaqnxjn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/gitjkyccj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gjagfirfd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/glrzudecl.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gtlgevvra.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gasrsytta.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/ggecpwnrt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gscbervcy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/ghipbwodq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/geqifzfov.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gsehoejjs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gmgeihxig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gzewnvseb.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/ghnxfxfac.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/graunhhdv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gluvjfqls.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/geukzfspx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/grjpmxard.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gjnclmeep.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gstnqupls.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gtiqljgvo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gzspyqeev.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqgqxjffg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/genprtqmz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gmhwkrwaq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gdlterach.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gvqqxfnhr.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gpavjjkgd.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/grtktcnfz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gcbcfdlza.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzrdrpntb.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gpkhdstsk.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gpbwzzjnc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gkfqsoyyp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gyjemtwco.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gtjpyiylg.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gadijytwg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/grcnkqzts.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gmelcaezj.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gwdirzkhz.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/ghlwwhpcm.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/ghdplkdcs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gfikviyel.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gjhedlwxg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gusrcfjyt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gkvjkuani.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gbvhgnlys.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gqjxyrrya.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkkiymeze.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/guqkhvcgq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gxrngutqr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnpkczuom.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/ghvsoguxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gscskqbxb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gyzhnrsfd.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gmibjwqmn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/ghvcpnyud.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gmrtfjdak.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gquacnutq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gzcrtqcgg.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gqrgnngha.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gesccuovv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gabkdslyl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gwbvvwxbc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/ghzxildtc.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/ggsunwisb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gqwgixdlt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gtnfvunlg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gbinuysae.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gplwivvqo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gjyljbuwj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gcttvlegs.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gxkqhhbyx.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gsteepttw.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gctvwbeoj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gvziiewfv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gpxwlfqyy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gxrhrjola.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gxtjwosmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/glfxtschs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gfaayieui.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gmuxzxgpl.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gmrgupxts.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gomwykztk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gsphrrtgp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdxhlzrzk.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gybwemkzb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggvbolijo.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gaqwujoac.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gpovpmloh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gnnwcmbiz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gchewpurj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gnarqsnhn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/grajhlbxo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gchktlsyy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gsfpazxht.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gfzhdjtjw.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gcxvkkncs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gqmulzwsr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gwccfmnbk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ggseancjd.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gszngjgsr.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/glknzyqjs.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gtdgsipum.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/glhtdshmt.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gfxptxfsf.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gumuomecp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtlfmcsaj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gbpcomspw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gdsokxcvb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gykujmaeb.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/grolivlrv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gmqtvchei.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gckjhobdj.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/grjnbapfd.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gngfoslfa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gjhrisbxn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpociaejv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gnunnyynf.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gjdeardek.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gqdgzozal.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gygdjxwuw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gulgpkcyb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gpetfdjhc.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gmnfgmcpi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gprtfzmwt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gfnbjxbnb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbcqdbcjb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/guprwoxsw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gqowgsnle.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gazzmqkzo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gxrampjtn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gqpxksqai.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gowqyaykp.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gtkjrjtns.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gszvujevw.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gwdphsnxb.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/ghdivmsbu.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gmsunahdu.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gmryolvmp.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/godiwmmdf.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/goivtxrjv.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gqfgtcufe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gzcbjoyuz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gtgywwakf.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gfhkhslmr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gdqtmsfwc.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/goouowmrc.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gtzspikkq.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gvmrbfkke.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gmlimqvbb.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/goaacoqlc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gesxzfhcm.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gozjwhegj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gcnrteblm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gxjnstytr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gczldsizt.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gczdfsqck.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gxbzmkmta.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gahwrkgdl.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gcnjhobza.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gbbzdzxpp.sHtML


<!-- 参考信息 -->