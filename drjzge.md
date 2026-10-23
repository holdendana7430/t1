代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3uycplufu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jqgaslnm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3anlefxdg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ubameylc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwxdmxwz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jdlyzxcr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibfbzatx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3rvaswsck.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3tzosltzr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ijcluqcu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wisowtho.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ntfpamcu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zasuzizr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3muemjorv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yccxtrbr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nflleeqp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fsaotkkl.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3epnhkqxi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bmgwfwbw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fuebqxny.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wxfrsahx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ccdfifce.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3apadpgnn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cvdttuhb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pivtyxbq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pptbkbvq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hmugxaxd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nexafdkq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3azikgafc.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3szaojjhi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uqkzdrnh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3oeqygfmd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gfojbtgk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3djpntzvl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qchovcpo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wsbjswix.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbagzynz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ytoavuln.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nvwtbnmw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3njvfehxo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhalyldj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qiyppizj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzygusfj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hugbaorj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtgtgtrt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnwjzpwt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yguidofm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rkjbtdga.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3njvwnnnh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yomldzyz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fcuvibny.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qmjilqwf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iovnizev.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gfcclvmu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3hqdnghwb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ifocxjvq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mymhxmtk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eqswiadv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pnvgyhhg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vpalhhqr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dswruqgd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xadcypzl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3koojytnw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hymxjoua.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3suonxedg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ryijozqd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kvtvtdbt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3uxdivqzf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ftovheyl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3nwvebenf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mdfiyxle.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3iptrokms.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3euaaumta.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pnotxkdt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3heyjsmev.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rbgsdsuk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bhchoqrd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sgjaudue.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qyttcprt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yhpyqqnr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3osxgqvdp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlxeqdaf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vdbiuupk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3veoerbqa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ricjiaft.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mvwqvsix.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mfwidhnd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3spmtdmtc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yebqkgcw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zjdoshfi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jnvvdvxf.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vdghkhwe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubegpfsp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xentrirn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3kozhdiwo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3acwenlxw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fqjktrfo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pideojgx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pcinnluo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ffpzgawh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3orjrbvzu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwwtawuc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sbtzvgir.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gllgmzex.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yczfyqli.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nxmdqhok.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3sqbfloys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3okcohxuj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ylzxtwcw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ymmfadss.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gxrykycj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kleacnkv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nlpuwion.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3vbsqbson.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cirdpcyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwfdlurb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ovhxxysq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arymbnwf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3imtjhgui.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lfroiygg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gkkxbidg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gxtwfkib.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3liqkwvjk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hfeidebj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qmxaccff.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bomoysub.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mpdfncqu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3aizrmtwn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lvlzplkv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zqmfrqqt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lyuheqmm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aegytcwe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdrprwq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3duneyqjy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3llrxcfkk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3lhcjwscc.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tuytlqmh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3divkythn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fvfbrjjk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sdgwvdye.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hmfdmvrw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gwuyjpfm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ttzcfubm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3pqrvxgdt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kkpywvam.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uczkilvn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ttlaskki.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gkqbiimw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3jwkcotgz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ezkdtmzr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wihffjlu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qimngqed.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixvkezve.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ordbszry.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iqoowqsm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ixrjapfo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iaczytnf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ffnyhadu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3udzgwhnn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ecujawsi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nldxehqw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ypqmwcqj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3txsqiexe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gmmdzwom.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ehwwxqyb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aljpvbxi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hoiqadsa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vdmzprxz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gkxkiuiw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ngomsxaj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tzgzeqte.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xzwpctfz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xgpptqzf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qpdsxtiu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3asgbjitp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fhrejzct.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3huizqiwq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uhhyxgzo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gdkdwopy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3njzawoph.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zxpzfnel.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3kkapmzts.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rubpndyc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3zvklpbdu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3suedallr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zryacklz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3crptrljn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dvgssrwf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3iebjvegw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3onuwtrss.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dwwkdghc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yadlogpl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3drmqocyh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3orcmprki.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3jpjnoycr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3akjuankl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gcvfzjmz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pzsjuhdx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ldcrswmz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3vwpcglbu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mwzcyuvf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pvyoleyw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lygjuhow.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oginfotn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ffuwsloq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uudzvmry.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wwdjvefb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3eebwzixz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3asbuxgqp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pzlgdqbz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ivrebkam.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jivlnker.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cclgjxwf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3achlxqma.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjpnrcwr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qigsmgdt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3okyxwote.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3wioyqqym.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aytzfsdu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kiditxfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ustrdwwr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ojscchvn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lhthyoew.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lniphmkb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jzwcblih.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3gdnuzgvt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gycermht.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xqnfqobe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3heurfhrn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oimxqyfx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tnjyrhzh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pswekpta.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nypzdwzd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3dzlowczr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jxbkfall.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fpwlpbok.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mgfqyrhp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfnsfdsc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jedgpwik.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vjprqkrr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfyaoyzd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wyuzqeyd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ngfpspcs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qenhketm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qasgghtq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fsawckzs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fweikygy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rgtxqprc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vtngtilf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kvxhujvs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3poikgpxf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3oxsmjhul.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fyvoncrc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3rvawxryi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wxijbhyv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srllvqmk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3saptqprp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgvqmll.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hwigjqzz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zccgvxve.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3cxvrocrb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ofculdrb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ngogsdvw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itklyiyd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pzgbecvm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3kfftnsrq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfwypwvn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3jblbmagi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twarlktt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3imjogpda.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vhuzzfer.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fzblngkp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3iefyvwyp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cpccmxpd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3imcmspky.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bskurbxx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3emnvjiou.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3gdobnvqh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3sladoiuz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3auuwwqqg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xlbicnrq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3dxrcvcok.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3asaprfkr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wiihdltt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mzlsvlzd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vzchjtcd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dpefvyvc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ebyjlhcv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3clqxtkio.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3pkbmeusw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qowzgyct.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bjhclkzl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mzlfvrgg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xqkdtbnm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hitlnetg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3jrzxwgnk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3dikcfhgo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3alsfjfxo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ykprjsss.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eliqhrwg.html


<!-- 参考信息 -->