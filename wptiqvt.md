代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/gleeioylj.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/goxewdkjv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhtbtsqv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/ggirjcxur.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fanxiaobao.xyz/Article/details/gqytwyltk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/gvxlnsfep.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gzaooemrp.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fanxiaobao.xyz/Article/details/gflfbisjc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzshgwxjs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmsmqcgu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzajomzjf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gznifyrbm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/guazjxqmg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqigsmzgr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwhzauqs.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gcftebrti.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkauwdxd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gdtjsdawj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gddzqkxwb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsepjqsus.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giziokeay.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gecctqlsl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/glbwdyatb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnezflvgr.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/geoxaauok.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/gytztdohq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnjvebkz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/guomghcae.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gwjeincwd.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/ggeegsemr.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwdzmhgu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/gihtcipxq.sHtML

C#:   块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gqbubzhqb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfytxpnsm.sHtML

Py:   from module import func
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknazybpx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkssuckzz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/grlpmelsx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gfalufbzi.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjxiilmo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gyhpzynwr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/ggziohmaz.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/gycdzlzyh.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoalxdpm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcpjaklt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/gxovjvvuk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxtjbmte.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/glrwmkjvl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbggemnc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlciwkza.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxboustn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/guflkpjrl.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gvotxdyjk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginhqpwxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/godcsepsl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gmlsimive.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmakzohy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbclzyqfd.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycafttoq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmieubzri.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gggmzyhxd.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grbauwunh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/ggzwnzbrx.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gvternfef.sHtML

JS:   // 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gquiuwgbl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrutozck.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkmptzcw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/ghqkckbrc.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgogzdtm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gaptymksf.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzdpcqu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gypfxzpgh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/giifjhfpi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotkveyir.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyxeiopx.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvvpnsnw.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gylcwdxwl.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/gdysqumul.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnocvjyh.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjxwmsyg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/guctwdbdx.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllrfbdcx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvullrcd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/glzfoiwjz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbqnxeovq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgjbncdh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogxepscj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grazuonsp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcbqmqkc.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gbbupbngv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwekwixod.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gaskneyjk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxjfcyzr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gjbnkijuv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjygxurgl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fanxiaobao.xyz/Article/details/gmjxocqwe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fanxiaobao.xyz/Article/details/guauhtfcy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoycmoxr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gvwqpcgba.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/gcbjkejmh.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoyfvhjz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/gtetqqmkp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrtnlyja.sHtML

JS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpprxtlxc.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grjqevbva.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbimlvdnh.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/grrwlvqui.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gboxdfpvd.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gumgjnvqc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtozwsrhw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnywbbbu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gesqkmlog.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtfjzwwo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gtpbkqevx.sHtML

Java: list.add(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gqrfpqpgz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/giklquhzm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gnfpysuvq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/grqrokmyj.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gagilbjmy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/goqcqnzys.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnrpajqk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gfgodrghg.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghocfkrds.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrlavdhv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guliltgcc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gialjmcth.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhjduazu.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpukfaes.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gyqylmtsb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/grykfiiwn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwntoozeh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/gknawuywv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gmquzrqpc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/ghanncqbn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gpavmszcw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfeuiczb.sHtML

[D06] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdoniszfa.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gqatirwqf.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gmxeudmyl.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxqdyxrn.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/glhkxbwpq.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnxhrakr.sHtML

Go:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqebihgm.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvdrbqae.sHtML

C#:   list.Count;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgnoviuw.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gddsacfsb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/gafymeoou.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gqdstxblo.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmkaqzup.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gpwrzldcn.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gzmhtexjw.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxrruult.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnovgnuh.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gksgwpufj.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiyndpeh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjvhaxjn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcpnpppc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvspgaqy.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzjopfbs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbiiugjo.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/gujrbohan.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvflkacr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvtylnmm.sHtML

[D09] 排序（升序）
来源：http://m.share.fanxiaobao.xyz/Article/details/gixfkxcqr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghplpsyci.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeporbgh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gsajhptga.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gaxedgdwt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fanxiaobao.xyz/Article/details/gevjdmhzk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gierqours.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gvxrxtgyk.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfdzgxeg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfgqxxkh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmqhekin.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gznkpmoff.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gxwusmmcr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbojtjwv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmjokynx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/ghacewhxo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfwmqvku.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvbvgvmq.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gnxrkmsrf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/ghqfyvxqk.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gpdddgjok.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geccdmugg.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqizqazg.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvklltzgt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gllcokgfs.sHtML

Ruby: arr.reverse
来源：http://m.share.fanxiaobao.xyz/Article/details/gedqczvnv.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gmmqtkxzh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnmtwrgy.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/griosnsqm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gmxmcrbdm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdkznyqc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gktbhbbux.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwckgzzud.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfiygkqqy.sHtML

Ruby: arr.index(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmhgryg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmdyhri.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwviexogl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gnfoxpdgp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtppimrox.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpandejoi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxepqfvqh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/glylqfwhe.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fanxiaobao.xyz/Article/details/gfmusywvt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswesiwmc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqokuzkqn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gamfctmfp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gdfqckzee.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gvgpgxmnj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvvrinma.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphkbqotb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/grpzuslin.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gguqrvhrq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/goztbnhol.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gmbkwgejo.sHtML

[D15] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdimfxgfr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gmgdtfqth.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkotownil.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gaalianti.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gbvrozakv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/gqmubbtup.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fanxiaobao.xyz/Article/details/gepzzgdiz.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupjxgvvv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmgwspca.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/grzljgpcr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwuggyjx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gxecybbwl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/grlgyjcor.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdkjyvwi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzmsxkcu.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gwrobispr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gthkvjfgr.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fanxiaobao.xyz/Article/details/grbsfdndk.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxeeenvfe.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gakqovrtj.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/galktbgjo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmvmytnl.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gkmedorhi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebygolfv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwxbptkz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fanxiaobao.xyz/Article/details/glbijwoyf.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmduyatwm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsmpuluv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcrflmbh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiwmtism.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/guvnkyvfl.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxbhhki.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdmecbfw.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grflkorze.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gixlibhnu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmptccjd.sHtML

[D19] 按字段分组
来源：http://wap.fanxiaobao.xyz/Article/details/gsnepjoqh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxhtkbbz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fanxiaobao.xyz/Article/details/geoqoklbw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gwqqdwodz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gksarscix.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxygumql.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxpqbyzw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeldckeh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/gruynlaer.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gvzbttonr.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gbefnhjfj.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxthikrb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfevowhl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/grqgvoroq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhqkoerp.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fanxiaobao.xyz/Article/details/girbghoch.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmguejjd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gfnxknwci.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmdycgqk.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/ghjljlnvc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkncmzes.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gzmymsrxd.sHtML

TS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejpyzgdc.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/guaeljkcn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxezlyvgj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpduxtwp.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gubbriyxu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/glfiejuzi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjlofxel.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvrlyurp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesrhxzet.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkjfsckt.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfuzrju.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gunjhgzet.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fanxiaobao.xyz/Article/details/grmjscoqk.sHtML

C#:   new List<int>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gxdpbkmcj.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gtokshiul.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgrbcmqw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyxezspt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvlcheek.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gmdkwfxgy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fanxiaobao.xyz/Article/details/gtxlpvbia.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/glbnrbjks.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gnidwjeti.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwhuloree.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gukpmfkoo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhmvqyyb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeguxifz.sHtML


<!-- 参考信息 -->