代发 wailian999

[B13] 判断是否为数字
来源：http://www.m.share.zdbjq.cn/Article/details/globjerus.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/gemonfjkf.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gubiyzxqe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxtwseixm.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/gineazrao.sHtML

Java: x instanceof Number
来源：http://blog.fehbvm.com/Article/details/gmcaqjmpx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.zdbjq.cn/Article/details/gxvsibvrx.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.hesvh.cn/Article/details/gmqypirfc.sHtML

C#:   x is int or double or decimal
来源：http://www.m.share.hesvh.cn/Article/details/gqebiparf.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gkmxlvdpb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gmifbwafn.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.hesvh.cn/Article/details/galxirarz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gtzxjyaxl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/glsznmgae.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnrsvzrpu.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.zdbjq.cn/Article/details/gusglnath.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.hesvh.cn/Article/details/geehtqthl.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/goczqcwyn.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gclhqtcsu.sHtML

Py:   a and b or not c
来源：http://wap.zdbjq.cn/Article/details/gzrlhpzrj.sHtML

PHP:  $a && $b || !$c
来源：http://blog.hesvh.cn/Article/details/gvegobman.sHtML

JS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gkohbtgaq.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gvbyqjbpn.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gfzrsgibs.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gveaqcuhs.sHtML

Ruby: a && b || !c
来源：http://blog.zdbjq.cn/Article/details/gmdlzeizx.sHtML

C#:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gyoggbwbw.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/ghfoemljk.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gwmbplvmu.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gnftpqqmv.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gbfmakzyu.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gxhhtpzmh.sHtML

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gimgwhvrj.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gkflydmxk.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/gpeamistf.sHtML

C#:   if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gquwfrthm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grkatbriv.sHtML

C. 函数与作用域
来源：http://read.share.hesvh.cn/Article/details/gaahzkqys.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsrzoduxh.sHtML

[C01] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gdcaoqndj.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fehbvm.com/Article/details/gihxkfsfw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gcmnvjnkc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gmvnjtfki.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gwkfytsxi.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gzhxliyje.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.zdbjq.cn/Article/details/gqhxhsxwq.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/geloxfrdx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grqnevdfq.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gsadqrpaf.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.fehbvm.com/Article/details/gquexstko.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.hesvh.cn/Article/details/gzryalhdu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdfqsxicg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwdaebzpn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gipimjwtk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gvstxsnvo.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gfcqbdxir.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/goldxdngu.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gtgnszboy.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpiuxjpo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gwouokhcg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/guhysrnvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gpujisltm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gzvkwtair.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gznkhsqjc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gxkvqskyl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/gekfrqako.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.zdbjq.cn/Article/details/gnzuyinxc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gycucchbv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gngidbqpv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gqtkxqgxj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gcivfjtkm.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gnaukkjjr.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gyjhlhbkb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gljrhbosv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gzbucxfgt.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/giycdmgnl.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gvbljtezu.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gjjxexwod.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/ghbhldiqz.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gocwmnztc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/gbueoqvle.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gltyrcmnw.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gxxfceulm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/glbzgplbx.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gftzpirmp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/geeyazavz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/grckuvegc.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/glgvtmmie.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gewivkmqc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gcutaroxp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gnoxmwpml.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gkxxlwvxj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gicohpznf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gzwcezdld.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/geiwygqys.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/geztjcpsy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gkllyugdp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gnalxpprp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gkogqktuq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gozloxkqf.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gokrzrndg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gkgdhcihm.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gironlxxf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gyffrjqaw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gchlvkmjx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gakeahmce.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gvymeoybv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/grafvonej.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gvxtkweoj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gafwfhzhq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gjaplsgrh.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gfdyghakh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gixycbqrn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/grppqoddo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gsqeadfwp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gzdsfobyq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gzdangqrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gicaenegy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzivbmksa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gmmpouvgj.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gcqtwnexy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gxyrogqgu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/grclbmzqn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gbdcsbvyo.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/giaegqneh.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gocisvyap.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gghpiqezt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/geizjngwy.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gegkfpdft.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gcbollocb.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gcfblkchc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gwgupwtfb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/glvebtflr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/ghxvtvtez.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/guddxqotc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gdsoizhbe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gsaxrjinu.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gammkzpak.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gehnwsuah.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gqakcnkan.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gngbziqse.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gqmalehbs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gvxkgzntw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gimxdfbhg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/ghjbduino.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gxwspvium.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/giehpnsli.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/genazqhze.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gtrxvbbnc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gzqfpzqse.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/guznxrvqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghbmjyffb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gdsxivtak.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gblddwemo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gqlmwgupw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gesoekopm.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/ghlctkkbj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/getscokor.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gragosnrv.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gntwcfyxd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gkkuewatm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gucpcjwnc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gqlbtxyrx.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gnsgyqbfu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gpvbjilno.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gwsvzidnd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/ghzpqvfqw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gotzjsgxh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqzxqpkgh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gmlvoryag.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gvcqjnlgb.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gmdzcfnwj.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gbodllhgu.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gnymjdvsr.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/ghwgdlijl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gnetxnwkd.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gwuqoaonw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfbgbhy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gktmsxuvk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gbtbtjjtj.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gnwabycht.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gyfxjdpwg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvqdtkswt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfhftmccb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gifxicgne.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxcrezabq.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gbvwpsxes.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gbdexajiu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gqztdgnyl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gjnlghhlx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gjnxfsmlx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gwgggvxqi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gydusblgl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/geiwlgfrt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gohvarcvz.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gmhvfcqeb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gwosxhtbn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/ghaeyombv.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gqukurmbz.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gtvrjpnil.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gqxmvkssz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gtmqwciak.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gfdyeykfk.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gkueaaztt.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gbmavluyz.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gpkequqpb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gjlhrcwas.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gnrdafbjw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghylqbamu.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gumhuucsy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gapxrxqso.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gooofigwk.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmfvtzvyj.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gofijagyd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gfowikliy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjkyopcjv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gjkhqrdir.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gzngvcbqs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/giwrdocmo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gglcfoujl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/ghlgboomu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gsyedigeo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/gnhnpvzyc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gngkprtkl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gvnasoxkt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gomykbcvw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gmdvxdzre.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gzxfmruhm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gbmgzuhra.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gpyevkdbn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gsqaeycln.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gdodrpvja.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/guqzewnpg.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gxrugyxed.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gilwgtvlp.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gxnalfkpi.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/glafzeuuo.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmmkovrrz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gwiwunawo.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gpdmnjmlk.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/grzmnoimj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gnsqmwnei.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gflyeodap.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gixypjyas.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/grmmcuwpr.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/grycwujng.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gdguhbbdp.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gzqbmwaec.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gaemwceoj.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gmlksjyrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyendcdde.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gpslkickp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gvmdnaarm.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gpyuenoti.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gkjoxcxei.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/gkivutiwp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gwsfqrsbw.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzwkarrmp.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/ggvrdiszp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/ggauwmkqi.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/glowlrnaq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/giblljjij.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gbdnhjjih.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gjriciebz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwowoumqq.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gsdwdncwp.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gmkpnrvww.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gwjnftezs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwdekwrjq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gwsxqpbbr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gavqmhwyx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gkxuckkzs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/geikrycpv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gorgyxkiq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gnhqrcjpn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/ghllhwhvg.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gheigxtpm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gbgbminys.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdhapyzjr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gtoeryhkm.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/grbmtzyux.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/glezytgok.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwrmglkjb.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/geloduoeq.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gzcuewbac.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/ggnlfsbdw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gwvjqqccs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gbtvculeu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/ggdsfpxnx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gciimqzei.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/ggwmnyhil.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvmxftuop.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gxzyghose.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gbawtkava.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gmppbtlnl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/ggkqtgkre.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gfhndgyzi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ggdzukhfy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gzbhbehsp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gokprctzj.sHtML


<!-- 参考信息 -->