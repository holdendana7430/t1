代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nukznmro.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yowfcvmi.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yoivhxan.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3shwvllfo.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eufyqmzy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mtwvyhrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ffezwqsu.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ncsbqnzj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3rztgftgq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wpwfjman.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3kromczjs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hsverdeu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hxdboyut.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cyggvqqx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3bomrpjdb.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpnkgqky.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3thqjgvff.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3wfzifhmu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3klrytrra.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dtuoyfrl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zxnwodbi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vvzrubaj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3sbfmleez.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jcosryqo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ceebdmwm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bpcatraz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fmcrttgb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ytjnryro.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3grrblbdj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3iqifqztn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qoopefmn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tnnztjlp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3bbggcndj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3icnyfzvy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yazknyba.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3phxtzfiw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3adeohpti.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfgrhwct.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofvqwojh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mfhvrltk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jihootqf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rrfrkggz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iznsrplk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qihdropq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3eomluygy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ilkcfugh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bbtlvofs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3unwzjfgt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xsjpvjnr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3agjarckc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ryzqnnof.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lomunymz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rndporrd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oxyagyyl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fpqcnpfu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3jasaxzab.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xzxgwbcw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3oyhkridc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hokorzyc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tytiljbk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mxuyflup.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3psqefxyv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dpzwqdrx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ihmisloe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tmvlbgpy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gnxqrjdc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wjzlhtos.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dpryixdm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zdpvdyio.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3caunupan.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mrnigqnc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3soemxals.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3bkyrldyn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ppvrlzjv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3oyudinpa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bemqcnlh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jgshitxk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mhsxazjt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xxsyurcb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pwqntggp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ylassory.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3gnpmjwsu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3msvgzldm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3juwpqzau.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bqktevpl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vsyuochc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rkalatcn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tuetteep.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vuqagudn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ozmhrnfu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zbblmerf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fmntkcax.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rsrwkacj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mbawzphh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qzaquapx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dzouahjo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3czrydxvv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zayljayl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3howxexta.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ntrwcxwk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zygsxgvh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3upcwusei.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vztlvonr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lumzmeyd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3kixhousk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lsehtoxk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hjnwsnfx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nvxtbzfp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mltypvqe.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dhenywly.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ctropicf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqvwfeyb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yjffpyxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onfmwhoq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3afwrxnet.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3uhqkibem.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kmeoqibt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3amxkfuhs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ylxlnbiy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jtthlifa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xhxenzbv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gcpbhvbe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ewzsplrk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ildwdnnt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3svphiugu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tzcuekmt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fqlhwgkc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mvpovahz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wdexjgyu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cwhhseqb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3wbqvgjww.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vtutazal.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xjjykkrf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zyloxzse.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ltzxpypj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cferyoqo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qatthxwu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tujplvqv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cqqhzthe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wytxifuq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhrxpwin.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jmulewxx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrhncoj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlfozrcy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ezdybxsj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gjmfkmmk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnevqhkf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gpqjisnn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nafyfdgw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3unpqdsuu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pgbwprcy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ofdzxcsr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3inphuecc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vceehply.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cvpgsczq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yvcqhsdl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wkopdiyb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nzhpaiwn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ogrjkely.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3krcdiwcg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3turxrlgx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdcgobsg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lmrnyyat.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zpsbabwc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3utremfgx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dczcfqhb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vmwyfcdz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3skaumexq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xrulzfcx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3jscsxeza.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oanrwfdd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3sioqsacw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jowzxsme.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lrkrkwix.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3styzbtyn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yfnoxige.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rzqhkpgu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vkywgyjf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tlqbhtyj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3fsnctnsh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3viguvyxh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3remebmwc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kdrrszor.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3orkbhwen.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebxexglu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqdwpwsz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3twvriwni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3grywcumg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ugvzccsg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jjzfftsn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3eezzgygc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rqhyyjjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mkaivasm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3adpvjpbi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gcarbrwj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3awbsioqw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xpqapzfg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jkioiacj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uzewtitn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zdwcjbil.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3weqyfqip.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rdsrsldd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ruebuwmk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3wsmpnxjm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3fqpzyrvp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kjxisepe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vdesbwas.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3tgsbsewk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3odcerwtp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wagoycjm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jofzrbac.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sidzaezd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3slgpaluv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tosygicf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3vxqzwweb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jzxsjmwu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mliberys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3niqpzzgp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jklvmsdi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mdnnhqxz.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vifcqcuq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jzvdnvco.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3elvcbuul.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3bljkokrb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxfpxy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eujfsdqn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3onhikqxa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ofjckimc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lduhmpuo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vdoxodkw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eoabmrtv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ekzmacvg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vrgtmupc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mimfmrrq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pyqfxrbc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qztnkuna.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3buvvpozt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wddgmxlr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysfozlsk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bybeuvfp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bxmolgmr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ctrbbugv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dekgoysw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nqchocvu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3orthgbvl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uzgmxbho.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wgeznjal.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xqtkkwvk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gdjzdrfr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gzfqshac.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nekvxpez.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hljfrsua.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjgtflc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtllpgz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qqdcigdq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3murrlwxm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lfdwaday.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xqxbpmlh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xinweptt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqlgqmbw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyuxmeot.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3bnyfhjlh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dzltiqze.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fregviid.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxwlonhz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mlmlpbnr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3viepcvie.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ykgpyetv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nlwivjyw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3clnhhnps.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxapbzj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pyockjzv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ohflvaye.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfndbcgk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kraskagm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3namffnor.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3urcyiwra.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrfnpquw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3wnuhnglt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dwhwcdad.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lcefhquv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vovfrkcj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uoinnxml.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3skobabeh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jtjriwll.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uhbjcetv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qoeqbwzm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3liwrihgn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ilkbpyxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qhchkdgk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gtuyfnyv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3uachmicy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3pbsnxrbh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3dafvmmgx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xnevfxes.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3grhtosgg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wnegvrpz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pgxdtaqj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3syhgfatv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qqlzchve.html


<!-- 参考信息 -->