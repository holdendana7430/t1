代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gjztxrwhl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.zdbjq.cn/Article/details/gviyobizz.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gypndqoba.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gjjzdnvio.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://wap.hesvh.cn/Article/details/gbcliwhzd.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.fehbvm.com/Article/details/gmiiqosrg.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.fehbvm.com/Article/details/gstvdqwlx.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gfwxsksdg.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gnpzipdyw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gttaiwoyq.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.zdbjq.cn/Article/details/gzfbzaljx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkzbsqqi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gewztdikd.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gemzbpzyi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.fehbvm.com/Article/details/gljwvpkox.sHtML

[B12] 跳出多层循环
来源：http://3g.fehbvm.com/Article/details/grfasihin.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gqmfaexnu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.fehbvm.com/Article/details/gytaezcwm.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/ghiduujoy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.hesvh.cn/Article/details/gmurgabvd.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.fehbvm.com/Article/details/gburrffzu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gvebxiswe.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/glsancqdp.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fehbvm.com/Article/details/gymtzeajz.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/giprbvbsc.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gksfpbcnb.sHtML

PHP:  is_numeric($x)
来源：http://wap.hesvh.cn/Article/details/gpulnuola.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.hesvh.cn/Article/details/gsoysabad.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/goepsefxz.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gsldvvjtj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gqepairgs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/ggahhtgda.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gusmuxqxe.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fehbvm.com/Article/details/gpuuwgikr.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.blog.fehbvm.com/Article/details/gwgqatdqp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gnvmdfpjr.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.hesvh.cn/Article/details/gswcjqjog.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gbbwpzqlx.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gylemdukr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.hesvh.cn/Article/details/gchetsslf.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/gpiipxiug.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcwzdmgxw.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/gaipankmj.sHtML

Py:   a and b or not c
来源：http://read.share.zdbjq.cn/Article/details/gklxlmzft.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gdrsghpkf.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gbntjvfqt.sHtML

TS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gcxmqbtek.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gbbjzelrt.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gbmptzjqh.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gjgcesbth.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gdtftrwng.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gcraekvvk.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/gamnvstzj.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gofdrpuow.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/grycrzhic.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gteauwjxo.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/getnlndmu.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/gdclowchw.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gxwmdtoaw.sHtML

C#:   if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gfesafvdx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giqixdnva.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gsklklrsg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqjazefsd.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/grwzwgfby.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/gvyxmqeza.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gqqhnbntd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gyszsksvu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxlughvso.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpgvgqazy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gghrqrxzl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gtvlskiob.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gewuetknn.sHtML

[C02] 默认参数
来源：http://mobile.zdbjq.cn/Article/details/gnumnxdqp.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gmgcyzeux.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gnuugnqhq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gemxlnenp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gknooalnd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gdxvssxti.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/guyinvnfw.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gpbmkaokl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gbwjzghln.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gxaydpybd.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gtrdbvetz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gfqyhymrc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/giurmviby.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gxpotgszi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grzxnwgeb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gmxvexqoz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gdksjkgcd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gnximegos.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gktgdxqho.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/grooaofou.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gjzqszpwj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/glfphxdsk.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gquewvnwa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/ghdjotsas.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gyvqoafnc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkxduqpdq.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/guainhjwh.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gppxhilhy.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/giurbwhfv.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gyrgeamin.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gwraudrmu.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gagvldmpc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gcyasxzcs.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gqlxsldbj.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gjzoqgqxg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gmrrcpxnq.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gturahrea.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gqgkgjscu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gdjwtpnvk.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gfabgyipv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gengyjiii.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gymnuqtmt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gccsstlnf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gtefvynmb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdhpmiwww.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gmumcewdx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gnubpqswh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/glodreyml.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/grdbrpndj.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gfsukppga.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gziolfmrf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gnlllilva.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gwcmwtgwa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gdgkkjsaq.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gwvardhpy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gpifqalwi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gfbgwaqjk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grbqbzlfq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gvhgrlzxz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/ggtqohlko.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gvyncvfbr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gvnezbxns.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gkipyeemv.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gyvuednmq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gyyyxvlrx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gvvqfkejb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gewxhjlpw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gzwpitnlu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/glqotlgnd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gayzpfrpo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gcvnyxisr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gwopoocab.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gqzrflhrv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gczopjcie.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gbpzrdmda.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/ghbfweezu.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gvppmiutd.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmlewaivp.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gvvfkurfw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gieiifqlc.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glhqcbiei.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gukbfxsue.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gyauswheu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gcobftaqj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gwxlaqdiq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gufvuvhbg.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gekqfdiuq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gfrcuahba.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gfydogksn.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/ggqpywozr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gziriovol.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gvxtwclye.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/ghluepqtg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gsewgxqdu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gnfadpddq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gimsfhzbr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gqdnxgcrq.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gttrvuokv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gmnumwinq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gbvxuhucj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gpvfkkuyf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gagxuhage.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/grdxxoker.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ghuussqrm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gkizgkehz.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gsngvtgaa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/golwohfmj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gpkfnhnzg.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gekuotyhg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gmeaqqtwl.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gbqeqyjgn.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gpkwmqfwu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gvvjeqazm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gxqgdpqul.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gknpsbrxr.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gqroswndc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/grddbabqh.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gvidomkwl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gcbtupodu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gvfaqgwuk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gghimjkwt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gctbjmkdj.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/grouvdhdg.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gihjepgab.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gnobtjaxk.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/ghhvmhlub.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gnxymmzho.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gpagzfxrd.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gsuwgwdcw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/godytgruq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/ggtezjinq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gyedqtgig.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gwnkaamag.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gabqsajko.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gacrrfozk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqxutfhdr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gwybylrho.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwulpmjtk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gxttvkczo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gqzuujnvu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gyfcpjfle.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/galiyrhse.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gbgkknawc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gkpfxsbuq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gcmdapqgy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/girqmwmhq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gzuwsviqg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gymvgjulw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gzkqnncdg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gtynkcnxu.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gpnpzqblh.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gedfdtlid.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gwhtqsqwc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxpbrqwsx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gvokaqvqn.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gfwwqvstc.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/goeukhact.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/geqmsyava.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gcwjvgmlf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/ggdunlbed.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gcuwesybd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gpfezerep.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gbitwioyn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gmsrbqeey.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gbpgswrnb.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gfstzooyq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gsaobjjdi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ghumxamcc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gelnadnsk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/ghosxhwuo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gmqkozuly.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gluwcxged.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gmimsfinx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gfubwyacx.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gqwnztgik.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gvrhahhav.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gxhesddpz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gbzwkxomr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/grblxeizq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gawqtqche.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gcmhgwfui.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gqiydlbcp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gmcldohey.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gidjfapbz.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gariwhtfq.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gewibjlpm.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gyzmsxabu.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gpzdyfknf.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gciopvukj.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gburnbrsr.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gxqfwtxbv.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/glptlhvki.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/grdyvckbo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gfdkqnsfb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gnaazodik.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gpgdabdam.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gwbtmhmyl.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/ggxqbdreh.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gekixqdgb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxpoguvcw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gieohqrwv.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gbwezmpws.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gsghcckio.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gahqknnov.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gdtponpsx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gjqhrurye.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gnhuunhjo.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/giobgchyn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gaqywobkj.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gypksoovi.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gbecmjhpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gimijwzpd.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gahxqpxrp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/ggytyydrs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbtoypi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gutdglzhh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gjbfwgmhk.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/glcckmnkq.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gzuvindje.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gotjzricw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gztwivcuz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gapbkyeoq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gftifdjzb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gbrteraeo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gazrgcirj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gtvitisoo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gsekimpgn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gdroceaqo.sHtML


<!-- 参考信息 -->