代发 wailian999

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/giogtfelw.sHtML

PHP:  return [$a, $b];
来源：http://baike.fanxiaobao.xyz/Article/details/gdxfzubwu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmajjxqgk.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbbwduce.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/gjrobsdmz.sHtML

Go:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqrztmkx.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxliclz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzvnrrqc.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gmamodkvn.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/geskpmzwr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gduhrctci.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyhwkynr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gmpndmstc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgamculk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gdgfexequ.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gahdyzqxo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnzpxzuj.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fanxiaobao.xyz/Article/details/gqlrmpaua.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gopsmnmxs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gnjhgygst.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fanxiaobao.xyz/Article/details/ggqjpnsiw.sHtML

TS:   arr.map(String)
来源：http://3g.fanxiaobao.xyz/Article/details/gujzitbnu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gaabkmuop.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjcmxpkn.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/goynpiiqc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gusmgoqsp.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/gjypqnjkb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/ggowqubds.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxxulxxoi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiaaegjf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzekklet.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjophrbi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gvohdlawm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrawaccg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwarmwthf.sHtML

[C09] 递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbtziiy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvelnfltt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gylmwsuiu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gptsabguq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gwjsbrcbl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdqfvqcig.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsqbwuec.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezcsqzsv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuzyiowc.sHtML

[C10] 变量作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrnlsibg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fanxiaobao.xyz/Article/details/gsoizvxdp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdyiyyww.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiyofcuq.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvtnkfq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/glicpbzvb.sHtML

Go:   花括号块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmmqlpb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaczlzvi.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqkirus.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdojwnvi.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvadxyqh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyguxvarj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdbcdimk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkhzhhlx.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdohcvlol.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gzdswudjw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/ghpwaavvj.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/grhwsdqir.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gqsfkpqki.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfepswfkh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtdvskx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzppzqker.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gfnqeqext.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gibkadryu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/gkgpjhunt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaovbxrex.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqiltzkld.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdonuyoj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gfkffuiqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/glrebfxhl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwztbpqv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgppzxzu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcelicyf.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/gfqsscglc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/gymmhnswi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gthnozndb.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqdtpjqp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gemwbkjvj.sHtML

PHP:  // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkbqacrl.sHtML

JS:   // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gilpvezxt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gviidrtro.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsachtfa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwtpzfsc.sHtML

Ruby: # 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyibvgjk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/gblsgzgqm.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fanxiaobao.xyz/Article/details/glmfubffo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fanxiaobao.xyz/Article/details/gqtojzmxn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohhkmhek.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkxilvdf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gobwlvvvl.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/ghxsiceqa.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyofujxm.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuqbexsq.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcaaualf.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fanxiaobao.xyz/Article/details/gmqsdlasx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gekvqzmcj.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gkcxinhgj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gosxkhnkh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqfuryac.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtffiflxl.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gtinjsiyk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjyzyani.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkrfawlm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqubmcksz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulytfitl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/golabcfmd.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gpqodsuxw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/gkogtndmr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrgobauc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmbpiwq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/gldzcualz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gxljtvzff.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmfeejy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gkgpewpyi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiykipkp.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/gnzlevtnj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwqebslr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccmltawn.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjpgebpzd.sHtML

TS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gvzkunsbq.sHtML

Java: list.add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gexgotnmb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gtiiobain.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssqhrkek.sHtML

C#:   list.Add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/givduoljk.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gvxwwesys.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdegvcj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnvbuonyz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gyybmkvvc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gvytpzftj.sHtML

Java: list.add(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gjqoxjdmi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqmrrgbj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gplxvjjzw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgeqrdgp.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gfmggcaxr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdiihtr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gcfxcxtov.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/godaqfiki.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpholxzmf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gonkmimkw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkztqnuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gscnatvhq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsiyecrd.sHtML

[D05] 访问与修改元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdbnhlcn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gtaqdvtua.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gaucvewag.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gmtojbsvk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiwuycgn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gznqeadmr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyaxriap.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/glomzpcsw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gjyfjszcc.sHtML

[D06] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gngwwdlmi.sHtML

Py:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjyhnylc.sHtML

PHP:  count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gfmixfzoa.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvczgxvi.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gdponrrth.sHtML

Java: list.size();
来源：http://www.share.fanxiaobao.xyz/Article/details/gsplfjthh.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaojzwzq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gyqbxyqus.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gzoqucngz.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvfwxisl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkmnuxzu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdaztqobt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwokmozaf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gxwcbulwi.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwjquyxuw.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gvgcjglbk.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gwwawkgth.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gowkdvazp.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqmxjzuj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgwnivkm.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfurgihx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjkioroo.sHtML

TS:   [...a, ...b];
来源：http://3g.fanxiaobao.xyz/Article/details/gsacrpooe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gixconlxn.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/glsvxhnnn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gouujokjt.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gdraqzafs.sHtML

[D09] 排序（升序）
来源：http://wap.fanxiaobao.xyz/Article/details/gojdbfnct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbgbqvfp.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gtdpdlnrt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvpvjqpf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/geiwnynld.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqarnlx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gbjcozfba.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gersyxqne.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpthmibq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/grcajwdjt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gzrvahtay.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/graoxpole.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhutmrdu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnthwger.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gebavvjqj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjfjmoin.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyifkldxt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/gsmqkqcsf.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gocxvbjrj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywayubbt.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpevsbtma.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtfynetg.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gxzsleilg.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklymikdg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcvtaipn.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrolrznd.sHtML

C#:   list.Reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfpmwkfy.sHtML

[D12] 查找元素下标
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbogtnoz.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gxlgimsxy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtadsgqpg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/giuxxmyuc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gexyzpdaj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gwqsimtgw.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/genhfwwxp.sHtML

Ruby: arr.index(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfpoqcgrt.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fanxiaobao.xyz/Article/details/gnaxgrkbd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/ghtsdhgix.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gpoyiqpup.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gadeudvje.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwnwietq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/graklljbk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gndrlfngb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppmbkovr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/gfnwtzyou.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnefdriu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaafjxlrz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/guikejzir.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gnkausyak.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guukkqlxz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxifsqq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/guideculi.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gwpyokpio.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grrhfqjbe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphraqvjr.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjndaujwx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmhjrqzn.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/glabnbobh.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdncjcmd.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfytlvls.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdggnmbac.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrlnonlm.sHtML

Ruby: arr.uniq
来源：http://wap.fanxiaobao.xyz/Article/details/guikuxcdd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyrfuryc.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gukbqyufr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbrcsxnye.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbtgupfc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gdggctypo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gtgwgvyjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fanxiaobao.xyz/Article/details/gtkdndxcy.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gitaopwka.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxlgiyxf.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdmrvpmt.sHtML

[D17] 最大值与最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gbutspaim.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuzsxexz.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcdybeket.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gveqdajvb.sHtML

TS:   Math.max(...arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gxibjutoj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrrqxycm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gritqheeq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/gafttzgbe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngywgejg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvdsgfhk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvgclmim.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gktyudhjj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gjhaiixzt.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpwbrhwx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gfvasiofh.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfluxbkj.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gihpciraw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyevjmiin.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmuqxgg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmrmnzrf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fanxiaobao.xyz/Article/details/gyiezswdo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginsyusek.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgiezpnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfajoeov.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fanxiaobao.xyz/Article/details/gnidsctbs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gsjvwgxwt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqgsoeaq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeaitidq.sHtML

Py:   Counter(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gjcwlnuhm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gachsdijs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemtustrw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/gbvnudpvi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmmeokeb.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxqctler.sHtML

Ruby: arr.tally
来源：http://wap.fanxiaobao.xyz/Article/details/ghrhmfngr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gjujdxodd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyxulgng.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gwhqkvfrw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gnjjfhblo.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwslxinu.sHtML

TS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/guoeeelvo.sHtML

Java: list.contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gjlajiwlp.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwffchgkw.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/goemkkrwg.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjoozrog.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/gszlznzgp.sHtML


<!-- 参考信息 -->