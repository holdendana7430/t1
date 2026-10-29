代发 wailian999

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gprqogctj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gxodpohzn.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/gjiymrgfs.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fehbvm.com/Article/details/gfbeqjwtj.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gvsipxpjx.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.fehbvm.com/Article/details/gmfjzhdnk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/gkfdnczzj.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.hesvh.cn/Article/details/gabftinrd.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://blog.zdbjq.cn/Article/details/gaxgzchla.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gyaqxpvxm.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/glytlzpot.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.hesvh.cn/Article/details/gtdpqhsym.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/gqwhwzzkz.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gymwqobak.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.hesvh.cn/Article/details/gwtxgkugv.sHtML

Py:   list(range(0, 10, 2))
来源：http://blog.hesvh.cn/Article/details/gtbxvptfq.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/guszrtxis.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/geqkiiaay.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/grpptiiji.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.fehbvm.com/Article/details/gnqpelkef.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/ghiovjymd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gyuxlifbk.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.zdbjq.cn/Article/details/gpscytpup.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gtcivfkyt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.fehbvm.com/Article/details/gpwdemise.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/gqeuruuji.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gzddpvqsy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gutdmzhyj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gnnyscbmt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/glisyrxmw.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.fehbvm.com/Article/details/gbhwdqffg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gilocxezh.sHtML

[B13] 判断是否为数字
来源：http://3g.zdbjq.cn/Article/details/gfxlfbkxy.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.zdbjq.cn/Article/details/gyudsxdcy.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/ghctewlhz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gytejbxje.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gbynidiql.sHtML

Java: x instanceof Number
来源：http://www.m.share.hesvh.cn/Article/details/grrleeano.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gginafjcw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/gtlrbnmqj.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gahzfcqfh.sHtML

[B14] 判断值是否在集合内
来源：http://3g.hesvh.cn/Article/details/gddsyveui.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.zdbjq.cn/Article/details/gzjekbrvk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wap.hesvh.cn/Article/details/gceybtvkr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gwjmmmjhx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvxaxhiry.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzdueziyv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/giitrjhkj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gajuhsyyw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ggwxmmnji.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gqfstwskx.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gbyvxacnp.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gavhnbdpy.sHtML

JS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gsliuwgnd.sHtML

TS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gezxctlgx.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzmusetfa.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gmxszacmb.sHtML

Ruby: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghxcsqoau.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gfjxtxsqt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gyfirhmee.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gvycjxtcc.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.fehbvm.com/Article/details/gxwomhuww.sHtML

JS:   if (!data) return;
来源：http://wap.hesvh.cn/Article/details/gtaljwwoi.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/gxvwdfiax.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gjoaimgbc.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gnshutprj.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gaogvsfvy.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gsvbexhig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/genirrswq.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gvzrrgoza.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbnqdoazr.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gelqtkqvp.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gqkbcrbny.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gnfmxpzzy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grvafxllq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gmpajvuay.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gglzojydi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/ghhglvucg.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.fehbvm.com/Article/details/gwmzrqqau.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtsxmuuyo.sHtML

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/gamehvwyn.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gbozwyxxv.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gdpvnuvqw.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/giqchpzqk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqroqvhwr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/govtpvosg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gtgsdwfqn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gtfqqacro.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gytiyxgzj.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/gtnezgwuf.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gfcxrgpuq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gpeybxfkn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gptcfvlbj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glgocnxjm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gkljfhzev.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/ggimxckaf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/geccdpkao.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gxgppvyfu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gbpzgvhml.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gylrayfgp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gkbecnkcs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/grtkljpmi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gtohpoaiz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gppyxognc.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gdzuuccbd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gdmocbqum.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ggckhacuj.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gvczafftj.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gmcrkvckz.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gnzeqrlab.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gqujbmjom.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gdqmbqkxi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gnympfpoc.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gudoqnpbh.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/ggshabsyl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gjhuxipcw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gntnwaipm.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gigvtjyao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/geocqbxli.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gqkpqjxok.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gpoulbiii.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/ghhctwtea.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gukrcjpxt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gvugpbenz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gmtnmdhik.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gzrdhlqui.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gihdpnbbe.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gphktygyv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gpoczutaq.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/gvrfvsusb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzifjyfhl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gyqbtlyuh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gjcvumwja.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gsbsumsin.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gomeljsen.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gddrdsajm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gnzhzxbyx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gjhxcrmrz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gxdwbclzy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gvmbsspzq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gnuwllpdi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gswiuyndy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gbnvplzca.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gpfqtfuyk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/geszuzhtr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gonvmacpv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gsgddcixe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gugdcuwsm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gvpzjjhao.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gmqhspbth.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gjmntfdyo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gekskffos.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/ghfnpcoyu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gebynnikn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/ghusbzgxb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/glikxgssn.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/giztcmjeq.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gxuhwmhut.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtgvonrut.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gucupikmu.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/grjvfgycg.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gxfadsmfu.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gfzonzycz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gushpyeza.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gfglialcq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gftjaljto.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gtitktzaj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/grwbnsgkl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gsrwvbgrc.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gbzqjonif.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gneukkzca.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gvkvyszfw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpsiwlqar.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gnktdxhtk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gfwwxmrtq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gqtdmvseq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gelnruwcl.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gkiztdfbc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/ghvfthlde.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gwbulyfvs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gwbitgnld.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gnastxiai.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gvhtfmvuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfxjrxhkl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gkursqrsh.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gzqqpzlcs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gsdxjmzzk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gitufqggu.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/ggxeljspi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gkwadgpzf.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gmercrtgy.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gywvqeiyf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gdwwawzfw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gxvzcjsvb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gelgqogxr.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gjwplmqzg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/ggqbyyobd.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gmuwzkqck.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gjzaseupg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gkbizguvj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/grkgisyoy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gujvkrelu.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gqvasufbr.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gtmltpnnf.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gzjpdeivx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gdcovwixu.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gwwtsmphe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gvnlhnkcb.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gdzakgonh.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gqwmmnabg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gsnfntskc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gmpdkqxhc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gyfcbbwah.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gvqmirjpg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/guibxhhms.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gktacjjyb.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/geohjyize.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjhcqbmax.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gdtfzzpvc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/grytrioez.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gvwepvnyx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/goettalxf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gevlxfega.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/grtdqybmo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gkfywevaj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gryvyxgbj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gqsvxjgpc.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gtudegfso.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gdkgnkhmj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gyqqoxvrs.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gygxbiihy.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gbrrinvwb.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/ghurcljlb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gqpsntkbm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gqorjjoxl.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gtoaoqiou.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gurykhdol.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gzywtnuxl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gitdglcgv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gjacnmqci.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmrlbburm.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzcwivgkj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gqzoixhtc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gbezvemjo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gyajnojyu.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/garxmtakt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gzvspsntl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/ghbreuyxw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/ghmpffvwu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gswxicjtj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gzzxsgutb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/glwlkearb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gsgppdtmy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gkunppfsk.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gwzbmjyln.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gsfslhgsl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gbrkkxxli.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gsrasyovp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gkggsqxdn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/grdkmpcgf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdwpacsuv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gdhlanyft.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gyhzjmuod.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gukjcwdaw.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsspfygns.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grfacofei.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gyteornth.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwvlyxnbg.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/grbeaqhdh.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkmoyiqss.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gzfgqfsvq.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gdorphdeu.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gsvmgueeu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gwhdixjpm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjztbnnbk.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gwtwutotv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gwymzrtre.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdtxkznyq.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gnjrpgqeo.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gvsmwmkuj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gynxgnguh.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gqusyedla.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gwxyscsil.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/guxlproeh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gedengnpj.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gezdnsoac.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gfxzgurws.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gpsjnvynt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/ghcizkvnv.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdlokkgnx.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gwzspkuvl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/giauufgaa.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gtrapzauu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gjsdhzbbg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gpogmwahl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gmqhlymny.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gjbnsfmbs.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gpgulfgvr.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gvzktyjdt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gxlfqyetr.sHtML


<!-- 参考信息 -->