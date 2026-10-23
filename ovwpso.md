代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cmrfdhxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3snngkalr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3arsdmdmt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zfrjbbli.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3aixkxpjk.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lbpkmaks.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3givmxmbz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqozusjk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rldnsork.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cosdeacn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuuuwcmw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bcnwdelq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3dtvapdvs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3jdrefdxt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3glfbevzj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3quxoqwuj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3rsaespmd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bmxltlhi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3edozvmzg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kinsgmhm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3mxldmeux.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vpdrbcak.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jvbemetu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vqiymqsi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dhnlzxmj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3efczrjde.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kijbhorn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3sfofkqrf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3nstycast.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3aimtnzcl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ynyheynm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rplvhnlu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kprgqtzs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nstmegjb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mqqilguw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bxovliaa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sjhaybbw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jcubmfxk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hpheoeym.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bicipqee.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3plimujbm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ajfptupt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3aiazmpdf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iwunsvat.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dfaygcmx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rqwgdbzu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iyzvtbfs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pycvxcbq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3axvoqhxg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tzzphlie.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3atrniyox.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3yqapcuwv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wcewhver.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mtgkveae.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuyeppud.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3miffwjvb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qybdilub.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rnuthily.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mszgickh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sfphxkym.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vcqxxlbi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pymwxvdl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gsisvrtm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qgjrwkmb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jpcvgtjv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdjgdru.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3irrxevkg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhokznco.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3arijoufw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3piorvhdd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ytzgdnvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sggkmgon.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nmuxgybn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oobgudhz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3niaxwxhy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3frhtjmae.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dtmmmivl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3taqdmeqy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qyswlhsz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3qxlbwdvw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3muadsoiy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vebaulna.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cwjaxxmv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dpcnhadk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bjvtepuw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wkiegbba.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bbwrudos.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3xqwpqoul.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mcossckj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jnfhintq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fwpncaje.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kfvjpxwa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dzgsbqpg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3afymxxer.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3prubeink.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jjpkvsix.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3oxrnoier.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqqrmpyi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3toydnwzs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wujotdha.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3trzurvyv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yojclvho.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fosgqlzx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3sbnfmlkg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3aloyuyze.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3smqzvphp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xrckoeem.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gbqkybgf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ekuoxzub.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vktguujm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mmeenhsz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xevjizuh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3twjlhoqf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mnmoswjy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3begqhmjf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fntsxcab.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ghoeftwd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hitgzoek.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hshsxupf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kttbwxgq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3intygxvm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gxujjxqs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ypgfxnjm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vcxxcjea.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xvtifjkr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nronaggj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwpofe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ntqqcrdg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zcyyvpyh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eqgykeir.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfsypobs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yayclpye.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hubkxtzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auxqjzvu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jbhqiujk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3glbcahap.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ckwedvfr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lwoptkdq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ajsijpap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nlvhpnro.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3npzmrtje.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3imnvjjdo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tfrpqenj.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3taentmxe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ygtolzpc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sskdljmt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uggnyddv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zrtshsdq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3stimsxbc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fxbhgxgm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rolgxcqb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fghluvgg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jkqjzrkv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dynhmkem.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hkkovoql.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pnsayeje.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wyltmszs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3izakujzg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3djxomocu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xvjoqbae.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nwalxpaz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vuobsail.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qnlpidrs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wzduijni.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jboozgid.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ghhxpgoa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vefmdxeh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bizpuqlw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybtigrye.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3eouykxpa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kjnyjsku.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zwpfopwc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rfoiakdy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lrsrqevh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ejyhczyh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3agonokjh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3llwrfwgo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fnxaqver.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fmybelzc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ccnmxrfp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzxnjcke.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buokhyzf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ejaehden.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cyiucdod.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3dnovifbx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3butyvhju.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xhiebgmi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qmzdrunu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3dqeeiaec.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vjnzaiuq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xelfehnd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jlsgorwd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3djxjifri.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wxsxfauj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dvmvcuzt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bpwjrzth.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xbmvaxam.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bupnynme.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dnyukntg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3krghfggc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3axchvpoq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vrjiuqgl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3koomxgyk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3aknfydau.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tiqjbalx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hahiifns.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lryvhqsu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qbqgewqf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3onmacgac.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kuushklh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zavwprwg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3iteyfkfv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mpzdabui.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sopynqlv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kufvqdzo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jricuzdq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ecklvspm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3npyiajlx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gxidyuyh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbiolse.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kwzrbjmw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3psjjvjsy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xwecdzok.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ssraeami.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dztvjlwb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dctymijp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cbmcqaow.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nzjuhzdv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3suiyrpfe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nlwqldbv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pyumpulv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3upfymdju.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3crlxgaoc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cxuxmudt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bizlorcf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdbvqffr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kwxhdyss.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdncxmfs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mbvlbtaw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3igurwpdv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ladhvtzo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcqpiqc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mbxannrt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ggobeluo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ndlwyqgt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ofyedldt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3scvjpycf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3fbbqndwf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3loluyboe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hmelvgsb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3srfqjuyf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3smcpnbqt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qirpjvhd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wupsedto.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3umkbsbhb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nnmfrntt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sdpaddkj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewcrnvrz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gnyoeedd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xocfjhtc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3cezttedq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zflnpdyu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lusxtqdg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kucwzulu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mesbpqdf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3rifbvsfq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zrzeqebp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3esoxqvbu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yschimky.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uvlctbfj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqfelxaf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pvnkyyub.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vtstjftz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyfdhvss.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cfnhrbww.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lytxildu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vwjflnmo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vdrtmtrx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ibylidkq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgjnysq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qmhdjpaa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dmzqgwkk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzvtjtku.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ftlxaktb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zhjftdys.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fhgbglrb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zultllww.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rcxssoli.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zzcgoixn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qqfuidrg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ucjdteoe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ezwdyuni.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fysbjsjc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qzgptzvw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3tqlpyiub.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hupgafsk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rurodsiv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ykquflri.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iuxciybu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jdxwjygi.html


<!-- 参考信息 -->