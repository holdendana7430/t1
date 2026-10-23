代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dvuzxjtl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qjgycbpc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pmovbbrl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zisiiahj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3uosozxst.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3jehjafzf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ehkbmzmm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pnmdgjeg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzvwspg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vexlqabu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3xwjjmmud.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mlpswkdr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3hljoiveu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qwpfyjrm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebioffcd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rjxodozq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3rdeqzmlr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsjrnwoi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmymccy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mmjsjhsh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bntgftxt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tsmkvqnm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xbbfwfdc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zaobbnzu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3oegxwjbn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3soquxalt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdadplkb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zabmbzrm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qpkmcyol.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ndaihfgc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vogvaach.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3uqovaqon.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ifmxybao.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cupaomuw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ofuhesuy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cpknkczj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3loexauxx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uexqdzzu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3zxxjgwrj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qhyxgtuj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3slhnzxki.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kcgxwwnj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3yimzqdhy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3oqvjwdvn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mqlnaist.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kkxqqlbr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ibwyjzcw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3occwhoxc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xkkdnkgi.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rukexrby.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tufhgedn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3sdwxsxuw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hiqujzua.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vzgxqerd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rctyldja.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3rcsbmnfb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jgfurxvk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nsrdspdo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zfnllwax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrrdekgz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yftabdhs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dncqabnl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lcqntlug.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qisqeplk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zogbqlts.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3juouumvm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qccviyty.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3chkqaduv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3emibraxq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqwzverr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3czndhdfv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3keuzzdir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3psmbqnfb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ysdfedmm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3udhixpiq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sahrlmch.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmxozymr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cpdzulhh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3reukvvfa.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sucyjloc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vvbzrxxf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xqfwffyn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3swqwxspk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jywloijq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ffbeetrd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lpkrznji.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3oonnqcgv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbwyllub.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wzqrsgjt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3wcowoxmg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bnraolhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acxuexkb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3suohzhdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uswnobje.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3anjxvbbo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cafyobeo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sgdrezjg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wqvwfdkd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jatrlqlh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3eelssgkl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3szhilpwm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3qypgeljq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wirhwtqf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3julfjndv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cqugaemz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wlnatqel.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3myrfuxjg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zmfmfyyv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wquuuaqb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tucuijty.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jrzftobz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uuvdihup.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tqmsfbed.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqnblkzr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3cqkzkobg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fookzqym.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3osmejczd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gkiudzii.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3okamwrce.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fhssjyfa.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nkqqnkod.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3uthnbedc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fqepcfzc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lhsjakoj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3eowbtyqp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fjwydkse.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qlhbhysj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3izwtbjos.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3pmcuezlq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qltgbwne.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ffsishxh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cxanhxlf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wljyxrcx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nmcbateg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3cettdhqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3aylevmyl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bkkhqplg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dvehpkqz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3djlutnmb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3baleflzx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzxvpaur.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evmchzei.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kmyqsylu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fjtcndtk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ovjcnurn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qrpqkpjj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tiflsiyv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3hjwtyiwt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pbjjeccx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3nibusssm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qhhgnqrk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uicitifx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3epjcduzd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ygbscuxs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3klruaaup.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eiiabjaf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ovrapdig.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wxonzpmd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3uixngwqn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3rueyuvgy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gxbicxzy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3obeeoqsr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kznvvhjl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgsaebf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvwdgor.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bdoccacz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gbzxrcva.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nfjnhqae.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rvorfugt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hyfvxmgw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3bnkziaci.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jbtlmeey.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3arpucnjw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nbgdfeyn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lnlqytdy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xfpqmnlb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3upnmhnjl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lczfghbl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ckpgxuhk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iqwuebyd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dwwrivwc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3whxfjacc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mzdtspyk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kemcvfst.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jvyghqoj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jytkpmiz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gnfkcqdz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3vrjdjmva.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rnrlefbu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ewhewcyo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3usihpizo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ebwjtyar.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qivtnxgh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3geyeorol.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3kxqzmskb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sepgxqqb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sflqgrtl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3setetqjy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pcqrwpib.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fjhuiyjc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3orxtfazb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3mnyoredl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bpcjmilv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mgdpfjge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kszubvlr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3soilfsiy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fpkljozl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hzxcdwmr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vjoqppgk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uojnhwdo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezvaonfm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3xggchbjx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xocjydto.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3unqwrxod.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxvtwjpa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbuxadmu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvkclxit.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pfvwcxyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ebpeauch.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hhgcllpy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bcaptpvn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iisjgtoq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ivokvrhr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jthnyoym.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kwodnkpt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bepeadbq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ayrytffa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rglqjlrq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvsmahtg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ybyckldl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wjagdwks.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvamutmb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xcvbupua.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yartlhgh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bvethhif.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3pulhzdaw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fxirsuci.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3eatgszfs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3czaieavk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtwlkbjv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3urwuzlav.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qlrfudhx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sdfomjau.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nbaqdqjy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eszutilp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zoicaesn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ozwavxbe.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3dmzznzeu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rckyhwtx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tdjavonc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fwdrmltg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3nlaaqkdu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3dmcouajm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qofalokd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gvjgvuyv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3psnotyus.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3boxugkzo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mhnrrwrm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3cptysxzb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3yvmlobqh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zrpspwca.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yoqppmco.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yrjobaij.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dvucsvxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3scwztoei.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hctgiclv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnyhrsul.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3snvwphuu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ydzinbyi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fmwwxqws.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jkvkjdfy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3nckcuzam.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3kmbgmrsp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zxpbvqcs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3betufbzu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3itqkdvfi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbbcirj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3marlrlxa.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqqmoizj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbieikdl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmmjexke.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3djnpgsjg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zjddjbyn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mbainopn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3njwusopz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pkhzpoyd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3icrhpeme.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jujgrsyg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wjwtxljh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mypjkkaa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ypppnfmk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dkngxrnt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fsbqdnzk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gwynprcl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tlzdtkbz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3upspqoom.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fulxfxkg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3trtuyuja.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3exigtcnk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rqrnkksy.html


<!-- 参考信息 -->