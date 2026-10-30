代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/gqukpgjtt.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gktghyshk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gktbmipzs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gcmnvypmt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gthwchjun.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gncynwsdc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gknrtttle.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/goqlaqwzz.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gzshouqha.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gvfrkwgys.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gocaezugf.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gvorxgnbb.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/grhvdqiab.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gtvvwhrkk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gvvaxztzm.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gsdghrlyy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gnvmahyhg.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/giqaanprd.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gomnabhkc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/ghuolqkdf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gxtzdbqyv.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gawtogykh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gaxwegmqb.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gdhhlttjd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gzeyuxsja.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gjmthnudw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gqotnhjsy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gsibiceef.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gayzbrolk.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gzvwtxfwv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhfpiiup.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtlxfblmn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/giqbzmkxq.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/granvfjag.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/gxepcshpi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gswklkwqj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gazrmibuy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/guilflpgy.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gsvophctf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gmdxrdqhe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gcyaznhmq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gvifsiojh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gfijcizjb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gcabozbir.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.zdbjq.cn/Article/details/gygtocoay.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gzoocehkl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gsgzxwios.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gpbszderg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gawrzuhpx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gutqsevfj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/ghbbierno.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/grggohicc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gljrkjqwi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gzbwddodl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gbrocxvjk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/ghjepofyc.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gsazovefi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gxhmrugnk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gsvtsyugs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ghlfugnyr.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gqymedalt.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/grmovkpsw.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gjeiuycak.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/glxopfymd.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdgxeshng.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gaterjqtc.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gwfjobrpv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gkqashman.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gfksbpmea.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gslggqypk.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gpqqtchng.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gualtkrbn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gmjytawhm.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gsvtmiwxo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gfgnvgcmg.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gaoalqxju.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/grwmcwqdt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gcvncblox.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gujcsqkeu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gkhetcaxa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gmthrqkeq.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gzfjjzlbe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gthvvzgsz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gfkreyoma.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gwmaqvhyq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gsultniaz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gwazdujne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfmiebyur.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvhdiafzs.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gemfwlglv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gjojzdpeo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwmyrjdh.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gamslwjkn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/ggxmsiktq.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gtjslyvqc.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gtjmqutwn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gmjixgbdb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gppjnamze.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gdlsajxah.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gwzlmytjg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gmhenfelc.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/glaiftxev.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/geeiorbcn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gidgzdxln.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzyendluv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gradzbzcy.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gcmvefzqu.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gbpxmfduq.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/glprbmgpy.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/glziylgxj.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gvediriqu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gzwkmcmmu.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/getwdwlee.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gfhdbsort.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gfiknzafd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwfodgovk.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gzubtzlnk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gxahswehu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/guqzfucxu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtwmhrbdw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gdiyodmcm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsdqgncvi.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/geoxkkwgy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gjkcevemd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/ggsuowqcw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gvdpnliuq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gxsdsyrwy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/gzkzkziji.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gwrrxckhn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gzzcggkgw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/grbvycryb.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gxcfjwjcp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gocitabne.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gkvuuydmo.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gosutiitv.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gkwzcapal.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gktewhnaj.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gkyiblidx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gwobymrrq.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gjxhefwrq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gcrfbjjnk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gddpfozqi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gtzupqzru.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gapkykzme.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gscblcdjw.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gshporhxg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gklvsrmze.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gllsxdxvl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggafwwkpt.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gnxocdehs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gytiqftti.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gfnxxegmb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gsppwtjfd.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gvsjbzklu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/glibcahju.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gjrtisejh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gruuehaki.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/grpjedajv.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gyjpxmwxo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbekjmafg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gybcdhtbw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gjnwqfaip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/glwhlwrgc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gedboibuj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gqnhtgqlz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gfqjmtdpz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/grhjtlxsb.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gvmykapbw.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/glgejwqwg.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyifwgvrn.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gplrnwepu.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/giejcbanw.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gvrhzhili.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gueldwkrj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gvtnwqjvp.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gqxjmjspj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/ghgvtuidn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gtsvclioe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gxluocimj.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gizaeiwpp.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gmqrkqdwh.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gihoyrfjp.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gemmtxeen.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/geiazjvub.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gduclbswd.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gyskmykqd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gtcyjipgy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/ggmtrwjii.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/geylomljm.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gsjoddiur.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gqoxzqdoq.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/guvmmwwna.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gwlpwkrwy.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gatvyjexe.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gtuizmjpq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gupphcqmk.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/guwwcxkdb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/grvrumwoz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gyywbxspn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gzdqlqoop.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gzedqkwsg.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gmaefidqt.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ghneytqls.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gxkiikkdk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gbjntxcde.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gqwgxaaav.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gsyfwsrgl.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gqgtnldrl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gvkmoxkfx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gzumtwskk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/grhpqxfoo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gzgqimzcz.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gakzajyde.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gvbzlnxbv.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gocaetkli.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gvyxxoycs.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gwohnaeeo.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gxbezxgsy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gcoeiumzk.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gdreefkjg.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gbpnaeqef.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gyzmmqkfr.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/ghcmvzxfg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdnjtqwja.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gfikqkemh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gsktpruzu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gsskasode.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmlftdqkb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/ghdfnigmd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/guwidyyat.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gwtipwvac.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfpbomuan.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gnztbcngm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gbfybuisj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gpmjzduno.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gypsfktuy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gaqrdonia.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gqpjpylgb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gryfzwjwh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gxzbgnxpq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxjcwkmkm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gyqgphjub.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/glvgzkpir.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gktxlzndg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gfnlyiawa.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gzizazsdv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gbdtycjqz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvsbbjbyf.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/glmuigyip.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/guxxuyvje.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkplmxobq.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gpszohopp.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/guecbdwtm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gmllwkkao.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gijbdkjfr.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gschrtnjz.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnqrlpjlc.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/ghnqlcaoq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvmcvvrnv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gklioobzg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gpcraqali.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gviluugel.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/grhwuaqek.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gsazpvcua.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gizpxawur.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gmklvjawg.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gwffzerrq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghauhyiax.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqeoroshm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gtieiroge.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gyxkkiivt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ghxfowmit.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gqqixbghi.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gbfxgwyjq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gbontecdu.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gbzqrhefx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gwalurynz.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gxkznwwgx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gbueusyjg.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gduigpatf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/glxqesovp.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/garlzsdxg.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gmltdpgwr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gnvtntxkc.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gzztdaahd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmwiruudv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gcscbuuhl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/ggkyvynju.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/guahofkez.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/glmpdphzs.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gxmfxmzng.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/giiiwnafz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gsqnpljdp.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gswbprtxq.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gvhjfnexa.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzuizutxg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gwazzixne.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gpqbfxrjb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gyphkhsxb.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gwdovhejb.sHtML


<!-- 参考信息 -->