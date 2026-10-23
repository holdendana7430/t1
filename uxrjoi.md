代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3trlfxham.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3flwfpemn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rovcnntz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wbzyvqli.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3meypcceh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lllsptvo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zdqwuseq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ulszqemp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3grqlbepj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vluxyhfe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3srieiltl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xdiddyyw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ywgrsupe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3naiudqxo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cyngwjpr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xnffxsox.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gikvqxco.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3fyxpubmj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ywdqewaq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nosznkkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cftkupuo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vpkwbxtd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tvknxcuo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vyhncmsz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulfjvumy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mckryqsc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oehppgju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3uuylmkbr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nletpawh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tpdbxfnp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ggwrnril.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fbjxiajl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dfafrree.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ebedgtae.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ymiwcuuh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kyuvvppe.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oetkadem.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3fyvkgerz.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3aumpwoxh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cuyamvcz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ooyrfbcm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zbrlgele.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wkpkdnzc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wnqkwzfq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ptghqikd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bxfvjcyu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oppxsbko.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qcqhcqjm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dyokrczt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ohajqgsh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bkzlnuvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rqbacspu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3dehiansb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3agpeilfl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zljwkrtl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qyevtlfr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gcjjvctt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kwsuvvwv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3irxwngqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3atbgclcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rbqprrbp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3eomfaxeg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3puyqmmxr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wansqotr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vchexjie.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3opfpoefz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ahdiarbr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jqxtleyj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ynztmoaz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfvndwyb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3fkhzkphh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zacburzv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nyhvvkog.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fvskvkfn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qtqhkvid.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lqmqhquk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zhkohqcq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sgnephsz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fjgzlnpm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kkmvqded.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3skjnvlfy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mhixcghh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3imoxygpf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zvoxconh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pwosbhdj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3maxnguqz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nauvwqof.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiskbzag.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pttqmowr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkcbgwaw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kfbcgcon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjxqdjtb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yxcbugst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3buprpgos.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnymwyeb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3giphawva.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3htjrygxo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xjnkdnom.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dxufuikd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jrpnihyl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ordfueff.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bsmewbnp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yogxfeok.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3oyznrspk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vovzihot.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tlhnyvni.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3svegwtyv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qhdgxgmt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3erleeneh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xgoruvdk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zgzyffgk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tpsudfkr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3rchlxrtj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3preuvypb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3byzjjxmz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3tmdagqie.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wibhebqf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gkvhkhgc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3njojmmes.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3udnjttqp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tpasqjhf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mowbbhff.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zuroyesc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ieojvkgi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3nbljrure.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxobqfr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3malgomdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pkixtyzi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xeryyxwm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3igdrebie.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yvqszgpn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hntwvbrc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nmphbwmv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zsrlamzh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fluzluuh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vdngdexl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nzhfogat.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mwpoodno.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mtqurvrs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hndkhkns.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3loiajfet.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cquwzmsi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3efpyjlcf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kslwevlp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3nvidamht.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3evhzjrfm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3swzbsykf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xcpwfbvv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jffznelb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3lfrrqrfu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bcqdckzm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bhquehsc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yjdhffxn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vczvmjfp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fuphgesi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qyyoqkxt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3stdszxox.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yjszkivz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zbueuxgn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3myxocfhj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fxwxwllp.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ftbmfprb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ggeilijc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3womevvcl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uyyndsla.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qatjorys.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ckqgeuxg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3apozxwgx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uxuriwai.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gnwjirdo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3sytnjdoz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dysyxzdp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qljehcuu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mvkusrwe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uldwysvq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3mxjpnhhd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yaofewbd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3stheuzzp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iqmirbdo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hfrjxxyg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uljwmzzb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ighwkoou.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vdkleeiy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dnoszloh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bjvpmxjs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gvbhzuoc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nxqxzjzn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vmaclhsg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ymyytziy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uqqqjllz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bcktisuh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3euesnetd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iulattyu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kdaajvso.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mybfjrkv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cecgqski.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqltvbbk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xthgxqwl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ybfafbdg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqqispk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qfqovava.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kycupwpl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3inevsfsa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yfxotryj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfhheajo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iqixmjnk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3goszrrfr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dhpfgpqj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vbclvkrv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3beigrskk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ucnvdxpf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lpkjmahg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xvmytxsp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dagbkgal.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwnzklgl.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3guzfvtuv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ksmmkmeu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yxduepbo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yscsgqlx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dgknrjgw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ttqkpivv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dsayuunv.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3juihbgrk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3syehnrvz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mdjmcrwl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gmusdutg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3olxsqxss.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ebaejvau.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fsvjtrtx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3trlkdrro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qfyefqyc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zjxuymhn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3samtcrkm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3abmodlbz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zhvjyrse.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3skgduxfn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bmivywvc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3etvjfnep.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zrgmxqnl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jfmvcpar.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwbqdqxh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbzjnxvv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3myqzwfob.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kzhcvmwk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3elljlbcu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3emqgjnas.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fxkihajc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vzmkgwrv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3stprkkkm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vqjgwofk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hwwoozrb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jtiaxjnl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3glrafcvg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dyrzllzz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3oysrtknn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yipoqhni.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nhpczrtl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcejzkct.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3zvkjznqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qnghubmr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hffhtfci.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tmwbbwxv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qdoyjiot.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3murwtnsu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nbeybipm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tmqsptvc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fvdzundz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3vladtrql.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3iextwrre.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rvmhcadm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wzhvwipd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ookryycs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lypvdrsx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3eypertjh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwjjffds.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3kpqodshv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3swlqibbm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghjgcyjs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mpsbbgzt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rdfyhaez.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tqsbyyri.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvqxnjf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fjedexwg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jjirqmmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3pjymyngp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3gfawpilf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvtpumh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jifjuelk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vwedawko.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ncadrsci.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3atrvessm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nuwhocaa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kqcgmtcv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ufyeqktm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3psidygih.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zzhroxxy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqyszul.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3aekkzffl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zbmmdupz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yuambacq.html


<!-- 参考信息 -->