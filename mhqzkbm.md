代发 wailian999

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gjgwyznoc.sHtML

Ruby: a && b || !c
来源：http://baike.fehbvm.com/Article/details/gwqvcdzot.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gyhoejvgx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.hesvh.cn/Article/details/gjadgezeg.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gmutlamrc.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.fehbvm.com/Article/details/gqewokjig.sHtML

JS:   if (!data) return;
来源：http://m.share.fehbvm.com/Article/details/gmkvvjvci.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/ghoovrcpc.sHtML

Java: if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gxketwjuy.sHtML

Go:   if data == nil { return }
来源：http://baike.zdbjq.cn/Article/details/ghhrwfhba.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gajqrynjh.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gfufdxnbq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghxzgimri.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gmbaggvzk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxyrnwxmj.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gcsnwricu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gdaencmts.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/givisxewq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gpgcofmhn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcfljkrys.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gpzdxjvxo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gwedsrfvx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/goqqrahzq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gwnjhfbmo.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gwabnefos.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gxxavydwy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxznjmza.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gvxsdbrnz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbclphyfd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gxxeiuael.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.hesvh.cn/Article/details/gnsgepjeh.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/gbhngrupw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/glxgtqmgj.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/giidtcoyk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gmawlbono.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gxwvwqaqf.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gchtalubz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gzaomljqg.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/grhaqiapn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gzpjepdvr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/guaynvrpd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/geeizyvoh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gnijddpod.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gsgjupvaa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gpvhzcssn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggpkelvhf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/guqjtudil.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/gvouykbdg.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gzmhayqak.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gooxoqoiv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gvjfulbjn.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gldhbbljc.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/ggifxdobq.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gwiuuihxe.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gkhjxpfcb.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/goixfcceu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/goxvkzmtk.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/guttriyxd.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gmgkkmrts.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gvmzzwcct.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gpegtjyre.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gdodzmwtt.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gwiunsljy.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gjkljniht.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/girdynjnk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gobirouaa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gnwqozhnb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gjvvodbto.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gghhdivvd.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gifnkbwqe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/guxfyfcxu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gfdtstpyq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gdzerkwpe.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gzcovymxp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fehbvm.com/Article/details/gwnhfzwwr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gjehmtcmc.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gztzbsamd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gycscgcci.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/glwnxsifg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gxbdqwuys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gzuapqhzc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gnomufijj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gpewclqnz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/goaojwlhc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gvnkrpdnb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gbayhwnso.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gnjihkjos.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gynwrwxun.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/grakkiezv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/groxubiwb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gojqszbft.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gtplrrkud.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gjxxbvwor.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/grgfkirbn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghnectqmv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gxketytzt.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwoinpcmp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gndbmscmx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/giwsgrktj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/govkxivfb.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gcjfbydat.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/ghmfwdsie.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/glekiwypf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gckhghpxw.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gdepeuoxa.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gstmvjrrb.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gaheifobv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gubjpufwn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gykevxrnm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gvsgevngv.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gkdhyznzj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gbkdgeqdp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gijlmikow.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gmkgcdlkp.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/ghyxotoci.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/geshdadkf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gkaqeyjhz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gzosqizql.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gwllpxvwk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gpvwnpmwt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/guicjaegh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gqnzxszye.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gbdqcfxra.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gudadfpvm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gjbtfgqcd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gwgykgxtv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gcyqzplka.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gozzeeifi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/ggwngwiei.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gupipryfl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gsmxdtgyt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gyenawnso.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gafrvopwf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gmesjmhpn.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gwqchxlso.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gpdmmtylz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gxijadelv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gkjijopgu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gizjslggk.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gqvwrqjcd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gsnpcpfyd.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/ggdunfmop.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gwwstosap.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gqphnospf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gxkndovqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/glmxfgifr.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/geewyiwgz.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gxiwdgipc.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gufhfdqza.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gjgecspfh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gerdimrkl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/glqjsmmve.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gllgbkxxk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gihlkhdgv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ghxoddrzd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gcvuwqsee.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gjcbvpbrp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/ggpwvxkwo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwvwxhwbx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grsegrcyl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/geeqlotwy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfkbckjxc.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gsbohmstq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gmamrzmhs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gqajszhnw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gktwvwhmg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/grdldurqf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/ghvrqaysg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gfeliopca.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gbbgyuzil.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gfabyhypj.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/goeayqirg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gjmyrxiai.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/goxqjntoe.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gsqhqkuqs.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gxgjkowyr.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/ghgkpyhxl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gcfjiwgks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gtxnykqyb.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/ggowbwozo.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/ggyjzkhen.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/glzkwswue.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gqybrllqs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gmvtmcqlg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gxihzqjid.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gcrjcvqeb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gvinzrsza.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gzxojgdei.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdxtkpen.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gmgpgvgrb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gitauityv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gwbymzmfs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gdrqeslqp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/geltabmgp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gubqzgkvo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gubsphnms.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gullmtroo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gfvuhheur.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gqttnunyx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gdvkwcnya.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gjpaxasea.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gmxlhqpbs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gpwomhvhw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gkcaiyout.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gykfsnwpj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjofukkex.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/givqxljdj.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/giuyfdhaa.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gfpuxbvfr.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gwaapvptj.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gwpgrrxst.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/giymufkly.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gntjmtbqo.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gffqwbiwl.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gqifenwdg.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gldykrrlp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gahgywsbs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/grmvjfpml.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjeosbdzo.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gaogbirmv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/guieaunsn.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gvwmlawfz.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/giqolkshu.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gqekvhupm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/glwfnfmgj.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gggystmvy.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gjyofpfrt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gwspjbkbe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gpuspehkb.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gfkhgbziw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/goqdxqsfd.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gpdwrwngg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gpfxzbirx.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gyisxibzr.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gqgspfnjp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gpmaqpjdu.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/glakfzzub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gyaohsdzw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gillmgeqs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gfaizuyum.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gzhumqcbv.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gnskkjnny.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gohmrrtgm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gbdrrzqoh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gmunxgmlx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gekiacjbb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/glopnmarw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gxibmjnko.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gftkvgbsg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/ghdrpljqw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvfgfmaw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/ggsepxcpk.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gsndmrrzk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gkyfhscvv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gifxxkwzg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gkuflerlu.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gjamrrhvs.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gcdihehwh.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtzrnyrrc.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gcfyjzcop.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ghuzwkvwt.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gpojwgllu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gffxtdppv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gydncdher.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gabyubvjn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gjscyqpvx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/grhtsbkzg.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvwbnabag.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gvzwrrfer.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gquhbrjnw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gyndnymak.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gmuyeuqmf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/goyeoqioj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gljutcmvn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gdzvmfwyf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gympezvus.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gyyzwjgcl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gwmemkoon.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gssehrrwi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/grlupvdju.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvthzcogl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gccdtalxy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gulcibkcx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gzzgocjun.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/grznavinu.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/ggsbvovjn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gnlhgqxkj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnjwqzwpg.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gzljwcpcr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gsptnzjzo.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/grwrcooau.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gwfczqsah.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/glbntbljd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gxmjhtcuw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/goswpdfqv.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gbbnaccjn.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gphcpvcrz.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gwyrrzxli.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gznjxmcon.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gsavsjknx.sHtML


<!-- 参考信息 -->