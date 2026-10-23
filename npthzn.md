代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3angoizsk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lejdjdzt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3okmnvtak.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3nrchcvwu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ailmjsqb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3swlzbaiw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qllrfobl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cphsonjr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tbhhmiar.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lpscnwmy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mygmamgr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jtmzjtln.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3npxlcjsr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cqefqjgz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kbavbkkj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wppwqhzy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vhsgnysw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3odjofwvt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qgihwlhp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rntlyots.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3eavhidou.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pzynkego.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3veubzxrr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rutykkhy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uhqxdvsi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3olggfczw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bvecswmv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jwokcebt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3hnqqwthg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3tptternf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tanhlwgp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xccfvibr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqwyvfyt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yemeopam.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjxogntf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zonkqspp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3iyngwent.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3qlboltpx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3twcazzlo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nqnhwjgg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3evyvjcif.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jmzvkewi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kptphkxw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zhdjwpvq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeihmhrq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zhlsebav.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xunhvkrp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mhphatuj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3alogktke.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tjbkenqw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pwornkbi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rknqaahh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hnadnkim.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxshan.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ijwubmdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nrjfxwdn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hvpskhsf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ahsfbrsm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ovcpniaw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3eidzrxdt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kjnzfxue.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pxqlmskp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3peypumcr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ygczmstz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3brbucqjm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ufddiuzl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zdrqkjon.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3tjmzgkpo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ipftbefe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3snasuevp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bjqdcgiq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wxfwncge.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fqlkogqw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ohqjeyfh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pvyjmkam.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ezoaxgle.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ckcfagbs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yjgpcuyk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ibfrxmdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zrwweajy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnqytjpx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3waufyqml.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wkzvcxcu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lrrvyoeu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3qowokpfu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3pnarvwot.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ybitroxs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rmwwnbub.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ybknrrxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ueqspkpy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tfocxoll.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mioebbvo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uqdozchi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdsmyryp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3osunusss.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pporymde.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsxhlsiu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cbixacnk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rzidlzvc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uveydool.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kjthkspl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3njwhrolq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3cqjkyrcs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lzncjomn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ulzgvmnp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pgsdxfju.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nefkvehn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwqemofd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fudiuvsw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jkllfapa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrebdvbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slwgqtqr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3watwyjew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcoesnyl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rvyofdon.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kobkhdaq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3naxlsupz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mnwebdyl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bqkksvtp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xrihaunt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3btsymmbd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nfkpbeaa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bulidgln.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eyesckfb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hioctror.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3myzsqlsw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3byfdscgu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3toilljre.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3srvgxddy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vkbcodtr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3evrxvxuv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ehsqzgdl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ioqhajxq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whrnrbox.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3gyshejod.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ifdrgotk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bskvntlx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qgjymldh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hemyjwfn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qyoytzxv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kzbridyr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dxkaymlm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vlguhqxo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vwchzkje.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bpjjonan.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ubyzusge.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zgdyiewe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ryskgsou.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3eszprzwm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xlvtdasa.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lzahwlhb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uunwrrwm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zyayzyzj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3odbfbgey.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uspmuyus.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fnksgrxz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xiqnvrwb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jskfinhl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lxkvgcnd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uxuozzyv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yfepzebb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pybhaxpu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ccwceafd.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lryntmhc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3afkzjnfg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxwccmub.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tkxarfrv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hdnlobls.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lqhsavby.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3kdosvssj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lsgeyoyk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3buwamdpm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bernntbe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wwpmgqfh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tohkodsy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3syalrfgv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3avnubxxf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lmlavaop.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3bsiesecn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3pugiqyro.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fgupqmyf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3rnoabcgn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hftupknh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dcglywqj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vztnrepy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iozfvgtm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3krlpeabz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fagjzsra.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zyiaomvq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3lmsloter.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gjwmufnt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cfuvchqe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkykukxh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pkjnjykc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uwffywkj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qvwgcoqo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qkefxkkd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ygnrgkbv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qhbtvfnb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vqsgqnpn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3rdhhkfxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jvzqkcbc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cumvgqop.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ktljaldm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vubcativ.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3stbsguqn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zvqlmkfg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ofwbimvp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ybffytmq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3svpcqaku.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3stioxwwa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3igzpdjln.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pqmccdyx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3onjsyfum.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qetetzfe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uijiivoa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vefbdnot.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uymvkuyy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yronungo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yexxzdgl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3eafwjblj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3diktrykm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vakhuawb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwyoqdqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lzicvert.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtggxpp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xvkzrotb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gdinqide.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tjozjhmm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3grpnkcbc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ohecpbya.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3grvfuyue.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rcepwxyk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwphbvnj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lwrwetxp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3sgvlyznu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ezhailrk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3psvmsmvy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dxvrdegy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xkjisjoq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hbyyahol.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tupdcjvl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dumqyqkw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3auvmnzre.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3luuljsrl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yndmpigv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ndjkhubn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3spdeqryv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ioxsngpe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hdpthsnf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jixeagdu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frrrqohb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3hhoxrpyh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xgghrwau.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vhckjyhq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3qbusczcp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kqwehmuk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vsuoimca.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ijolsgsy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufivyeky.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dlesuwgv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pfbllifj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejngwlpx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3svuxzghb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddsnhxcr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3mhhxzwod.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gsxiyehv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ltciojow.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zqwirkkn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mpxhqfxf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3fbipmbtx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xemxmhvx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jsjempde.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3nsdkuypm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ufarduuw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ismlvkym.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kbsamytb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyopuiwe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vhehxfkt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mxgrzaex.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lbzrthbx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lfffmsea.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rhmktwcj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3upfwfrbn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rkdybhbe.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3yldhuwfq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3akfcytrh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lydsieqx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nzifqfat.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uuaqrbog.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3rnahbvrh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vhsfouhh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zzqbbdjd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xtndwqaq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vrtctvmq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rnjwvszr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3agkfhjps.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzrbhhv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmciuoaw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bpfbnfoa.html


<!-- 参考信息 -->