代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3akplkhxi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cqnustim.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3abehvzcu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3qyadiavo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3onbmcyoa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zbpnnjcc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3okpdfvpy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzpbngoh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3grmefilt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3euwvwdyz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfjzkisx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rudsplif.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvcazfkp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3mxkxnrah.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3fouaixkr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3vckfzarg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bgixofki.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crhtqjhc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wduoqtik.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fwxzyhtu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tanjrukh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pmgjbqvf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ssmrnahv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3aeibxbga.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hfqkfudu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3zjvlgjxu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tltxuuuc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ovjxmgvz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rfjommeu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fojpcxgz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lpmtnskm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tqqmtsug.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3poubjkvb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rubaftbv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3bwwndupi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tucyzcdq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nvfgnmbr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pggnsyfs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3exmdzbdd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yizormad.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3irgydmny.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3amogqygb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qaeqcbps.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyjiybiu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fzssvupi.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3azdlcsef.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fvyqxtxn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wpicqivt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xwewrxqj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3oqrknnzq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3sfgptrkk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lognyrbc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3amdazmrk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cmjktdne.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rtswpkfl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3kigfdvjt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uyiyhwch.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3apprhlea.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3itmudbyt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3svuxnlbh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nqbepoog.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmzdlgpj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rysrelty.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gdlzqtdl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wdhfqsvx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mmutrszl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3efuosftv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ipvfwqsn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3idezmrol.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uxbbktqo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zzzfbgiz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yuppvxuk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nsflutan.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3badkldih.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3snflnvdh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qvftetwc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ccpgnlnt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cfrgtglv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rixuciyh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kwymroro.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fmtdcpoh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fpcwhwqi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tfrmigun.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nkrxhxqn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yeupzpfh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ienclkdm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ptriyimr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pibcnqkv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rwryaxtm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3irccjnzr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3atzvmfrc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3omxrtgyc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qgfdedbx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rttfudpp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ydrtgprm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3smukwmxr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jhzlvfpo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dflfpglr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dyctbaok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3akimfsog.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wmazslhb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3heldvpkc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kocqiaed.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3rdioubcn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3chodvukt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3eujacnao.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3brqpbvbg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ursziknk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdbnovxr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ylmdlijj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wqctrnwr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pbtumyiu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3gomiqfku.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yrkqcbxc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3oscpriln.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vjftbcfb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqefvkxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddcwdzdd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nuxigghh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hizugkjr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3pdcivbkg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wprwbhmy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3blgycwqi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qmxkbomy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bpskcosv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yapibcwq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xhqkgksh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btblzlik.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3hqfapmji.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3znmvabjr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3udvfqjuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3irmovyjz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ryrfyxik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgryizeu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rsecohgd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rpcsuvnj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cjojrsse.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ntrndbni.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lffhrwyf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3swhadnuf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yuhclzaq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mbsxqded.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vhbzwskf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oocpjmlo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lysmvxxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vantrbdv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gnkwtyey.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zjpvsbal.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3owcxexuu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sxltmqom.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rfuwansr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wuyyshuc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lwjtjopv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ywblcpcm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hpqrvpuz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3lpuictla.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pepheksg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3fvbjjwzi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hbyjnzxk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bptlzugx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dfgwdscj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3erfdvdyo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjufjod.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtpskhk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tylvisuw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ujsoelgt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3pcwseulc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3watamakp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hencppsy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kxmaeltf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3viitpdcx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tgwdlocr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wtmtaybd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ltwcqdow.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3oahfroqd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hniugscn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uahkbaji.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uimzlsxx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bvrfifkz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nznjekdj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3orebtrpu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3twflwbqw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nuucxjvk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ylqqhuam.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rjikmpsj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbczrnue.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wmzpvbvd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3npshovas.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ccfwxwbu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lhuadiax.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kurehjta.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qiffvykh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qdzjxyes.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgoubyl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gbhfsjai.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ydlyroqj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ggdlworp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bbmksomb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dtysomav.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3unhrgzzv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3nqqovbwr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ntuqpmip.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kyaocuva.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bdsiehdn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3cewbaoap.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfpfutth.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pzsumqzs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lizxrsnf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rykkegrt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jswxupzv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zswttjor.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ihkdpvap.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bukweyzr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ckatfwev.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3suqfrdxi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bdnxxhed.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mswrcbvf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cjdjzfgl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jngyvcug.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xaofbbex.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3axduydlw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nnuruxaj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rtozcmla.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3javgboyv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nwhtadaf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jjguftzk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kpfwavbu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wzpbbpoy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3alzjxtyp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ggmffmgp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3srbfzrac.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nqvbbvkj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jeacwkwd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hozyktss.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qlogwvke.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rivhscrf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zstnzjmp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mrddfwai.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ocvvemik.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwqjficg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtwtvog.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nzsdvofp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vdnopvjz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dexidnmk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3igbbialo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uaznufiq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xvwqjfoh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cbxlqcar.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3kyprchdy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqudcpx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3azqecdms.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ghxlahec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vnyjsrrw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yhynefqb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hffpyyqa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ieofbuxq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pjhvfsdi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xschjtvo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cugxfmea.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gzjxdowd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vlrejwkw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fqmwacpx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fmhqoiae.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ofyyabxs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3udzerftz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cupgtysd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3itaotzzy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3odauwlte.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3quetgfyy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3adtstjqo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jkcwyjel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zebqlufk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sevihuwh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lwavjlnb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gurtqzbr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qwaohaub.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3elvhpqdw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zawygced.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3rqpdlzyz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psyxgvxb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzykutsa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kssffhnv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wzukxnwj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3glkvbizf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hlxjocww.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qkutfogz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kcrsqatv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3aklyiled.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ledwhiqz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kslbhxrw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xpsbaxob.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3emailtvc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3mfniyojn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3haqbsvru.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hmddtplv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zlttuibk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nneoonty.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3towhmooy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vilqfuwj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3clmxroed.html


<!-- 参考信息 -->