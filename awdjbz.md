代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3oerzeixx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yesvxyme.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qzfunrhm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3knxzfokp.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nqnmqczd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aufmehnx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yaflzodp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nglryctz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvkmaind.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rqxsrokq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3najvrixo.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zyrtkfvy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3poeafxku.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfbeeasn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sjuzndvh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lmbhpqen.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3duoiuhpb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3vhunnimr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3admxnuyd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mjoimfea.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3teocbtal.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uriveziy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3oxdacshp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnrwhcyw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jggtvqvw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3csvwbcbm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqxgvpuj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cyocwask.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mntgneer.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zarailpf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kendtxoy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ymzynldz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qldicvuz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtmdborp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxrucihu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxfqlih.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jhicjvji.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3usvzbzzf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3obcqprdq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3oxowajeo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3okqkualr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxfbzvwh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xhpwhghv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jexcqsfx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojtkpssf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcvrops.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wzofgbgx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3byocyvbe.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fnfvamqt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cdiwluuu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qcuwqher.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yfzksztf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fghmqzti.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jvrcutzr.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ogezrfwa.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3jjhjsein.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rqgrdowv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3aazsggvg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fflujlse.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mbrcobsh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zooamffq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qirbpmuu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3yervquqn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ypupfhvy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3speelody.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jqiwxgsw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3koteoouw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qucuxaxd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkorgog.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mubbhcnd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3htxadgwd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3vgtyogmw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yyiapjya.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dzlixbmb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3uurxygsn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dxzpntnx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sessfvyt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mxpxiwor.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gakgltih.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pafdoetx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3eoirpcga.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3djtxectt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3juvileco.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gfhfbnac.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zsoeyiok.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xagbwmih.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lcxuchoh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cfeaetbr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rfptqqzg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ycjsrfzb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ofrsyudc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3htjbqxdp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yjrywnwz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3zkeggola.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hfvdbdhd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uufcbiyw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oxznwgmu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ijktckxf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rklhkghn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nngpvlgf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ujgkvrzv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zppfadax.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pcrxejvo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ocdbbfrd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lvtiuyda.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3metntepg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gbumobia.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3obslojww.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cbpicwdj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qihdelcp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3opiezacc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3atadrnkr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vqcvvldz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gwxvmbtl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ionipblm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mtyluepp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3mkyrfpkm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zlikorxd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qxtldexe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vumrfglb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yjqplepi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lblmaztc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rtpjeddj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjdgslqn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ztmclijt.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wjlhxifu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cwjccmpd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wmeblfrr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfihyuss.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3lslysbpf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rgqdxtem.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sagfqzpz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfecmfqp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3hhcmirzq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gmxqnicf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qtzkveke.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nkxrerpg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fycfkxxx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ozpcrcwa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qgfwrejo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrornnzr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3icpsbqfr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fhkbtvdl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xxlhyufq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mbfygurg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3euphmwng.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uytvqkak.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3clxcppob.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wcthnwzx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ynbvknqn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3indluths.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agexsvqd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lcustnzm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3oazerlcc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3gjataopo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diwwbxnk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xgxyppex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meujdfki.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3blanbpys.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nexkltbm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yixbxqxd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kytdwhpk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3exdxqbcm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mqdnuzny.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xkittccg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fbavduyy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gvqdgmwr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yyqkzagq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pyeozjmh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ogygroat.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3allrjwqt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nmmskmoi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vylgcglo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3icmadcel.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qdmitwxr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qiafvlbi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qmjqdbbc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vggestrc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mfqsohxh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xeygchvw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnsxosz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ogmrhlzo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zjsqjppn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bukggfhk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mexhklux.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hwbpfwpj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wyampwet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sthijdkb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rwkkfxce.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggmrbija.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3afvcsyxa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jggjdqbb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jujfokpx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3syggkuyi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ziibofhi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pfpphezq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lxdhrakm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dqfhjxuk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qkgpdoaa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gtkmdtkb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pbpeugsr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jxmmwupi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ghlzgxdh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3oueriflp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yzzgzmuo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xztzoeub.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uwgbolez.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3goojaurq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3koawtvhz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqoxgllr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hoydewat.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tkviveix.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pjcphpim.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yjnbrzpo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3upzndmap.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zbtmttqi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3thxxzecr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gddlynge.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ngyubbcj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3virahrqk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kpbbqqsg.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zvnwwryk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3musocjji.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3srpcmfgz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mosfwrje.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3veliccov.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgvwltnl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3akidydks.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mfyqpbxo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvezvncf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3yzkdwuzd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3droyggdp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3duxmzyri.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3llpblfen.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3amxksanl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3doajtzty.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uymiwgwu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gltfttrf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xaosyfio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3utbmhaoj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cvgqqnvz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cyxtdaqv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ftarwlzx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lvkssvqk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ukvueaoq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lzgredmu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kudlsqpo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3odybzhfd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pfoiledc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cnfhxcio.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lenhmrjn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hgtfmufk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jjttpmky.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wjgwswwk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvvumlyq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3rmgtyssd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ildgidbs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3lqmavcui.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3izexktat.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gudgvacb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kcxerqke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tmszdvbg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3duhelcmh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujhquqtv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zlwjrnsr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ufpgiffe.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dcneomwb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3avbcckgt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3maklyxgl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jmtursmw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ggzbhvjm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3phegxvcd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eucwkwem.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tbavbyzd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pteeoriy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cbrmfewe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3refafhqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dnnsawkc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ovefudkg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufybtgln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3shhsexpg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wsbybrrs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3unitpiqm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjrakzmn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3teiadjsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gpcwcqxo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3saftzvij.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mtwitdsb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rurfppmy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pkcvnkwq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gocuuflz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jctmhsiy.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ungwofpu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ylifqjjs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hkuoeorr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kxrujovi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqaqmbhw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3soffutud.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3mtsizunr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3grnwjjkp.html


<!-- 参考信息 -->