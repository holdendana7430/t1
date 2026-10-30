代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gpjctvjhq.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gwtcxsfgq.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.hesvh.cn/Article/details/ggphadyuj.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.fehbvm.com/Article/details/gsvanohhb.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gdgsvimno.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fehbvm.com/Article/details/ggtnymqrx.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gvnxihtta.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gnhfspkop.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gomsxilyp.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/goeeiruap.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/gbztemzub.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gzdlcbuwa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gtlnzvoxd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gkqgqazos.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gktqndoqk.sHtML

Py:   a and b or not c
来源：http://blog.fehbvm.com/Article/details/gwtefdpon.sHtML

PHP:  $a && $b || !$c
来源：http://baike.fehbvm.com/Article/details/gmrbaldgj.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/goixsshkt.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gugpenqvp.sHtML

Java: a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gtbervxia.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gbquyasaf.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gkffftcep.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gntomwfdq.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gqeapdcrm.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gvltzhzgr.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.hesvh.cn/Article/details/gjsnwyaro.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gbsroftpv.sHtML

TS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gvtpubeej.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/giowexpkv.sHtML

Go:   if data == nil { return }
来源：http://m.share.fehbvm.com/Article/details/gsyxxqriq.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/grhcdilhq.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gupejadgb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gguohfhus.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gkfyuaure.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbxioxjhw.sHtML

[C01] 定义函数
来源：http://3g.fehbvm.com/Article/details/grbpqnwxr.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.fehbvm.com/Article/details/grfombkmr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gacwopfii.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gxhcabckd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gntxghvwz.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gyaubdguw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.hesvh.cn/Article/details/gqwplwhcv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gyifcimww.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkklllzey.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gewviossf.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.zdbjq.cn/Article/details/ghxtyxtlj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/ggnyxrulj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcwstcvoo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/grabnjbiv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gzagrnjxy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gnwceemwd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/grscvkwhq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gmbrdxelk.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gfdwmarld.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gzkfkqxcw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.hesvh.cn/Article/details/ggofekxmv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gsynvpmrq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gezocxqeq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gaqqhawjv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gmkcristo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkexqqtkw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gdwdedbqh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gkawkyjyl.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gvrfhxfiy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gcagzoboo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfmaoezq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gdjpqtkqf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gliazuxgu.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gwtptjine.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gyipsmjlb.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gblsclpyk.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gvcbrfmlg.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/ghegcvldx.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gnzvgybmy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gctltejvk.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/ggxnepccs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/glxcszeix.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gifiavdxk.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfzsciwyw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gfsrhblnb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/guehsfxvx.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gecrkermi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gbnedneqe.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gqqzfuitz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gtvdtzjzc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ghomcvpbb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gilhchjaf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gurcdgnym.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gtrbkkwvq.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/groenovxc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gloqjnwla.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gpowspizt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/grkgslwgx.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gvzeylngw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gixswvlvb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/goindmisa.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gburejfzr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyyvccb.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gckauxazn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/ggyfdqnay.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gdpmsnkhj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/glgmfofps.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gkhuufcco.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fehbvm.com/Article/details/gvzxjsabd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gavuzjdni.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gvwnkocax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gjrbminby.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gjuozehnb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gdtuvgjbg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gmgcvybrk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gykksydru.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gexnadpza.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gydnjlewr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gaigrmwau.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkacudaki.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/ginzkjtcn.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gkckmeuqu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/ghojdhdkw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gjzcpfgtk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gkzccuego.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gbmyquurq.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gemrhvhsn.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gurmbhkjl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/grixrkwga.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gsangubyu.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gsascousj.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gfweiwikg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gwemqknqo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gmcrlibet.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gxlrfgeek.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gtvciccya.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/glqvbkers.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gkboaviky.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/ggtatakfo.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gcbqjrntm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/givixfimj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gduhkzpkf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gqgzfdbal.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gtzcfoxze.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gsyierwph.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gqfoyqkvz.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/ghelspvxw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gngtttgfv.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gfidwaowx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gaadcrmqs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gvlsfgzmw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gyjfafusb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gkitxgymu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/ggnuivoii.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gpxtpliwt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gavvblear.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gnfasnwqo.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gcshxjyey.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gofdmjgzh.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gfqycmtho.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gelumjwon.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gnztxbtpk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggswsqryo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gfivnjvcg.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gczbzjapg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gfqlshtam.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/guuuqnppm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gajuxvfhy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gqvyreylh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/glklzzzmk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gudbjtsdb.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gfklpoong.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gewbjkaju.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gaskrogik.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gckenbhxp.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gsutfmqpd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gkfyarcqp.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gyiebtdjy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gdoxauzot.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/giptvkxbs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gcpjgfzod.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gnlphuztb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/ggxvplrjb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gsthqqglx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goafauzkj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gvgdbonmx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnqufpvtg.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gqvsycpnm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gwmgskgqc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gdewixcvi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gzdrkpolq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gqanmafud.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gicwixiqr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/glnfzmscd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gebtinxpl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gltbgiagx.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gwccankda.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzdlfoc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/grbxsuljg.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gmdowmocp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwhzdetx.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gnjkzrvgg.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/ggyxmjyen.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gghkehznr.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gwdrbukys.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gzjognfyu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgsdtcv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gjcegulqa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/ggancbsmr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gpvgeywxi.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsvmvznoo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gotwbtjeh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/ghoicipfm.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbgpmbmlq.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gvjeejqxp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/grxwgzljz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gdgejdcpc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/grsooyfqx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gemxkrrjc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/govceswpv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gtabirggr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gufmxyexo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gnkjtzgnm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gfgzdkvpg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gpfvundox.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gdyxtzhaj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/glflkerji.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/ghumulqcd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gaqgyyhuz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gomhlyfpy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gtsceuwav.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/guynowjpy.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ggshmslqf.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghajtxatn.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gyjalzsix.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gqbwyrfcz.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gpbvrtzot.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gixoqgdmu.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gltltgiws.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/ggddfqhdo.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gqhstxyea.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gpdrlzwam.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gtbbixtmx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/grlqreusn.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/glookprnt.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/glerzglug.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gpmpiojdm.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/grttzmliu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gnjqaieij.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gjmuzwjbi.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/galtezokd.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/ghleawkpe.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gvnsevnqq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gftzehwtp.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gvjcjqtdn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gsyqficux.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gbmgihunl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gkxxddgea.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdfcydljj.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gnxdvflvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gasymyjmj.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/goczgpefh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gdzymgjnt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/geuisbmoe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gkixnjryz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gswstmecj.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkvxbveem.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gwhcmugjw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gdkewwzan.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/goipkkiga.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/geuqbzvhz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gtbritkqf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gjxkstlfq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gcunjvdfd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gebahslkk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gnzanednx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/grrizbnyg.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gwdoybezy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gxcygnnvf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnslpptvq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gisdqohja.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gbjyaivjs.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gjcbhxiei.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/girycsfxn.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gcuostlxo.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gppowcoxd.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/giuxtkmju.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gcfovwonq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmhhtmcpd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gcplawveq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmwzdpfpp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gjpjdtsvp.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxedbqhtr.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gmbwlleok.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gtuzwuvtq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/guigmlmpx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gznehpvfj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/grrlccqum.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gwufgmiov.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gedsdsqnd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gjhtagskq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/glkdqwngp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gmjnehsme.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gabgvfood.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpzoyul.sHtML


<!-- 参考信息 -->