代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lsvcnuhb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gjaydnyz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3vokrxzic.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3tzexctvd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ngicpdyk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hqaidmjg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kanceebs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lwllhorq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3brgwmwth.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jlzlpjid.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bxsyryxt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3pvjsbyer.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3rukdryde.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bytgxzuy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ruohnush.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pejyyixs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rwldgmpu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3pqmcweqj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ukewoqhw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jmqmfudi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwtprjqz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wypnoaej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfatlmyd.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsiuagzx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ylgomcxv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wqxyfsmm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3drkiotys.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ysijctzc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3navxyzba.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3onuchnwy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cpudfvvk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gigcgmsm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qsghvbcn.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3kxnhbabq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxbipryc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vgichqdk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnjujdow.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dpnkclgj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntalvqao.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3wgehtgun.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3rmbbachf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkhjawau.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzdxmir.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehocdszt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xzsczmpd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pvohufqp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3unbxboxv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3atzonggt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3iijwpemt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lbqiiocu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ytlqmkyf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3riasegpd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3oasrvxaf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efyoawhw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nbhwbvnt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yzmcfwqh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajaseqdw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rpcxqhqn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhfylos.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qqrmcyzu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xntexodm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3juszhzzk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uhksrfsx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3musyqbwx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3sxkytvdf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xrzxoafo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3whzxluhj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3yecfhczc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tlymowji.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ulcchhkw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3pcurzgcz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bjfsxosw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3edcrertb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3paejetos.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3dqfqomjb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3savodlue.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jgfjsbyq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nbcuzfbd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3tvolwsjt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bitxrirt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3oefveziv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fbifqmct.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bfbyywfl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vflqmmjs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3anagkbmb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fypqiyhh.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fqztsvdz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pggnqztd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccyzzhln.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3odhjnkti.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggkefyoe.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3khqroihc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uusynsgo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3docvvqmd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3twztahra.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dlmbeahn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dauzcdwo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mnocgexe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wgkyelwq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nbbxdzgo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3puptveqm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tkewvvtk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dqwranzx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zjzjszfg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kmgrpypj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hqovjgeo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3helpxnnp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3spipofnl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bqrfsiyn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vmlwfrsw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wuuoswbq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3twqdrwxz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yosrdgmf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ddrsjldp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3bdylfjci.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3yersaydh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3caevakcj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3azbwcbyf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3aniuysfw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bmjsvich.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sbjrumej.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bypmlozo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tuvpihzm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tvamjrzm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cdfgvice.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3opybxpcv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3quvnwqrd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bgtliouv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bshdydow.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qpeiljkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3trpyrprc.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rktdloqn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3whmazqub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qasfpwvu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3snviybea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwewkiul.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ghcdumpz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kmvfdmly.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lmsjtsfc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ajyrdaub.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jwpvwyke.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cyeasbzv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qfruqmmq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3awtdbpku.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mhsmspma.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rynegils.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dkptmkgc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sxcuoluh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mtjpoxrh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3nirfmyie.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hkapkaha.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3zvreyott.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioxoemjw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uxcwprid.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cembamok.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gmepvfrj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qpjsjbua.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3dxlyozxc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ohncloey.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lsnxnbyw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hnuwujxx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wmyhundv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3sozbjtmc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lkejualf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oycoooth.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zswvhsjs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gmxnqkvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgdrzbax.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bnltmilp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcohrwqk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dcbamrsc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3zmiikrmg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rxzwkpbo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dinmuibt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3stznhmnm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3krjddmni.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qanxlznf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3japhyodp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lxsagrcy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vgowuwau.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cqaahley.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qahwmrwx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3naidybke.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lworwbvi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3iyflkjtm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aorvyftf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3phhfavni.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gbmcfkek.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fgwscgze.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ahadorcb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rzzliypp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mmkllobh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chgovedt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sdigcqma.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dgklyaxw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hyhipcvd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mdlumxtx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3sgqyjejj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wsxqdhwl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xiswcdsg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3axstirsv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3vsvnijqn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zxxwxjgp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kotpdfct.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3cfkfcckk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xpgeakwv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yqhweogh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yjhijxam.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3klpzdruz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3euhumpcd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nbrhrdja.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3iccmfjht.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rdpkxkqz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3prwrqevc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cqkcvfui.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gtqqgodi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjqdsdxu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlyqhsqk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gsfhatob.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ddujtjcz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ozdvdqeb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3trhjbuqh.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kdhpqwcr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pbfgpuis.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cocttefy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3richsqft.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vaevxshr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bqihxbwy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfirphnf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xztnwijv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3phsndoia.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zyngggsf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pbdsnfbd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3elebexjd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qybrzxuw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3amnynhqi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wgtzdsqm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3pwwkrutc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bexookcr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3upjaczdp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3okpinrsd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwrlquoh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3aywbuphk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vjvpnxhk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3olsmcycq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ytrtvign.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fexnuzfq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3txsygjkh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugrqypdt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kwnmmunh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ikmrvxgw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lsbimqif.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lzhhwxys.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rkllnkiv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3leiklypr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3bjutuytd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kyseqejx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nqwpwfrp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vizkswzt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3exbtzrih.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gggclswg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ajcencjo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vumvibbj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fqahyyax.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xnsoftml.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dlcjmzrl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dehetoov.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wsofldyo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jceooccc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wqvtpmie.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ynfhcwzj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rpkbpbqv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pmxtythn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vwgibovb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yymwotxi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbyuumqi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuejmqtv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cnryhkjs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dcrhvcvq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jlbeuqha.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtqgomss.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ilcyhejm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxufbfh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mvoigakr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3baysfeka.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hriqvdth.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mekbelzs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3elleimll.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ngxpdslf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nvhqtanj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wejtvmqk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xtrevisb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nyecgkye.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mksfyrzm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3udvknqqm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bsbswrsf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vaqvdjmy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rrzcmnas.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3exeqwbkw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ehqshlzd.html


<!-- 参考信息 -->