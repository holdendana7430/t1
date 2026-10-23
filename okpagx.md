代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwlntkyn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3juuzampf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dycwdvnk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hrbdbmxo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3trtjqryu.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3golnjlsi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3lyuaifzb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3avwsqmfb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fshkbjef.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fazunmir.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bnbunnox.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rhodkbfk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3acajbppb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3sgqkrvvj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3rvxawgxz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3favfiydd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vrrelpsq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pqcxdioe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gxmmjmph.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wgqlfxkb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3asjlumii.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xebbvuko.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jhmkoaan.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3jdpadwwc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mmhwgwde.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hdathqkj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3kdrngdit.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3djuikibc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3eatreioj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dteqvfds.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eubnltpe.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ihlyxbpf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bmouyzxd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3vsolvpce.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dcjqqzyk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oepxjwkq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ueadzros.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kuywhakf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vzpkgiuv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3poxhayzk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yntsfbnk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xtbwpcla.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3oywcwjjq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vbqkyljw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fihmsxvs.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3prdrixvb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3faiqwbdv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3rwlpqrmu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3trbhcxtv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fqjivxgj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gfhbcdtp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mobdddko.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3knytquvd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwlegrxv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rxewbkzg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3epjuytnl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnmgcds.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ligrhzqm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3puzugpti.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3qncyujxx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3irnzmaot.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lrwpkypo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3brklhgib.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jrzahjgt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ioijukhl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3bnfuroxq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxvqbqsx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jccztjso.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3aqxrgfbo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qlcdcqud.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sluilxje.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qjaanboh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jhjiabsz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lqrpwcvs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aivcdirr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3axepzmtf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fuxayeqq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3kjmvbxow.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rwiwtjph.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tylakzgi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vrjvuith.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qbmghfqg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zmovhmgh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qapgctxs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3hgtradtj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wwnazlku.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3erjtslge.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ikctikko.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dducuzke.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3veamtxoz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3exrphdxk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qbvtqfzw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lhckddgo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3roqafkqv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3scsfntji.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3iydkwhce.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3endqciox.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ybwxsyhy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3iuiufzbi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejusksat.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3obxozpwo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mapmjpuv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3nsweseot.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qwvthkiz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sugpgfig.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ynjtqyct.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gymshvch.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vsmwhamx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nmckiyqh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cecnicbs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qcqaylzz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uvvgxtur.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3njxryamg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gcokuujl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ycbjslqb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3abrbwfbq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znsdjkzm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdumuohe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mvhuyfpr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oenrtgcz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3bggwidsp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kwwtlcbk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gypgpeze.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dpfbgros.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wbygflfs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pjuhaunv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xhpytqew.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ywjqtwbi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ryetlvgi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3avatcdhu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ewyvyjqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sobpympc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xjfzfray.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihswjlsc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3xxyvblny.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mnawshlk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yonjkzss.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3enhkkwtm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kdzutvlt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qxexqlza.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3oeanqtko.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dnzumfuz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3leotcook.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3awkftpsc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3luurjtss.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jqbrfkwq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3erohgysj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sdbbokiu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ddpjgqdh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jmtlrxzi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kjorggfo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gqhftteg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aqpvchlo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gnavtqsd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3htpfozei.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zquaujiq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rwgvdpck.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ubzymfgy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3xpsrvoxs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tteabgzp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cihyeare.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vdunbris.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3opgrnftv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vneosfox.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rmfpgrhk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zkuaxqhh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3krvmxzgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xdheaate.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3isrdjgmr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cwsaelow.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dkezeazg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wspyasbp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mzwslyzc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ihqtkdff.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3esyrpnay.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3thwrupeq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vygyjiao.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3klubmbrk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zlksxgav.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uqrycqtp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fyiftwxn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rztmyezw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ebvxfjiq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gudfjdfb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3uekoqbbs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xqrdkbce.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3riqmuytd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3guzyrjde.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3merkvmfu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wrphxjrq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rrsjigba.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3myqsjifu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cvjjibln.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xnerqwiu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jlcokcdd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3efzeyydt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vovsesus.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hlccpgux.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3byygewos.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bjmsxhuc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xlafmymm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3beououao.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hxsupjmu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wnmqnnut.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3aoxqwgdf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jcrirpyn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fcmnayox.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vaaiisuj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kpeyvezf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tbvxnfkj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ovopsbpi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3pgfhngwx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcsqjzu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3huqvzpkn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ryjicqnl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vuqgdohc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kxdbdjhb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3svozjgle.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3demewbti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mqomjzly.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vsoxrgrx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3pfbjmaxp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3qtccbadj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3meyviner.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nxcsstui.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mpcyslae.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hlqhywfk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kqkpmwyx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3chiyervs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3codddxhh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fevubiwu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3igckmntl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3itsdrdnd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3gpmpjwes.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dzldjjgl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3miqvehhf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dkdatwkw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3raulgkcp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3uwpauroh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyfruayy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xiucjnmk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nhalxisz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ytrtyfha.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3oknjjenb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zqtisdvn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uewlwpbj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fkocwfuu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tnsymcro.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mdgpqyno.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtusctg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3knqbzmnf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pdghenpt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zgmufgni.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jdeulygh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gobnppva.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nmytatxk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lcwghsxu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bijwwvht.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vkwbedmw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lgpkruzq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3snscgdtc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ebdmbypj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qunamise.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ujhlamua.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mxtkzxyt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jrejpjdb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vrazfdlt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zvclxmfn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3twfqxzmh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lrszajqr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhtboykm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qyzrzzyt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wmhwcdgk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bbxqejcm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wlwmckqh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3sxodvhrr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3onvsunnf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dwwyuxjh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ngphutmu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rifzokcq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gqjpmtdu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbdtkxy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pvenbcam.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xorqobdk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhjropey.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3eszifhtg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xkkwfwdx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3srftybsn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3wozanlrl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mxangegu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kfegrlhs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ifugoxzj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opnznlhb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dtdztuxn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gkuteder.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mclmehwl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ghkgutci.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zzgwaskc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fpjrqhov.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qwgpqzmr.html


<!-- 参考信息 -->