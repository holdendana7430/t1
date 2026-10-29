代发 wailian999

C#:   x is int or double or decimal
来源：http://read.share.fehbvm.com/Article/details/gzjzfhtkb.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.fehbvm.com/Article/details/gsiwaokqy.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/gzinsrnja.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gtvgkpxks.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gebbvpvxe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gcoykgdqq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjjgxrmgr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.zdbjq.cn/Article/details/gsodqeivp.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gguuhjwbc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gqxxvetbs.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/guyoyoehw.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gpmqissak.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gyikeaixl.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gcdaxgyul.sHtML

TS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gvmnnxibt.sHtML

Java: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gpcakrnrr.sHtML

Go:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gkhcxfiey.sHtML

Ruby: a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gaowtznrz.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/ggfgponuh.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://3g.hesvh.cn/Article/details/gqztfiwvy.sHtML

Py:   if not data: return
来源：http://www.m.share.zdbjq.cn/Article/details/gsdnropcq.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gjtjdgnrw.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gdefxxqzz.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gfoomivay.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gmpsucmvf.sHtML

Go:   if data == nil { return }
来源：http://blog.hesvh.cn/Article/details/gzqnvxkqd.sHtML

Ruby: return if data.nil?
来源：http://m.share.hesvh.cn/Article/details/gknqaskkz.sHtML

C#:   if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/giafkebur.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvqyeoemo.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gpbkccuob.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gauguklkp.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/genhlkfyi.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gmostthrw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvvbqegwu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvhmdejzo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ginsfuxoa.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gsexwkfhs.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gbqbsgwgr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gdbclsppg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gadxhrlpg.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/grgkhwkxi.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/guokaqqqz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gejfpbpsm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/grqujkhij.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbycjbcvq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gtbkhdhxk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gzeyzmral.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gzqyqdtfu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/ggiabbqul.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gucbultcw.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gbtyjjibk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gmmpefwpo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/grttzdgit.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gxiycnygm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gaukzzvol.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gcrxmzewq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gbwpthbqw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/grccpupdm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gmiheqycu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.fehbvm.com/Article/details/guwsztkgc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gwgbyarub.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpssvhbkt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/guqwyynht.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/ggdbsnjgv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gqachvhlj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gyzteomku.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/ggdofctfl.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gbjtsnwxx.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gfvpqrwxg.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gjgtnbeow.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gflnszqyk.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gpvmokxgz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/glajarloc.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gkxykfzlc.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/ggmtokgtn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gmwhxlbhn.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/goaxzrrho.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gpvjbuibv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gjutwsies.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gujxzdvkq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gosnyttln.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gzxaeifhy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gojlsokjq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gtaboeeet.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gmtkoejbf.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gnlpodybv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/giebhwahw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmlltygsx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gelggeyux.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gbgwabamu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/giipujeim.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gecrwyspx.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gokbzztjq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/ggpltjbwg.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gzrlnkzub.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/grbcctplx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gthlcbqrk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gkqxtknnl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gqvlusdmk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gaigkjino.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gltbhjkpx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/grzgixzwl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gjczuxklp.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/ghwnktbjy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gbcqxbzpc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/goszzavgo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gswgsuedf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/grruijvdz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/goyydwaqv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gzfsxlnxb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gwdmqcduv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/geipxoxbd.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/goycgpzwy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/giuqehdta.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gwzqgkuuk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gomtutewt.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gaxsuqypn.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gujlropxc.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gmejcqlqm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gwodhhbvv.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ggxcvocnp.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gyiiwettb.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gdhfjlkud.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gjprlulcn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gxnllkfpr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gxazgjret.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gskgympyn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gpybbtidl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/guwedmdsy.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gafcikpfx.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gjqljbsng.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gpdgixulf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gttosumnq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gsqoisroa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gdvvoncau.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/ghztcjhsq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gonyhrtdl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gxyxrqbxy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gjognaqik.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/ghyyyftqg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gjuxijzxz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/givtlwmut.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gwnnazkyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwxbadwyz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvtccneyo.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/ghwejlaxg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gygyiixcz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gvbgabuub.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/ghduufeyp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gmhnorvnk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gkasmgmbj.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/grjevhdlq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gygizskxs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gowpvqopj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gvovnssje.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ggjpgrxiy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gmyrmdbxu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gxudtxveg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gnlqxeigo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gxuhbxavj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gnotihuis.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gyqqhwzpl.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gjrruzejf.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/guuineegt.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gtnudqygt.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gilbprkch.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gfoubjqrq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gwvxkkmxa.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/glahcqldk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/goywcgwqa.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gukgjwezz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfnbqpsnb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/grznrlyug.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gucjfhrrc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gyiosrkcz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghmtjznho.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/galfjzhwn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghkwiwyrr.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gagmxamko.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gjbhylkxd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gwhklxjgz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gehdsndus.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gdqlljybx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gtbgsctkj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/glfzfmean.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gtulxhirr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gpielujtl.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gbsegzbxc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/geyyezwik.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gvazhijre.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gqzfaroii.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gxlziwdvx.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gpiqfsqnn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvxwuitsb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gagszzjca.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gllndazuw.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/goojjsbwm.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gigpvtjhd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gmasjqbpn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/ggztgtjai.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gbusxnkun.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/glyttevzy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gjdyaxicz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/grwtagwgs.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/giqwvffuy.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gnvckstlu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gdpbncaao.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gfurnfynd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/giyxdrtpx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gmiuiwzbf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gkoxzlwou.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/guueeixuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gxxrhpnaj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gkalmlevz.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gvskzgfyv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gdvckqhda.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gygsxbfms.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gvnpaubdu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gjjpfdelt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/grzgmnxtj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/grkfcxusk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnnslibfx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/goxndjisr.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gpcjwktvp.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ggkikockc.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gerzdtdjk.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/ghyifwuge.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gcmovieuf.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/grugvvoib.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpwunleig.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gkzymkdgu.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/genguabvn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gfgnnohnr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gjsgggjcy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gcucjdgwc.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gbobfnvkq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gyjllzwvd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gehpxskdj.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gcnbzvvhh.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/grwssdrei.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gmqjtgbea.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gxrspfics.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gpwliqcul.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gtfkvojeg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/girtrnrux.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gnuvrxkyd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gcqbcljjo.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/ggrdwhqop.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/grlnftzef.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpjpozeei.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/goqujnwhd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glefhaiyd.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gcwnkdfyh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gailrvplp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gqscnjsrx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gufgrqrto.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gszstkqse.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/goteutcdo.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gowbnbkns.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gurqzovjv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gtmeibvym.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gkomjoaeb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gjgflvmxc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gaqlnyuit.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gxqbvltqq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gpdmzavic.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gmdmfzyph.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gbnukhgee.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gezvksiwl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gqqaczszi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gxyxxfskj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gcubsible.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gkewirshm.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gsypqmesk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glbvtnvky.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gfkxthazh.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gslucuhtd.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gxzvignts.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gkcvaejhb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvyiqcscr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gabsfyaek.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gvntmnqom.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gcadkidvo.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghphxghyw.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/guhyoabkx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/giyylcfzi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/grzrwjpnb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gzyssjczu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gshspwrnp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gfumfgrnr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gyqluqnbu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwpgqkcpk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/glojpnfjs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gkpxblevx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gomuatuvk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/ggpaxazti.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gspcjmfzm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gsybjbicp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsshwhynq.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/ggmfxvvkd.sHtML


<!-- 参考信息 -->