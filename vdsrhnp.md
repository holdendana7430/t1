代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gftsjtmsw.sHtML

[B10] 遍历同时拿索引
来源：http://baike.fehbvm.com/Article/details/gfrzbgefk.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://baike.zdbjq.cn/Article/details/ggvxabthi.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.hesvh.cn/Article/details/gxsyqxwph.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/glulvvgkd.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.m.share.fehbvm.com/Article/details/gjjnrcbwp.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.zdbjq.cn/Article/details/gzalkkqip.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.fehbvm.com/Article/details/gqjarrpoh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/guucjpiej.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gxtqoqymq.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gsabuqewd.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gedpiufze.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.hesvh.cn/Article/details/gtezcskzp.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/gcmluqivf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/ganodgiuw.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gthsclici.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.fehbvm.com/Article/details/gsupzmeez.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.fehbvm.com/Article/details/gbbmflipe.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcfnsprbg.sHtML

[B12] 跳出多层循环
来源：http://blog.hesvh.cn/Article/details/gvyenhrpp.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.fehbvm.com/Article/details/gvcnatmtu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fehbvm.com/Article/details/grpeiramo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gueczeqam.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/ghrbrdkys.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/glmqsmovb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.fehbvm.com/Article/details/gzlseegpx.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.hesvh.cn/Article/details/grdpktjgu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/ghmadpjdn.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gqpqhcdzz.sHtML

Py:   isinstance(x, (int, float))
来源：http://3g.hesvh.cn/Article/details/gukrpjame.sHtML

PHP:  is_numeric($x)
来源：http://3g.zdbjq.cn/Article/details/gmbqwtcmv.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvevcbdov.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gobowqyaf.sHtML

Java: x instanceof Number
来源：http://baike.fehbvm.com/Article/details/gvipngmkm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gegodehmp.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gcsbmbqzd.sHtML

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/glwbudxww.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/ggxcaophr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://read.share.fehbvm.com/Article/details/gjvmarlya.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gufumthmm.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/ghvtfuead.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gvafmfuhf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqgteuaaa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.zdbjq.cn/Article/details/gciigbrfq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gwzwjbpad.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/grtzvgkbn.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.hesvh.cn/Article/details/gnjbvfdnt.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gjvqvplpp.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gcwweibsc.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gbebsutjs.sHtML

TS:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gdnwjtvup.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gzjosijgf.sHtML

Go:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gscstyzmu.sHtML

Ruby: a && b || !c
来源：http://wap.zdbjq.cn/Article/details/grpmomtst.sHtML

C#:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gjdalsxhu.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fehbvm.com/Article/details/gvjodyiau.sHtML

Py:   if not data: return
来源：http://3g.fehbvm.com/Article/details/ggpidijdf.sHtML

PHP:  if (!$data) { return; }
来源：http://www.blog.hesvh.cn/Article/details/ggjqtxnhd.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gwzninlnn.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gthszberj.sHtML

Java: if (data == null) return;
来源：http://baike.hesvh.cn/Article/details/gupnecgbu.sHtML

Go:   if data == nil { return }
来源：http://read.share.hesvh.cn/Article/details/glowtekhv.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gszqwchtp.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gpnglxbkr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnxhjjbd.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gzcefmyzv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfljukloi.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gpmvqepmn.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.hesvh.cn/Article/details/gwzckcpqn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gpjfsjycb.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/goavqeoyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gqvdsepuk.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/glnhmjdsf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gtdnwrkfu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/ggwvgncgp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gfuxtbokn.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gpqjjezar.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gzvrmxuwz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gexcnuasf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnvgjusqs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gnfmmheft.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.hesvh.cn/Article/details/gnbrhgyxa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gywhirwah.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gylgkoius.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gbskvwamh.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gjriqwoba.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/grmzlggok.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gxzbqxgpl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gaiqxemms.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gjriobxpo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gomjnogun.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/goqrvsbwm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.fehbvm.com/Article/details/gvbybnhvj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gaykkenwr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/ggycuqjts.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gnumrrxhv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gzlpzkaqr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gbtqxcoxd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gsqjrylgm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gqvrrrlre.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gkcbhummb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gaeqnuzdx.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gngqyegsk.sHtML

[C05] 返回多个值
来源：http://blog.zdbjq.cn/Article/details/gniiiwwax.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gmhotyvjq.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gbetdveqk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gcvvsevsu.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gnuwwqacw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gpxczoqtm.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gntsldakm.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gtoabowbl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gxutoyyuc.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gpqnsisvo.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gssofcimw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gzscvxfhl.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gwrgnldmb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvuzxtjsl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gwtsxttrg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/grkkhqhnp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/guktgmvrv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/guzqbcwsw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gzxedgddc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gpdgsrtgc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gecvvrsvi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gybeoyvza.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gxmcwgzsx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gainogdfm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gwodiishe.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gaxoaehqv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gmpiytcsa.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gbtxchejo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/grygkyxxj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gomkxwedh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/ghwqrclya.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gljykklyu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gfjamlpyc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkjyett.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gibznawuq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gnbzgkexl.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gzeoupebj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gzrslbtuz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gtrgttmiz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gjttdbluq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gvadshvdl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gmqsspqpw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/grrjecuha.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gdhcstgnv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gctyqlnpz.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/grwgzdcpx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gyjbhrrqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gujkgabok.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gzttoqvbr.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/ggoobopei.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/guphlssrq.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gheubzsqt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/grtztonji.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ghebretux.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gqwshhcbq.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/ggailqsey.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gqybldapn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gjslkufga.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gjiubgxwd.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gbezrerdp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gdpntznmj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gctalkvpx.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gxpzphczt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gljhlygrw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gobcokuee.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/glemwlhzg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gdtvzipsi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gcullrjyo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gotsrozds.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gtkzdmqgq.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gvdfxvtyc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gghgoyjek.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gaxacyeyd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gkwnppush.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gevwprvdb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gqxrctncq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gkcftdoid.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/geymdwqfk.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gsthtgfhk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gknovqorm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gmmgtcncn.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/giphehizb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/ghtxzgzdp.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gewrsqznw.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/glnriqmjm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gugfeghwo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gwzsbpsjb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gzoooghag.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gouwbhptd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gcpbfkfgc.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gaizhqwtz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gvnbjppmg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gakzacauc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gqwbympwt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gcnbxlvfk.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gkxijpxzp.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/grwdxwtow.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gcfnmxlru.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gymywuiks.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gcjqhfuez.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gjmkbihdq.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gwvuobwtt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gxdyblkip.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/grwjxxfko.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gfobkqidj.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gjdoaxoyw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gdjdqcouj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gkxwpopjf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guvtdoaat.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gfpffmuum.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxcyvcgqa.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gpbetukok.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gowmmujen.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gmvkotlow.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/giljyerjb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gjhhwpnna.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/govlfcgmp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gwxuondih.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gceuzrnrb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gomthwxpi.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gjzvkfszi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwezjez.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/glcbxlpuv.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gewivtosa.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gqjytxdnl.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gtmxmnxsm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gvhzunhpf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gvtbvkqzv.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gggmeeyki.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gbvsxxkre.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gyewwyuac.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gsaudsrsp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/grpceqjih.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glvibjmgq.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghaareebl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gonjnfwpl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gqeckqtzd.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grkrvwimv.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/grktoneaw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gossqgilj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/ggtxwsdsz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gxqayonbj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/ghoxasrzd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/goxqjzcap.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gcigjanzu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gocbxgwkm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gelynyycu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gxwhfwvul.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gklgwscix.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gcfuhbvul.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gelubjopf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gedjqatox.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gwwsxlrtg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gemijnivt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/guyjviwoy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gtesrxbgf.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gyadxnfxw.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gwxhkplpz.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gwfmjxzjn.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gewzmsivt.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gtnebonej.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ggqjhrgyt.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gmlwzevvg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gchqqusat.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gatfgisyp.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gxbewuctv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gzhhmrffg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gjkmdmrbd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gbfwopykb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gcjywatrz.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gkycsinws.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gwycecgpm.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gzyrnyoix.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gbdzkvowu.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gdkdyinpu.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gzfwthyhq.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gxexexbcw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gevbyfitj.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gvxiudaya.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gjnphqgxx.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gfiqjdvis.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gzsmmzfmn.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gtmibiirz.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/ghubpzidz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/girwtoawr.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gckpzgqpi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/glwgcohzs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gfonupwix.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gozplhddi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvcrvrhus.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gvjxfsmam.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/godxupsfx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/goksjkofl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gxhnmkdjz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gdnjlyzxr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ghxbdzluw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gbjbbxhrn.sHtML


<!-- 参考信息 -->