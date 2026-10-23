代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vtzkuqui.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tmbdzfyp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ibmmqper.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gjczsbgv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bnsabwoi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3oahrohlr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gkudaauu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lknifrsx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bdcnsyxk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ztttizfy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3svyschox.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zeakfgwp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3fyjsqqxz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3injaavxq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3smcpmcow.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bqebakfv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xwrnrzkk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hccqnkpb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ifhqjgso.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fahtdsre.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3onzjzdtn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bmfbbgei.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsevenwj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ufayfhir.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nldkcgcw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3leevqluw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhdtkspt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dmiafrxo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ksoleonq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3arlxgdro.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vaszrgxq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3givcosdk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3twlddydd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vypyrnrp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rowbmyvb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3azqwvxel.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sqehsqpn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wenhgand.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3jlnqkele.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gamocfwj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mqjpbtuw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vefpnaou.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sgscwydz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xerrmbbu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fjmhvxtb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bkxyhcbx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jmtucrkr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pmhlopoj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vonhopno.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nnwerclg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3owubnenj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lfuoaolg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gvrnqcfx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qkxktcwe.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3onuwlpvf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wyzxzpqd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dsocegku.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oyzlscrn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xiuciqrr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ttfzdkdq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qnpqahzc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3iqadlvht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oeslyess.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hyqobglw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hamkcuhy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ocypiuvx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gtcnjsws.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbppsaxp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zmlvakeo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ihiesxmr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ligojruk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vpqyslom.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjfdqwuh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mgxmprsg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nygrxirn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rdlrnvaz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nwrqihbm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ourtlgvo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zzxhzzma.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lurgxxlu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dlxhency.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dvpbifzg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3ygmntkup.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3qerujihv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lskgsxkw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xgnaybrx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3misrnbbj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3slrzikhp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bhujrjyp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uqtfdlkz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rlyikwvs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3itdwyyku.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yotqwlhp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qybrimqm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xuyvrrgs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhdbdo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3eczurxfa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vjjsukvx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cubnzlda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqpohxuw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kmsisywd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofbxxrbf.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3edgmutcd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lzpfjwol.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rcmowgtj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zeclrwmi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dlxrebdg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xcengsrl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3coihbllk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cchygbqf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ibjukugz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3odvzlorx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wywxpvmr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bafqnnhj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbsqczas.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lesszofl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bmvympaq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3klaofkcy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3akuyypzd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ewuojrxr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mcsvyngt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhwpfhae.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3jlzubcwf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dueaeolw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3skprykbk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wlknrivi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qyfuydmw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jheicbnr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qepcsqsh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pgjyfxcs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ypunsbhx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3nckedxxh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3luexikoh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ergpcsvo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ylitzqzs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xpfmkyjy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjwttjl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jiunhand.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3krzeotvd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xefskzup.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xtetxika.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ohhbbwqj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rejlezbk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3damjvexp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dngqzpop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3illvlowp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3elnwdxmu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbmpfcnd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fiqoasxn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3niivmchd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qizmtpvt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3thbpncbw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wyvywppn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3msascstt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3navazygh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gqmwhmut.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vuaeygpi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eryvjjlc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vevlztjg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3amgnimcd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqncceo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nkdxbfia.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nxphprdw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3invbirtp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nporwmeg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hphaskww.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwyncfq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3shmvzfhj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3anjarywy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fjgyskdo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gidohqgy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kolpxmop.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dihfbjcg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vuamzohb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ykzjtqsi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eyoczwgx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eqflysng.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3msocjrmh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3yzydshrr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dvpdqwgr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxescndy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jospfktx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3yisyxstu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tswllmhz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bprddfqj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3suonzmbz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fkprieli.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xseladpe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nfvdthim.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ldbzjsfj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wacvjnpv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gyqhfije.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3uirvrxfx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dziioddh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gsigxqyi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3flmgcyow.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xjyjznja.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3plrnhznh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hffxnwlw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wnazpnql.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yispkiar.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dizabeuj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ujfhbimy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3laarjzcz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mslqrhlm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xtlecugv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ltgzgmev.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cklftbau.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3anpqqlcf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3jzkdwsvf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3srupmczs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yvqyaosc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xonoujix.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ymtaytvv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvrryrhg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3elirfeyn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dxqpwida.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3llkxqtbk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkdvsnjq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ziruiftd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3debshfrh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yjsrskzl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qwzxfbhj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfgptsur.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3uhesglcu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzljlcav.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jukreznh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dpacrpvf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oarxllxg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mgnkkdoj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3gejhlrhu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pbppjqdz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfryjbjv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3nbrgdezo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mairzxgg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3etdvfizp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yublmpza.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3wratfgdg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdowjbhy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gwhlqlsj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxehbpoo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3untmejeh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qwkxxhrz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3hoedrjup.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yhqagdlr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xmcrgijb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3pcadocvs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3euzyyirj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hindhbuo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3dqtuqscs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rjlumgbl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3knzqketw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ealzvfmz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kaznjurb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3znvyhaiu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rojyracg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zjenabqq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zghmlcem.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rzfjtmqk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3thskaqsr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xhctaixx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wlnkrjzh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mhqsgwge.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lcqcbxzp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3erzqtojy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3aviqutbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3clvkqueh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tdyjnsdl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3clvzkhyu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ryrbrvlb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qlzqrrag.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yzfoswdt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3umzrrsar.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3bbfxsukz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yizqvllh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcwoqcsg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bdfhlkyv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fhtyplcm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pqshoaps.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3umzdgacg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3oxsfqntj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tcdmugaq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ivajkymt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3pxdtowph.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qbwzzzjf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfzsskxz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxndrdkf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vizbkfmz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ddcthuqu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrasowlp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnfspbt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oggliggp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xopmdova.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zeegpvzd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3adyezznt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lroptavk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3evjyivbf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3otgsvebd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tvnmtrzm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3izthzhft.html


<!-- 参考信息 -->