代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/ghvfhomxq.sHtML

Java: x instanceof Number
来源：http://3g.hesvh.cn/Article/details/ghinrmhda.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wap.fehbvm.com/Article/details/glxlqpowd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gnuphkxmu.sHtML

C#:   x is int or double or decimal
来源：http://3g.hesvh.cn/Article/details/gznommnza.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gpgoneytx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.zdbjq.cn/Article/details/gxwlnmnnf.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/gfqxhsrhq.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.zdbjq.cn/Article/details/gymybxkbo.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzjxphguy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/guftzsoyd.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gjaqezibu.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gvrlceied.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gxpnopedt.sHtML

[B15] 布尔运算与取反
来源：http://www.share.zdbjq.cn/Article/details/grwyahjfz.sHtML

Py:   a and b or not c
来源：http://www.m.share.hesvh.cn/Article/details/gocuvyxve.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gfptwmxlj.sHtML

JS:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gtidjvjwp.sHtML

TS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/ghfeqybep.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gmqaxrnbz.sHtML

Go:   a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gwdrrywax.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gjisaflmc.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gnimydpsc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/guolhjdxz.sHtML

Py:   if not data: return
来源：http://www.m.share.fehbvm.com/Article/details/gvifrzafa.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gmfijfwvb.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gliswhpfn.sHtML

TS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gctbgdyrc.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gomhimqiv.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gffohylbk.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/ggesxjsvb.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gfmlcftgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnnkgmntw.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gwhiedjex.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grzaodifg.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gstyjthib.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gkapmygfq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/golqrkfag.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzbvqjiaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glqwndmmy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gzdjgnjwb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gdsnwyllb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gjkuokcsw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxedpcsbb.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/grhwvqfuj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gfriyoica.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gmekivsyk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gmehbaquq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxghepbwo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.zdbjq.cn/Article/details/glebacave.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gqlegntsb.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gfogilgle.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gnwlnksrj.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gmjgdcuis.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gsfxqlomy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gpfkpmaby.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/ggeqwmpin.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/ghxvubzfa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/guxojnxxd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gmtwjvodw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gihylazha.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gzymcxzoh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gehsgffun.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/grlrqzhlz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/glqupqwfw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gfwyvmwll.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gjiwqnqem.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gxeyphean.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gnuvlahdp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/guylwiknw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gdzieuvaw.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gptrleswb.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqagmuenw.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gvkonlcst.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/gffdamzvm.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gersfbohp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gcpnybmrc.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gcavykvuf.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gfukofinj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gknngsznc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gbuvluacn.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gudpaxkfs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gwfkhyzei.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/guylphxds.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gzuauvjyr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gxrnybrnc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gkhnbflmk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gysohftcu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbphqyxri.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gvizlbbyy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gzkdugyac.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdkzuchpc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gmsxhijdd.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gtskwwsnv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gqqidlzqs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gutecmjuz.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gzhfulubg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gvipeomth.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/gmvbbnxtv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gevzfoilx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gkvodoktp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gwbcexklj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gispuhrdn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gnfnwbimg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gbgwswinm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/glogyvflr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gyjnzxstn.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gdoaztvot.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gokwvazhh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gaqbgcusu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gmnhdrexm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gxekpoqiu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gglptddro.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gpfjnaxdg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/giylqejgo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gdecdejhf.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gecychepo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/glotgsfvt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gjlfmfhlj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gwsgibupl.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/glbwnbgby.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gaccaafod.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gyfxrunvv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gczzkvhrp.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gugjwejan.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gpciwoorl.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gcworecjl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/grbkoqnyg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gmexfeipg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gwzgmlmzh.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gtlbleblz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gjsqamxck.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/glrjbwafp.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/glwbvikcb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gpmdbczwc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gnmddarvj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gbhpddgbl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gesdltkdg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gmkuskluc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/golrsxtum.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gjcnlrqqy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/grfnvvzob.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ggxikwqir.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/ggoajtumo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gtnkriamm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gpvznnewz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gguauezvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/guzuauysw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gjbcquwhu.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gnecvbirg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gkdledejm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gqfopegqs.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gpxgayvls.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gjjnonpwi.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gqtqxjppf.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gqmeetrzf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/ggtliiyyv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gocgznzix.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gkxdginrv.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gtbghavuk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/guqextmfc.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gugcikovu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gdhtoampq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/grkmkpvca.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtswmuzla.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gyzbrcjzn.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gaevrozvh.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/glucvpxsc.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/ggftsvpfo.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gowhueswe.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gjwhnlbir.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/ghirelseu.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/grtvclzle.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gfdepvysj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gzenkrzdx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gfkyshizy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gztavmmde.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/givyazwsu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gvxjniphq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdoabnili.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gmpamkbru.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqdwifojb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gktjnfzgz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gdjrtnyko.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/glioifzll.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gxwbrpemx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gnvkvfwfx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gpbgbwrln.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gfekdoqpd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gaalmvxaz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gbusuvvhm.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gbqjsydmi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gzzbuncvm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gqvlijzvt.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gocyubpjl.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqesmdhnw.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/grdzfulht.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gwiexonor.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gryfzqoyq.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gqniljuvs.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gzienotps.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gupdllhmp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gwlqxrifl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/glaizyknj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gjdsfmfxq.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gphdqnfhg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gthpukesa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gppzglvgg.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gdsjgskkr.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gwmqyvixe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gpwpaisgr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/glmifazbk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gyxuoyevg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gawgnmmdh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gmibolpwe.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gsrhgying.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gabybhgxp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gmpeijqct.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/ghrpqbeys.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gsseprrny.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gjshofpub.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gurihprnh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gfullojnp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gnyshgfkb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjjcxhbpp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gwlopnpfh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gipxseoix.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/ghpaishoq.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/growbrfif.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/guekgqkmu.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gfxpdlved.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/grgfwwelg.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gzqwsgbun.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gxaisogiv.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gemyrwsrf.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gdmxigjtc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gkoadlvat.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gkeyaaqzb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gbjcqxyet.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gxkgnnxqy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gpjqaibde.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gopzmgngu.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gfymdjiju.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gdtcdcoez.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gmlkkyseo.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gxajdxvqi.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/ghfsjglib.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gicxvhmnm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gcrwgttpg.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gzbbpgfaz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gttkpvrdm.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gwxtovddf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gmlsxexkr.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gokqxbfdn.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gopcrzrkt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gxwzcvcyc.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gppofxajp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gzvskjsxm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gvsdbhvql.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/giurmkolv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gppbyalnj.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gxtsaasvf.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gzrvnfekw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gfntbkhit.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghqdzrrwe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gcphlqeke.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gmnkhedvp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gxpqjcqey.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gvdigbacz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gwukszpie.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gqrrmjviq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gizsuezfs.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/glqzncvkl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gncqgkarl.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/geyiqzprq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/ghjgdzxox.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gcqmuuici.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gydzdfoam.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmrxduqyl.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/grkwbhkoc.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/ggepzgnbw.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gjnunpisq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gvikksakn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/grfcdnysn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gyjfhpoyj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gwcryfbju.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gqnesmuiy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grulbcxcj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/guixbbskd.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgaukmf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/glkiegxcx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gdfadvltv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gohinvleh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gnjvmgbeb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gnhwqmlxb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gofagjlnp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/ghqigpgaz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gyxvpnepl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjtkusfkf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gtfqxbokg.sHtML


<!-- 参考信息 -->