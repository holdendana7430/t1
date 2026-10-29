代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.share.fehbvm.com/Article/details/gbgedkkoz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gjgxpoafg.sHtML

JS:   do { i++; } while (i < 10);
来源：http://wap.fehbvm.com/Article/details/gbsinngwi.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gqqpfxzdl.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gadlvxded.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gwupxwlsd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.fehbvm.com/Article/details/gnmhhyekv.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gfvbakxrn.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gmnfagcyi.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://baike.fehbvm.com/Article/details/goaqhrekn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gffuxzyrh.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/grwnxkzvx.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/ggqwihstt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gnfllytxt.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gkjhoffzy.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gxdqewyxi.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gpgpuglfb.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/gjpirvvzc.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mobile.hesvh.cn/Article/details/gfrctfcyw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgplpgyx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.hesvh.cn/Article/details/gkhzgsheg.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/ghnyohqlk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/grwdazhin.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.fehbvm.com/Article/details/gxnivsign.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mobile.zdbjq.cn/Article/details/gnpnnivlw.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gsefobugg.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gawcmcrrx.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.zdbjq.cn/Article/details/gkedmnojp.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/grrouaggw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gukhullas.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.zdbjq.cn/Article/details/geqkdmkvf.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.fehbvm.com/Article/details/guiclkkgy.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/ghsybkmwu.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fehbvm.com/Article/details/gaqbdycsh.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://blog.hesvh.cn/Article/details/gfcumcydn.sHtML

[B12] 跳出多层循环
来源：http://3g.hesvh.cn/Article/details/gclyopmcs.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/gidfqdyly.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/ggsdeztgi.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gnydkpvna.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gmnhpszbf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/grwxqskom.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/glffmfmcx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/grxfcails.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/glfjwragq.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gklwdaagc.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fehbvm.com/Article/details/gvxthwdkw.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpyhony.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gasqawnso.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.fehbvm.com/Article/details/giircaqpy.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/gshvisnit.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/ggieraiwj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.zdbjq.cn/Article/details/gyshaewid.sHtML

C#:   x is int or double or decimal
来源：http://mobile.hesvh.cn/Article/details/gagjoqgrl.sHtML

[B14] 判断值是否在集合内
来源：http://wap.hesvh.cn/Article/details/gdpshoqzt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gsqumujvb.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.hesvh.cn/Article/details/gguxopwbe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gpcljmbmo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbfukacnv.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/ghnxygnjd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gzlruqgrt.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghpsyaopi.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqwhavxyw.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gwgwraavq.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gfxxalvzs.sHtML

PHP:  $a && $b || !$c
来源：http://blog.zdbjq.cn/Article/details/gcpvduugn.sHtML

JS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gmsisgcuv.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gbjznscyt.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gqmemblzt.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gercyipgq.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkmyhvidl.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/ghkmoxlrq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/gabecihme.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gtstwxvty.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/gqxzsuksj.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gubbmapek.sHtML

TS:   if (!data) return;
来源：http://www.share.zdbjq.cn/Article/details/gsydcqbuo.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/ggsmutbvi.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.hesvh.cn/Article/details/gdnqqfrum.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/ghaqiqlaf.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/giajrhycn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gaghptxij.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/ghplmymxs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvyfkjdwv.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ghotawlig.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.hesvh.cn/Article/details/gcwswibxe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gltilcknt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjenguxil.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/grdsxhvot.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gwmamgvix.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/grqjfnqyt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gmaeysjlb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gxqxhtnsh.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gnpaasqzf.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gralrrpwx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gsqgteusl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/gdbljqdrd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnxiaxzgq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gehxzhoau.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gbbhwkdjm.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/ggwemxfql.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gikxhybcf.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gxqgrgkrr.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.fehbvm.com/Article/details/gvuecyulk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gffhdkcsh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/ggvljislr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gnwvittis.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/ggylppaqd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gaizjfwln.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gdpnywzhm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/glynqtmbd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gabhfkdus.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/guhlficus.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gsfvfavbt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gbiclnvot.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/ghyexyhmt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gpeoaamlz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gmfcfwvmv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gxenhkowb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gctcjzgok.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/gyfgehlnw.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gsajpgtug.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gbpfvoaer.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gibaylvoj.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gmqrnybux.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/grizuqzex.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gqpjiiopn.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/ggalllxfv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gzwwvoaih.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gpmdwyrou.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gveldwwys.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gmqufdhjo.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/giirvycdj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqbkjrhon.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.hesvh.cn/Article/details/gswnnfqqc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gqlhonurg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gjogrbmmj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvfbvbazf.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gamqqougv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/ghftxicti.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/guffekdji.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gqoyqwetu.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gwegzespw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gkripobim.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/ggikliiav.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/ggufnblse.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gyjnxseam.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gpgqavykh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/guiowuamj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gsktghcwb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gslwobhqo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gmckshsfu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gqeuoxund.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/ggmgjqupb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gfxpggglw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/glycqmfma.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/grkpmsyaa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gbtmofczk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gbdbqjdgi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gbbzahwpa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/guakcdchg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gdoolapyz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gfunbkeum.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gytqanpdz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/govrjrmyu.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gecffjsvt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gliayjypn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gcvhfklka.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gobainkla.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/grzhdseke.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gybcgaxzk.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gryzdyiro.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/ghedetdjq.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gyhgbamgc.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gyruziekc.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gfgboqmiq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/ghwhagjup.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gwclwsuzb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gpfvupihy.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gsykxwvjg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gtkuaelch.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gjrfafzjq.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gqzchvlia.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gzdxabjnb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gkmroxwtw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gigntabsb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gjkpvqeep.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gbtfgdyhg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gnxtstist.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gjblcwqku.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ghvhzmwxy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gkujkglst.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gxksgvuxn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gwzklkshl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gesorpstm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gsafrswhn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghrbjtmtl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gklrwdsea.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/ghqjwduzv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gibzostbr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gmngkvnic.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gvsnnkbkl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gjqixxgke.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gczxmfklm.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gblfqgdzo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gddfdqknu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gbmbmgjss.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/ginyebfxo.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/glammxfqx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/goludmeha.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gmpxszxau.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gmdicrbpn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gxunxqlux.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gtxhlrbbk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/glyrmpsra.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/ggcldxkcx.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gbiarknge.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gvhfmlyzg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gqpklymbe.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gazdhpcjt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gowogdxxk.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/grixmozke.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gqnyvojdj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/grjxcrmdp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gtzfxeasp.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gzruxllam.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gurrfnkny.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/goybbdmah.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsqvbfqip.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gmorvifhu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gewqbmktx.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/godpdjswa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gzvpoxqmh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gkcyufeqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gbelztqvh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gpakhaamt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gunloslke.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/guudhvqud.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/grrjdcxla.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gmmccuzoy.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gvuftupmz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gvxohouxu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/geofjkxgd.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gljjvnjmd.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ginvyfwqo.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/geklemlka.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gbbcxznkn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gjyjbqciz.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gcekcflfl.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gexfedcuo.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/ghjeigebr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/geljxiihu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gdazzrmka.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gsubvwzat.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcxdscdgd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gvinwpmzy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/grtffmiyk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtrwlhbky.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gcmwuspdf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gzrssxeku.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gymiruhvj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gaohjlmwc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gtncsyrbt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gndgiufyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gwlnycrlg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gvxfohyfk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gbyljdxox.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gmxmijmjv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gydcfhrqh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gaixmntgl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gexiivges.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gipdrcwye.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gwohqadwf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gisdwrjeq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gosgoazzx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/godlaleiv.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gvtihykpj.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gsnblxgae.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/geycbjgnx.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gihwrrcux.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gezkmjwiy.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/govadpzon.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gpqoqivqy.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/guhhzwpjc.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gerpyouft.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gdtgxaxci.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gbdwsieak.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gveynhsfw.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gbojfgauw.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/grvrmgaot.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/geujffqes.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/ggbkrsnuy.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gxiwxrgwd.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/givuvsvwz.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gocdgwrvj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gmfaajoaa.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gvrjdbobc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gudpqexyk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gkphzoker.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gsmwtkytd.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gcbedgmzv.sHtML


<!-- 参考信息 -->