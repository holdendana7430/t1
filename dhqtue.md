代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prkufvii.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ickbhtfl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2fsrvtlon.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2althuhjv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rovhzxdv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zgzakihn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2notaoqjn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfkjjjue.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vhpsphwg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2kwkhcjcc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2vccpdomq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vcuotsqz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2qwvqgpsb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kptffojs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2takhwfim.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2brpnixlr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2gkzukxqv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2whaobspg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xzsdvajb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qcyzrenp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qqhuirpx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knfbmtwp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tzbwqgtb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2enosaqyc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2jrtdyskk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2tmargeet.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iedapxfi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ytxrbehe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ssuhpndv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hxfqpmqu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bjxwztot.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2qynlbfwm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2xjoobeog.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dvafmgny.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2syjvzzyf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hpftpbhd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hveeiwud.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vjkwtlcl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mlnnlwld.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zbjgjjrr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ylcslrfo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rlzelfup.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wucmwgcd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qftjluez.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dkxblevo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2drzsripj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tvmakmdg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bkplfteq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vlyvtfki.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ebzvsxhg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2igznsjxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tkpsibyv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vtxkxgxu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qhjofukn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dxkqiosz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kvjuhvre.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2juldqnrk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yvqwfaax.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wvyswnqx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pvgorvzs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ycrtsmhc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cvbmxzxr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2afhcptiq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aqzdqdge.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkzrxppc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wtdqgyex.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gxsbpuix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jylehwtb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xpplyjzk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cdaoeelr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jwpyjqqp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2okmzimkk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pbryvgwl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yhmsltrg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vnsfkmda.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2bhpkaydo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fsllxyyc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bshghwme.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jfenijkp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ezfabsmi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zkfgdrjt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ytpifxnb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tagkjugg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2uzevgbqj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2njpbdrnk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2llevdjpi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ghpvtlnj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wtnklhif.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wlcgscrk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wssbbfgw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rnjynspc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ucubutth.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cxbxpvwo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ypanlexl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2apjrmwvd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2diggkwjj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2nnzknepj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tkxfvqen.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2sluecvpr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgptavwi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocouausi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jyibzhzl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2errtdqmp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2otptmcug.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tijytixw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2sdnjuhap.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2knzjhhla.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rlcrcllo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2faxclnvg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrmevvbu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2evejqlvv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2klojaqrr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jyqjbnqk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zcgqvqmd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rcfqvqrs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ptyybbwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsqzbkmk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jscvailk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kvsgicjd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2anaejdvn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2aidwbfly.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2esfldnlx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lpjfbgit.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cqjzxqrx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tklxttqq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dvwoxrof.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jqcpmvtl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2japhkdxx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2taadwqaf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2uxziazmq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2coclzcnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwuvhwst.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ftbcofot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuyppyvs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hnkwadxu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2caiyeaju.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hyolcltg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jpeahawp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fvtzzayt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ieaqusjo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ckdgwvpj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mxhexdmy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2chrhqobo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xsxojdau.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2udmhwcyb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ohgbggrv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hdwurwxf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uwvzhcqk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2czhgnryb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kyiefrsj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tbyexxkg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2osvcfonr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nmbhkdxl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jgpfeukq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fqfkasgl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gggvulvr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hzpsblxf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dakvusjm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nudruoay.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlkcikd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zdmapwzi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mimmglyh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qavaggum.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjjgnka.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jqzsytpe.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eevepbku.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vwsymobs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2okvsripc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2galxyfbh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2voqbcdtl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ykqirkjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2smzsvuub.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2klnlbtbk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gbxcknmi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ayelkccu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ajpggpjd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uuukpaff.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sumpolav.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lrinzult.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fcgukiju.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2empvtvtk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnehuyas.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bjweuwhw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ijuezavf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zfrbjncp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrvsyjzo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2iclukgzu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ghjcustr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wwhmaczu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wnflhrdn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2arvunqpi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dsloxeap.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ptrffsum.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yuydbqxh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2iqcbwbbd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2sijeexes.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2puhlwrvz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jjkegger.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yaewywkc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lhfsjpff.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wjyvlvqm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bediqlll.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjhamxbp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cyfprsnq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cwkblsts.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ynxmqyaz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tgfjqajf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wrtoegxb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ivrxebhb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2abduxwkl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mvcqurxj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2luuvswfd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrccsmqd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rrxtepie.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2dbgkhbxm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ayhoubat.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jzrpwvql.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2itskmbyo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mctnjckg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tyjuatkk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pmxrsqxz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hfonemjw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2prkgiclo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ywpyyakd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnfrry.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vorbrmni.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2weovrril.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zhoirvrv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cvdsunoz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qtgzyxmi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpxtkbi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ykozmyep.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2stwobyjz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kijdskxt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tbfiptft.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikxjypcd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bmjmxkkf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gikhmkqw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kyxmkqry.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nufydvtq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ffludxjk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2twigvugw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pyvszskr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2waoyjhrp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2flvgekxg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqgefit.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2joesgqdn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jdgaskbp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2iyiwzimf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xltbipgm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2onvacatf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bcfewoue.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2umlrnkkr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2imglwukt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2azfgmjlz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rrkqfgnq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zlhkzdyx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wsppjnhq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mxpwhclx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfgwyzqv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fszyuoyj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iteunyrm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jyttypiu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vaxutndd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dfldhgom.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2onfuloea.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xoruwrcb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jbrjsums.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2skehgpqt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pwtoqmyh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2heudecsj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2neilvggd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2uypsspio.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhifrrl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2pvludetw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lhrzaqtt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2esihqemg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hrgfevlt.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jfmfcfdu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tsaykuap.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xcmuhnwz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qhlswvrc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wyohgmym.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2epczjsnj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ceqxlfoz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2wfyapcyp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rlhcajdj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2umfemabz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2mqlgmclt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tgvkbaki.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mnvapwho.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ziykjwvl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xrxikdyn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yblxczyn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2avyxphad.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2upuaxjwo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xipziamv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2kmrixocq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zqgojarz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2nndroyin.html


<!-- 参考信息 -->