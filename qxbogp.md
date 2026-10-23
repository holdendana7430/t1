代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufgyxiiz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3epfewcvp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lixepteh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mvzbjsnb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhvnzqlk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mrotljwi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdkzhwgn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxctwvl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrbwrlqn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3agqgkibs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bcgbdzqm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3tcqqdywc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3speqwdbe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nmuyjsrm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3hybpuckv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3iynhiyis.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yttdbimw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhwxpnpn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ydcdzxrq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mewyandv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tyhckkee.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3wkhpbbyp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3onzfrqcb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vzzgglhp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bfmloghu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mckeeqvd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aqmijtdz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3tubbofnx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfwvkruf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhufwryv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqxcpivw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dmukgoxm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jpxjgpyi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wxmiofsr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3iqgxnlln.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3npqziwjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3inqacqgj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oqwqznol.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lfgswzpb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3phjdfypm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ubwzmbbw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kqktwrzw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ggyobskh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3whkljnln.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tolqdmvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iinvhged.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oeybtcnr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gkpiconp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3owjnkpdo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3drbjaknz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fdtknxcp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hawfrhof.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xhlakurg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3oppinibb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3epgqnrid.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3axavvyno.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dtiyzazc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bdcmwdty.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gvgdfsxl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tkmuxdrq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3upxcskgz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwkksyiu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bctfpswv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3asnnwcbw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3fqkhsiqp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3usjibpyb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwutoofv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xsujzeeh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xkdwypyb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3stmwkmzg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mfjklzgq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3avsnxxmm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrifykcc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nxnpstjv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yhgemfvz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dynpaiwo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rwqwwxnm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3naehvgfw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gswvqcoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xejzppas.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3futgsqiq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pfbjuizt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3poffxpms.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rsefkcvb.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fecpbwmv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3agvpmbjq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ciicmhrz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tjivdkvv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zolhsjkh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vyokatzg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fpwkwcvw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xomknjig.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gptxtbtk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ecskzpbg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3xzgodhvx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mbeqqtfw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xareljhx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vmxxwlax.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ricfpsvu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3enszkwgj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pswnwnmt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nligypka.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gcbrxggk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3miofvani.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rtplexzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbjowjcd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3fvrsltqj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3liloflcp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytzwrvrp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fhacqnfb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3cepxypty.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kogbhhzp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wveppgdz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qzhmcghj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bxvpfhtq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qvqswjuf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwplocbh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3buqycdlk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3iamtyono.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zadjhhfp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3eewuqsnj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3phjaoflt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ozmqzxyk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dlqusckd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbchfuhi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tfzzaspj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uidplizg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3glenhknr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3haxkodtb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ynmweobr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zmnawysm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zuthttbl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3goavdpvu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ujcsepdh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kglpoobl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbiplbmy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qbamymlr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3spwsfshh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3svpjfdsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgytypko.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dmkrwgqs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbojsyhz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3alewzdiv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fnraqawp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xvzeitrz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3svndqcqi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lhnmkhrh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xwtgrmpf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xvwwbdyj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ituxefjw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3doxrylaw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3auptdyyj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xbgjejgb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nahvallk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3aeubxcbm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3muapgcla.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dinurwtg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlijkdmh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3exeahkxm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vadvwfvt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lsvwnnco.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozafngns.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3irbunasf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fgclrcld.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tpksaygo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dglokllc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3krzydrwg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pheqifaz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3edteeuif.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zxzoiqhm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajstykly.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqqgbxvl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3anzcbeom.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3nedidawy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lhdybsyo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lgoetbyi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkgrioiv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3hbiaaigq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3urbpqsxg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zbudxaxz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iuvkupbb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ppumgaqb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qswdopdy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3zvgpadaw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3evjgatjw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3blvrfmys.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wbercrly.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mwigtdye.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3klodubgu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ugrcgcer.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nyuzirfc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ygnvzjja.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cximovys.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uyecbbxc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3kmnjgbha.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jidpviwz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gwfygrrh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yrlackca.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xxdruhmp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uwbubfyb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqgupuj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3huwjndil.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lukveqii.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fycfxnkd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vlanfvgc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zfgsczit.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jmnjguej.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vdfppxlj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wuysfnim.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3nllhtzql.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3znxcqenu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sbmnbnih.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dquafirt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3smcmubco.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3uiddahlp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ccluwsoy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dolhduvu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3dqtdwgnl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dvlusrid.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qbbakcqi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lbmmrnmu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mnuavxac.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hlluujwc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tcpytoyr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qoqobteq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3utpxxelm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3afcwwgoi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3shchgatt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nfujbgga.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xkqeakgd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qkemcbts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dlvgujgt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jvivwkqv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jnpqjfsw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mqxpxhhb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vulxugft.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wjmvqtge.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rnowrvax.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfjzcjjm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dwxoeryj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mnxowjcv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zkqmnxwf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rbnhltbd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kfjjeefp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qpvvcado.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tjymyvbd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3vqvrtgvi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkstjqfq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyitqvmu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qzxplfvx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fckkuokz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3emjuyaup.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jfgrjbug.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wxttmqhf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vaebvrrn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bakzvjdf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wqlqbvqh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mirxzzfb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bqpmbrku.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3whlzssbh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xwwkmhzh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3brbdcvji.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lljobnvh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gbkfwkfm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqttzeao.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lffrbtws.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3eobjnouc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfqtibwn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ayzhbneh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ylmvdaqs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gcsmwsrz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tlynxvjp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jcfymust.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ozdzsrgr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3uvnxwuoz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tqfpmjfk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zhitdwbg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3nlqhzebp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcoplzge.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eugsvukg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3shriwktk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojsrrvfl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bijwwmth.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3npeazroa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xevpzljm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3foqklytf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kppilnwx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jvqzbqqk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vyluumpp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwngnif.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hveminyl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kyuvgodm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fjsjbuks.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uppreylf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cyjrrjic.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qicgrlne.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hgyahdyf.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3omnbdcgu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ihncrxfb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tvckvujb.html


<!-- 参考信息 -->