代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3gaynjlbp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycjxoowx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3paycizjj.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xkhvphwq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ogkbeipb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3aezizyhf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3usyuxjhb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kfkqnzjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfgiebop.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qtacvtzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsnqlcuu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3amfomnrx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ztimotfj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tojuwgqx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulvwtafx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxyccogf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjbfepza.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yxvibpah.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wejoizih.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhqizpz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3uuabpvfg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gmbgvvys.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3emfkqesp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nogohdlu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezxhntij.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lxcdzzob.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ruyepgke.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hnrrnnsd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uengssgh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3izxenymx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3spsbjxti.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nmmttxet.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ilrwrljq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqvikmyi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dngkexja.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkpwroh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3edwumzsi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mwtrhehr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3auetoicd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3pfynmdim.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ijuiltkt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnvrlbov.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rhldepfk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ggnaadul.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3rtkmnsjp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jvsarnxr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dpewvhkj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pavtinxf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zsvlgtaw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3flkncrxd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sgxzahbs.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yzgtdvvs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ipwepnld.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zzowaapi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3imaufomm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3qqapdoly.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3crempabc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gavqecok.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nlivvlpj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nxeeztlj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yrsnters.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wjjncvwz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qepxcrti.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wdftdczg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dbxopfby.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3glixtjtl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qfdefsro.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3otjoiiia.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uhszyflz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xnzlxzky.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kpixcgjs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rwvjczvn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3phduxzxu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gxxrmgpv.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yjjmfyqo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3boibjwye.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vkxfpfyq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mkjglldg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmbxwzzf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3djfoixcw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wjmzohsi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zluvmhhj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ibdqgmfd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qwvaxezl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mimmuije.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3adftssbe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ypizzqmu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ebmycvjz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqccwyv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lkwqmlgt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnefnsh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ejihkjio.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3egydpdcl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3clfyfwyf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ahgizfnm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rkfcrcoh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oasiqdsx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wphbekky.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sgpnetvv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pygvgpml.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ehorhpnx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3oaqsjfbw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3esferbyw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cbjxmfoi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mjlapavg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3wtrufslr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3evouudaf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rpowvihk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3biluenqi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fgscafhp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mfjmfrry.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sriwsygd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nsqtfziv.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vhaehbsw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zdcxqvku.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nwciejif.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fplfzekj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3xvrnufhq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3poxiuywx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zlglgqha.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fduhmypf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vykovkdb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zjmpsujr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yprsnvih.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbnayrjg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vbvmrjbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lzeyictd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ypbcnusy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3cnrdinah.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3eweovrxl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fzetzpxf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3escqynzl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3rznrzxbf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3htraupfs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kdyxoksu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ebnfgnjd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3vaacpdci.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pfsxvpka.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3czkihpuh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3deyhtsbr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ejzewigo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgpziryz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eavmxgpw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zykgzicy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3bfirkxsc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3irolriic.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ddapkoni.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hbzlxlei.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ddineheq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tlcevadh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vgcfgwde.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhrworah.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fxtswklh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wowkhtwq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujxyqtdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kihbthxv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yfpkjqhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajgrwjno.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fsvkomhi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3glivkglg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dihfigqr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ljemckoc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3aqibooxm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3snzsrbtd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3pjoiujtb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hstlzlwh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3awssdhzd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3irmrpkxg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3tcrzoxco.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uiloirao.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kxqjiiyc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tcxmgyka.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ulqzkwpe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sbthxiud.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jselctee.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mgxublfp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yvbgylds.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hnwmcvcw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vvktyfyl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3luyjzzvt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gvdempae.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jorymmlv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhodjyn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3owegpzna.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3luhiryyf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wxdxteoh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3swqzmtqx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmvcpzjd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rxmlgndm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlgutrr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qrabmpbl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lmayugtb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fqaeicps.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nweojnbm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ywcpetya.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ikbpkqys.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wqbiiani.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lohanhck.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vfronivw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xbebhiwc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3taapqvsc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bxzprimf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tiwxzhgj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ogifgkoi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiiktffk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xaadnsad.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3srcleafd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3evbdiscr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3yiscbvtv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3npuaowff.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iekwtdhu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ibnzveid.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pjqjhrev.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dzletzjt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3apwtxcca.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3brhsfanf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ydttcolg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ojhpknix.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hhwninfh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eblsdwxa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3myjbdhbi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xvxggali.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3besziznp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3akcrxqjc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qwhdrkrd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qtenjqot.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oimzqthi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jhtiosgb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kpwxnijl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfblanfg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hopnympy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3icvmpmfd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lxpttcgv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hvlnihpb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3riqxydmd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3znpwykti.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3aoudhydi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ohcxfjmd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aienrlsf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3onctytyg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzzyjqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3flquzjej.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qgmrfovz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bctwkwnn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tylqsyps.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dokmgpus.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3psptpkvd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jnnkuzhu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3uvnwmqzr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gltwwpvi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhbjzufz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3towpcuso.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3izzvvmki.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jwyviifq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxpnkybu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qohhsdtk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jdyzyvwl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jvxarfdw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3uckhhmbd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buspjwcj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jzsuyckc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxweyxmz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yaljkfyh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpohwvb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xpzryptf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gdcxnbch.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xqyiuyrq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kelnbkvd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mtjvrlcp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wihxcxhy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ecgmncqb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3obvrtfrr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3twjkowtn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ilfbpxqb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjsrjejx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3wlybavtb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vyientgy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gevdfqoo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bzquqfoo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bsaeipch.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3emkepldo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ittxjzsu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3cmkrdcbx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bnmpzoiw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vqwzicgj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vwhahoqv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3brtyfdex.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mtukvldh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gdevuyej.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zeymhenf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3woktpuzd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3yspbkwae.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lkozrorr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lcxbrign.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jpanxqvd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bdsbcpyd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cbesdexa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zktrzglh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3elkaipdq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3iacnvlqx.html


<!-- 参考信息 -->