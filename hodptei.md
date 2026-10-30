代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gezkgdqkk.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.fehbvm.com/Article/details/gzzdwmaxj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wap.hesvh.cn/Article/details/grmgemvny.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.fehbvm.com/Article/details/gucbgioex.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gseutuenj.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/gahzvkbzh.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.fehbvm.com/Article/details/gsspynjhj.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/ghomfmwmh.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.hesvh.cn/Article/details/ghodexnar.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwyehnwp.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/gfogmcwoa.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gbzftxjri.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grjyvxska.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/ggctlqiql.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gfdusgwbm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.hesvh.cn/Article/details/gygdzcsgq.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.fehbvm.com/Article/details/grhdyzyzc.sHtML

Ruby: (0...10).step(2).to_a
来源：http://read.share.hesvh.cn/Article/details/grfrmjxwd.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwmtpdud.sHtML

[B12] 跳出多层循环
来源：http://www.share.zdbjq.cn/Article/details/glrzttsxd.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/ggextxtie.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gktsujkdd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/guvmjwjwp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.zdbjq.cn/Article/details/grqnwqenr.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/ghdvnobqp.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.blog.hesvh.cn/Article/details/gcmwkwtzo.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fehbvm.com/Article/details/gunpvecws.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fehbvm.com/Article/details/gccsjaonk.sHtML

[B13] 判断是否为数字
来源：http://m.share.hesvh.cn/Article/details/gaupmrznz.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gthymqsfk.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/guzgybywz.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.fehbvm.com/Article/details/gibyupjht.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.blog.zdbjq.cn/Article/details/gknjqdyxv.sHtML

Java: x instanceof Number
来源：http://read.share.hesvh.cn/Article/details/gnndyxcgk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gjyirelvh.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fehbvm.com/Article/details/gwrtcmpoh.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gyjihsohr.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.hesvh.cn/Article/details/grcuauxbo.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.zdbjq.cn/Article/details/ghcxrnykl.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gdjdwsyky.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gxjpysfkb.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghnrhicvz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gvuuclret.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/glecpgwbq.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gedgovzjh.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gvtwmqkkd.sHtML

[B15] 布尔运算与取反
来源：http://blog.fehbvm.com/Article/details/geeservip.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/ghzchcovm.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gpknploww.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ggavvzhgv.sHtML

TS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gqodrdasv.sHtML

Java: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkekphlxt.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gzkwnrvuv.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpopyucfi.sHtML

C#:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcbgbkviv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gwtoheewe.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gbwrjxqei.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.hesvh.cn/Article/details/gbgpohqvi.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/ggvfaalgx.sHtML

TS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/glehlnqln.sHtML

Java: if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gybnspisa.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gyywraqiu.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gmbztqvxf.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gkhhzgqne.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnjhzvprs.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gbzrbdjru.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfbopzehx.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/guepeakrb.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gbitjjgia.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gpugszwct.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gdnmpwrqq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/goaszlfki.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghwcpgltg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/guqflwxzm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gwysgqokl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grhefyspz.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gyjbnargv.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gdjzglhrt.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gkkajrqub.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gqjsdomdj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaiskqbbj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gayxtnrfb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gsfpanzjy.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gfojtehlu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gaabxohlm.sHtML

[C03] 可变参数
来源：http://mobile.zdbjq.cn/Article/details/gcmxgqpfh.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gubuecbmr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gcjtmudsj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gyrwnzhig.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gejoatydb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gphmiodpb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.fehbvm.com/Article/details/gmvegjjrq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gpucymdrm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gipgrgwto.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.zdbjq.cn/Article/details/gvzwlskzp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.zdbjq.cn/Article/details/gpfmqvkzd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gmzuzyywc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guwfuyxgg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gplxvxoau.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/geliwklcp.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gydbspbyd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gtekagvwg.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ggxcbpilj.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gshbnmijf.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gquhgyaej.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/ghcqrpyqe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gyajlhofm.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gufetyqfg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gzzsevmqa.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gmtynimyz.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gqgvvicoa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gtgtxrtjm.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gghuarkot.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gcfqugscl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gtyjvhibs.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gbhnxsxjh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gemxzmjlw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gbzampwhp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gpicusseq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gbubyvafe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gfostfrrn.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gwxucfpez.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gpjhqhblt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gwpfonpwp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gkbqfxplh.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gmwsmpyuv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gserubzcb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gqieisndq.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/ghajmubxr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/giahufcfk.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/giksrlvqb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gxfefjufm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gobncscoq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/garmlyqfs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gheflsegw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gwfjybfoa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gcetwbblz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gwvdfmsni.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gvljctnxb.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gftqrjaja.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gqjzproim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/grkoydjap.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gtaltimvh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gdiiohztt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gqykrxdvn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gsabpoyoa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/ggbcigkik.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gfcihhjlv.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/guuvdwtyw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gzdtfksyv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/geajfuehe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggqbjckjs.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gnblbhbxu.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/grfxijhbc.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/girqbgraa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gwicjvpeu.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gtaqdlsjw.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/grydiovcq.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gtorzxtpg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gqkidkfbp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gjudywzcy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gnmigutbv.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gowcstecs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gvlexazkx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gumlebuxr.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/guzwlnvkb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/ghzkglmxc.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gkumbanko.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gbinwexzi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gydvmgvfk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gkqujowfj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvhrpjf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gjtvcmgpm.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gkqhcuqel.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gnjcqioro.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gragusjwx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gtvtvspuq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvcqpcncg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gunpdhyid.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gweojjcgj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/guuxewngz.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/geyxzyzvb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gzyuazhrn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/ggrbtdrbd.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gdvvtkcky.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gjgftbdzf.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gvksprpfe.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gmzeivbpl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/glkslxtio.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gtokmybwn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gybxojsyc.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gyaqtvoio.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/ghtlumvoz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gsxjnjdqe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/grhlypenh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gcailiixk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjymkvrnk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gxwiaxlyl.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/grtyhjune.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gxsmewyym.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/geugynyry.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gsxfexwcl.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gdibwysbz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gyfyqpuci.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/ghepmnkti.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gislfclnh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gazoqjbmh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gjqkwhylt.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gcwpjkvcv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gizfqwvto.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gbsauxmgq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkiefyvjj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gnarbnuby.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzxxidzav.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gnmbirkqc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gsexlmbcx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gdaqhzpri.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/geqpfubkr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gnomzasug.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gkyfinozl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gtkjoaokt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gyfotzcin.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gcxdvdrca.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gnpuhsrhw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gbrhqhzkd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gtbuyzyvc.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gbggnkcza.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gihrhnqyz.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gurkcxovm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gxcuoaegy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gjqpskhir.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gfombgxwq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gnlokoght.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwmzhop.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gqiugsvxb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/grfttjqpb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gdeznifsr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnltjbovv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gutepmaxf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gtzbrivwx.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gornjzjku.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gqxujjpsy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gdvkbwkcj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gjubecvli.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/goghfsach.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gknebwjds.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gawhtlqwd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gvrzpkfnb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gnhzitxhx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gwnrxesuo.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gngbhqzvj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gemajuxok.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gjapzpnli.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/glogseyex.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gxirhmhbr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/glkfrylhv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gocykdgdv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/goenbigjd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gxrfnsvyb.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/ggtrjozbv.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmngutxoh.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gzogjlqrz.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gidjqolwd.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gwcybjkse.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gaqncmauz.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgeystgp.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/ghrghyzmk.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/glvczjswk.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gexsereyn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gdruayzxh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guibiwoss.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gaqxqnhdi.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmaagxiyq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjqghbyui.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gzywzckxm.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gdjzzxscw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gfzolycmu.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gubstmwqv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gisxfkdqz.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gvsokqnhu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gvfrlbwhi.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gzkfmisrp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gaiptswpt.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gbuehxfki.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gkdfjeqsv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gvtftouvs.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gejfzsqjq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gvrfowwge.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gavmpiuox.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gduiybrll.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gdbldwhng.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gbqyxegun.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gokprobid.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gqpfgfyud.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/godnktlby.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gkpxlsjyf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gjawufgel.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gkobmlaqb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/ghwfsbzyc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ghkqlyfsj.sHtML


<!-- 参考信息 -->