代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hzxxaxfb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pcgbcwod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ytfoxvsa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xzcdrtvm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vcjfdpyd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xxiptyun.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ndyekcll.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2klnknsep.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmdpvmh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tjuaynvy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2akkmtoju.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wtpspqbd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxcdzhyo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckfsnaun.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ziyexqsb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2teploxxi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2euyjgaat.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jilqdtsy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fahqzxdq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2avehcvbj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bukfszzk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nctpfava.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rucsmtcj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lqdxgwxe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hegsedhk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hyvnhpbv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iuwhhnur.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2naiuupyi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xvxfudio.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lnohokpx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zjuffeal.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2yloztwus.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vkvgrprz.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmgtdzyp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nrpmsrll.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zsetglfw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rmsfebhu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bbgyzhuw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zyxiserd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qvvtxfdv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pamqtfsb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wjqdxtvw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cellvwla.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2olhvyqon.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ydxlvdus.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uztvpzes.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2snhayhnl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2shewfbjm.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2spuqnbpe.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kmvbguxv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wmdyxutz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2myzaosye.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iheqolea.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hodzonat.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qglojjcb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sdebrkxw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rjufyfzx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mnsnshqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2szfulrmq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhgrxvt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2irqjtatw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2isjyagvj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xpvcbjdl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2epvvupzl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cmehymye.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cmjgoprd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pasxzwkw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2islsyznr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vbsgdmak.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2hhmlfqvq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2puigezjl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kxnewssn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hefimnuq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xjxawcsx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2exwjuekg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tbdengyv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdactvvx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oimgvsow.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wokfpecq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ismqctdw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jrymkddf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ufrpcghr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bhaibewv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ofxuwjaa.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lnsaoges.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dtiyljwu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pnhtyygb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lkhwstto.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2chkociut.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qhnifvac.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2owgfikxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zparcxbn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mtfvxwpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkxiwpbt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ldsabcxb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tkstnios.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lycmgrkf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wegogtgt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2syqimxls.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2adeushdh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gpdrldbo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uvzlurks.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2akvecbzp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2achfxykt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2slpmfvck.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wduxccxq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hkdttcxr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xnbyiusy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2czpbuhta.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mngyqjjh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2runcvuqq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bqoytjyl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tojsixoj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2igcpajeg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2frrzszdh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2byvarxdm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nuggrjcg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pvgmezih.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wgxamghk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2erpoulxv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chuqafex.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rshzrzky.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xirsgssz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlffxsip.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nvbnsaph.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pzypskls.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2taccwspa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zkxmnpfb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wmupnvzm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2raaxztzw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zdnsiwsd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fenteycw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jzwinmzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ymlpylkh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hlnxdqpw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xfcjudut.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2prxlsfmq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2erfzjird.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2drdnnvkd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2idvsbvxe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ybowqhgf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rdkicwaj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jinjxhpv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wznbawsd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nqmbcvxz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbxkuxlt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2crpwtbgr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ttvgydqk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yklqbhkm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yzcfjlmb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kbtnvlns.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nfqezzex.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ilslykwf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ofsxkmht.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2upzngtec.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gijvrclz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhhpzup.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rzpdruzj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkrvafgk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hxoqeqrq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iiakwohm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2txhslaws.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2noqopopi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2czxubcux.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rzspvzlf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gumbjfrb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2utvhjppu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ujiyhfjl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zunndftr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2piipwlvu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2bfrbjkas.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dchrqkyh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvlzckwn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zcwujwhz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hipczgoj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2srjvngeh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2astvwawe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rhutfsvd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fkhiiqbd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dcmubflu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xiehpzck.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nxbrwhqz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hkycajoo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ismreioc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2fktefewk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vdpuhtva.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yqyfkvlp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2txgkgwee.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mujwyyfj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dyxxfwtc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xxysqnke.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2etyufawg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xhbmvino.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bmdpiddr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rqlfauol.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbsykctf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tfpscbem.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2riuwydic.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hmgglepy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dnnjiown.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2jrirbdgt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fykyihth.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lsslakpy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wemwpvzt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cqapgget.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2suzgvwpd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mechixhh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ukmmdgwu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rrgqgjgx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hqeksase.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sfzqmkcc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2grmosnyf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2brpbguof.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcclkxuw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnwfrts.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hqpyixif.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2haelkcgx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kblbvtcc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wfsbmhvo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ysnenvew.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2yqrpjcjt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pigzauiw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ntenkodx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mifzrids.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zyfdgojp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pjcostts.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2jgshevdd.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pglhiucn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kpjmabfp.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lfgbnirt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsrppqor.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nanmjyid.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xhyumdrn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2onsgkrab.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2abvmpcxi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fnuzrbof.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2aewhqsln.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2otntswkg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rbrasqlw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ozwoyxbb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jviiihnr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zyruanwe.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqbhffvh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jdcvopnp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrnnavx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oovimhly.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vpernbrj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2vomkrzpf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2roefmxui.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2hehuqvdj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2bavwtpdg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nfvkyrkz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2imlvqbfs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2adhhroqg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2uvzayfnz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hahvbdku.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qevpskxa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zuxgomfs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fnjpkvce.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2aqwcuwvs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cyixrovx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qnkshhvq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dshqgdgm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zeqigkjv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vnsdkjew.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dkrdxaqa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enejjynt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wxsurjuv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jlcqttlg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yniedjxa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2udltowpy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ymvewlis.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wluytkme.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2slafdyul.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fxjjbkuh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gtlmyafk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rzecxmtr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijgexjup.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ucyklxkk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zeodstuj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikgudjft.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vwfouauh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2olcjobpe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2giklffwx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2fnevleeh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2pmmauuhh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2nbyibgns.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2evuqdofa.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2byzcxmjv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wsbrmnwj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vwjhznxe.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2elegwrxy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jfaagdgy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wknnxoph.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2qowikmfz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvhyxfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2puiykeiv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2joktoiwa.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bgxqpgyw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2jjehipfc.html


<!-- 参考信息 -->