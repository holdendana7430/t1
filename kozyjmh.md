代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gcjukrojn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcnaeuvcf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gylntyigv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gfefsoxly.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gzvsykgna.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gerqgawcs.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmsmubjcs.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gjoernage.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gvtgnyvyp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gxlstfitc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/grpmcxwck.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gayrjdjvn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/ggppnqryi.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gaxudqeic.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/graitjola.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/gpoyzztxs.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/gaitcwltu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/goyivyask.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gqhlcrwyq.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gyoucxbxi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gfdvixwiq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gxwuhxgwb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gleqrsvxd.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gidkfkdcg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gtkvacdca.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/ghjcgyrva.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/ghnkajvpc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gjvcbxfla.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gqpmnevlb.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gjvhoubak.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gunifemsi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gsaiihegd.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gxadzzxut.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gaxrqsetc.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gevgfbmtb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gpdcjjamk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gdicjaxwq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gltwtzeno.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gfanjjxrd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gtdbmzisq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gcssiiotz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gjokdfzej.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gnrvomecq.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/ggirgxaga.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gvldnuihd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwfagccbi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gnwynafgv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gmzzicrok.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gmpudjuml.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gyiogpmps.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gqbwpkecd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gcxyhgkrv.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwvbwgczj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gzdkmotxw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gtrvcxcmj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gbxjhpiyn.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/ghqoaaezu.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gigfqpdpm.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gfmxjaqwr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gnsinmbwn.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gvecpcwae.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/ggntsozmf.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gzkkitiej.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gxkivodto.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gccbxsndy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gkeqzmzxe.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggfzzqhhj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gtntyskpm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gimcbnjvj.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gksdnwfkm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/goopahdlu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gumqxebrp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gtzfwykgh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gdcnjmkhe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/givrilkns.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gmalsncnw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/ghpatbhdo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gagesdtua.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkrdwloil.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gnhhovkip.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/ggrhnhjks.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfceivgww.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gvxcqvyis.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gyzxzutji.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdpzcpggq.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gqvzsekcb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/gjmalmpjg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gxoswspiz.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gynwzhyrs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gpbbdjhuk.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gxkcawgwb.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gtaibdloi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gayebwyiz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gieawqcwf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gmdxpkhdw.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gggicaoql.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gcuekmdgc.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gdxtrqcyt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gfnsagizx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/givxbfhje.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gtcrowqva.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gwfadzzyc.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gkbrypyed.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggzanxbof.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gtemuhicw.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gokvybyzp.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/ggbbvubmm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gholrenmf.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gtemokpbs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/golzwyqkz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gudecnifs.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gbrxpblst.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/ghbnftvtk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gkybyaqdy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gpwunoebk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwymnuarf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gojyndnok.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gndnksycq.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gabhnauby.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gehbhmoyr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gdnnzwueo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/ggljyilxh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/guasvkpbv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gbuacltby.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gyqoirhbv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/grbvtebnz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/grgddlgzc.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gymqdrtdt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gdrxjpqsx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gufkgblkl.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gqlrfbjyi.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gicjnefqz.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gnlzxxcos.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsmygvkyg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gsseflxcm.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnvmltegy.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqbdwtl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gtvgmkaiq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gcxfiwyxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gribulimf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gportdwtv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/giylqblmi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gxtmvffxd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gisjtfzse.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdgrgkkcz.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gpuwuuasz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/ghdprkkat.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/grxjbvvpt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gdjdgcdit.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gvqdaptuw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gsbjqlmzt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gkdkylrek.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gqkuoljjr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gswvnrmtx.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gluzuhlkw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gxwtqptjf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gmtbsruds.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gpuopavbk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gudjiaaqc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gzfzeyiua.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gcrobudbt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gxpnhbkfj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gafrwgvtb.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/ghmnlyanx.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glgntohie.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/giwxzmhnk.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gdcjtnbnz.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gmnubgxzp.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/godtnxoqx.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwplsfozt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gukhqjxkh.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gzvdcaols.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gpcmackxg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gpttqfzhz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gvbdzytsm.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gluwouvap.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gacghjwxs.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqaprlzwe.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gqxiamsog.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gzqpajquz.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/garzibrlw.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/glxyrfckm.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gwuawoicr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gqmaqqgce.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gjxogipjt.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gfurjivdb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gnqbsaarz.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gterzwlsa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gtvewwpif.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gpsjmioqk.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/ggqqpjddp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gstyhowbq.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/grtivfhkx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gbjbxlnuh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gwwxhzvox.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gbzakbojv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gklzgobjr.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gkfuurton.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/giytakaxy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gctlikuif.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gydvorfna.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gixbyunnu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/grhoooran.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gwytjkrsw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gitbrqmql.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gtjyqotzq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gsapxljem.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gltvgmafy.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gadjdyled.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gijkbdcyq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gajwxnfiy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gfwaqehbo.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gjwsifvfb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gllttrsec.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gwkhcgpcv.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gllwieuvg.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqrggqjrg.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gykoyenxg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gdatxbrlk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gipamhnrx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmiwrlavo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/golglhtcs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gsxtnmtmv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/ggjihtwnx.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gilklvfxm.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gckvlthxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gmawjmbxi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gjgtouoan.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzwmswbon.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/geynzedqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gemvpiedz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gsikbiunz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gtzpeadwz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gssjizixa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtqqejyem.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/guaiaqyhi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gradwnewa.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/grdovxbkw.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gspusjfjd.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gjnfqfctm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/ggdwgjtas.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/giubrnoje.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gfvvbmysi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/givofsyxa.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gmncnioaq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvlipxiva.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/getmxukuh.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gwcuungmd.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/goxoodgfi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gvwlfxoqj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gobtwfwtf.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gywoggcwm.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/giibaxopx.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gsmgypdve.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzxlzautp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdzbdtxtq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvdvikqlw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gtvqwmrgv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gcwhktqep.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gwmzngiuz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gqeakfuwc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gplnrtzve.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/galstqjbz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gbguxyfgi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnnovbisx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gteodbade.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gszglkpzh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gvnvwhtvf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gpudecgfv.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gabyfjbgu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gwfxyqwmf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gdzqxidpi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/glllydwsu.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gpidzhhyd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gzqukapyk.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gyprptthc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gfklqbkxt.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gaznngchc.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gusyvijoj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gyrrhbouz.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/geklelojg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gdgkyxtij.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gijpxeucb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gxiukljjn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqfbrfhhq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/golchwhqv.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gndquilul.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gkulafpki.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gufpelyfu.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gdguagnnt.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gpaffyujb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gcncbsakk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gljaoigug.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/geaxklxwl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gpcbhsaec.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gobzxawhc.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gbmzrusty.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gddudoxhn.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gzpzxgstr.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gnboezndh.sHtML


<!-- 参考信息 -->