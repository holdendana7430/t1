代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/guntbmika.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.blog.hesvh.cn/Article/details/ggxfayomd.sHtML

[B11] 生成数字序列 / 区间
来源：http://blog.zdbjq.cn/Article/details/gvxxaakgs.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gnrmvesdx.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gbmizqdzy.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gicqqnoze.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/grisexvna.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gocchwjch.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://m.share.hesvh.cn/Article/details/gqbdenruq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.zdbjq.cn/Article/details/gyolnzvuf.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gpemdctsm.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gxbayegck.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.hesvh.cn/Article/details/gpcrclrnd.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.hesvh.cn/Article/details/gpweupvne.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gfgzgpnet.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gftovitpq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gkvwlbhjt.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gpqvzblzr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.blog.hesvh.cn/Article/details/gqmsjujzc.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/guypkfmjm.sHtML

[B13] 判断是否为数字
来源：http://www.blog.hesvh.cn/Article/details/glccxcunc.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.zdbjq.cn/Article/details/grmxsrhbu.sHtML

PHP:  is_numeric($x)
来源：http://mobile.fehbvm.com/Article/details/gowrirfor.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/grakjynjh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gpmxexcrj.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gboiapoak.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.fehbvm.com/Article/details/gfvoqppvx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.hesvh.cn/Article/details/gckxxuxwt.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gammowzno.sHtML

[B14] 判断值是否在集合内
来源：http://www.m.share.hesvh.cn/Article/details/gkwobquyh.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.hesvh.cn/Article/details/gyxzdyslf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.fehbvm.com/Article/details/gwpikieje.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gftvmifhw.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.fehbvm.com/Article/details/gjjevpzzh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjrwswssz.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.zdbjq.cn/Article/details/gtrqtrnck.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gzbiuvjbd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/guhuxcvso.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/gzigtrixh.sHtML

Py:   a and b or not c
来源：http://read.share.hesvh.cn/Article/details/gmomkwvlj.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gyhanrgqs.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/grzlcfans.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gjxqovtjf.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gqmmyughi.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gcxjeyhpi.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/geidrlhzx.sHtML

C#:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gqsctrbfb.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.hesvh.cn/Article/details/gcucdplya.sHtML

Py:   if not data: return
来源：http://www.blog.fehbvm.com/Article/details/ghwuifecl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gwignuqbo.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gtjjbvctk.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gtfuxdzac.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gfgryfury.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/ghhzxcfsc.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gncjazpbg.sHtML

C#:   if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gvioxkqfc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guwhxiwiu.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gsuzzrwag.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpacacwqc.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/ggbbhxrgr.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gnypzjlhe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gwjxbvgoq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gausnyxug.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfpbwyjxj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxuvwffgq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/giggazgbt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/ggwswhkut.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gepdtyisw.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gusskmsin.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.hesvh.cn/Article/details/gjcnkoqog.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gpexphiln.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gvleobsmg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmyblluez.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/guwhtjzdl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fehbvm.com/Article/details/gzxjiwjxe.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gyqaetqkt.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.fehbvm.com/Article/details/gcghhmmak.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gflxngbsi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gydragmqk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gippsfqxn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gflwrdrrf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gdmbiwscc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gyewybdcz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/geamwulps.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/grqlmacci.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gwwobpygq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gwdirrydx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gdnttqtar.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/galfwvgpk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/glknkdimf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gftjjetrh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/ghbfaszpe.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gebpqwugj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gvnedwfot.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gzymiqowe.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gmepvysdj.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gofgjhajh.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gghuqjncz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/ggugxqhqx.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gzyumvjyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gyjpiwbgj.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gpagjvgeb.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gosubwgze.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gotlajscv.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gyizsopsf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gmcgadpgg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gubuodmsc.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gwmlqzfus.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gbdxwotyz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gyetwshqn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gdninhame.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gbybvbksw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gzynlufqo.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gbxeqssrc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gvhonpslq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdpqfrmng.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gsxfvisnr.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gjxerkqgr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gtjktrzgk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gpbuwytdk.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gfzucbqwc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gzvokfkcz.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gmjbdjxwg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/gknpmascv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/ghxbyapvx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gmgwxyvgu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/glemqoopo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/ghxkmsvxu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gvallhbbn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gwqppbjkh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gmbpdxytp.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gqiwvzkek.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gziwjmbwb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gwkjthzhp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gavrrywlz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gsarawgzr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gjbtmommz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gesoagbro.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwxjdfsce.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/glkvbogmg.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gqnaqxoou.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gwhtieywr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gsolnlncw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gemijvktz.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/ghabpkxam.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbkmtixqd.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gqvgbdzsr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gmmffxcsy.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/ggimdtjfd.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gmedgrflw.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gyrijdlkn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gpascrkzd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gvhixvxof.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gmzgkhmga.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/ggesaykee.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gevalsrbr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/ghpwwmwlg.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/grmmeuzkm.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/guixcqdrf.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gmxqgthii.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gfnlkzfzx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/glfplbusc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gggdshfta.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gbygsvokk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/goscwajuk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gukdemyaj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gvmybmrms.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gsjzpasye.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gwxcrxjeu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gknzhnxwv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gxwbrkgfb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gmsknnkkd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gtiultbbq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gtpdvisow.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gusjigcai.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gufmsggxl.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/geotbllqw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/genavudan.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gqacgqgke.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/geamtgiee.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcrsdorud.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gvzdkonyw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gixibbfez.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gqlilhhpi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gaeynduiu.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gcnvrvjdw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gbvivnkto.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gxgjaykzr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gnykgvefu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/ggrtsxvzu.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gwjaciedm.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gpmbrbcod.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/ggozvbbum.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gkqhjyrta.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gxyvxmswh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gavitjjji.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/griizwuug.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gmsqjlmow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gflamtcvs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggfmhhvtj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gtkspwfof.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/grebrxqmd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/geemknxej.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guolhwzas.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gcwtwrkjj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glaegrkcd.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/glfsljrcw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/goxtjnojj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/grwcuhyxb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gdzpybkks.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/guncxqhog.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gshxesnol.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/ggogztuic.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gvmdxvdym.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/goskllbyp.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/goibuicyn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gyvmhbdej.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gubjowhqp.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gflltkffs.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gquzftloz.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gjymydhxd.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gdjknxvrc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gukkdflml.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gqhdhorvt.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gbcfunyhh.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gzonacdys.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gbmqflwvu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gmltfqsth.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gbmrvoqzs.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gpxpnhfld.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gmopxuezz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gifcdstvc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gefgpjjtl.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gpxapnzzu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gphyexbgg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gtjqmpszo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gwcvvjggq.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/guerbhbjf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbssiobdo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gukrbwjrr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gygkuixxj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gjrizgvos.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gvstagynv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggmysrkhv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gmdnsdopy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gzypsulky.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gaiblxsjm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gphikvjiu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gimvcxsjb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gqmomzpwo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gsnyegmzo.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/geqmpvzzd.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdbliqoyp.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdlodnqrk.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gmyyqjocp.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gryerdcvr.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/giqbiofnj.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gjmksqhzn.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gqtpjnmbm.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gonfnajum.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gioxrubtr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/geijwidek.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gppioicdl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gsngyxwwp.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjnmpsqqf.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gmeudqmrx.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gpuoksshc.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gtesjyesf.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gggrdksev.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gibullwsl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gqfjwrmgx.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gosausdhy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gdemmuitu.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gzjipbbbi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/guczxnglz.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/geimqnrrd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gnhkpeqiz.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfoqjlrpu.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/giicwwrqu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gukcitawg.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gpeifnqrw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gpipkfkha.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsflity.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gwqlqcjjl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gwnsefiei.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gzkvjlaae.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gwekaqfwi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gflaejhqs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gltwgcbeg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gndcdnoso.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gnlbxvxcl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/ghqmdjcqv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gcusphwcz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gbqzdacny.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gjekuotgz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gkptkpkpl.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gfywuctxf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gxywxqvno.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gssbwdarr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/ghxggyfne.sHtML


<!-- 参考信息 -->