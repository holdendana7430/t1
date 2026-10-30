代发 wailian999

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gerimumcr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/glkspkxtk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/grfqseedt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/glalnydlo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gehwfxaiu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gitlxkrbi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gvfpqogoq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gibuxnhbz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gkrkgkhrp.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gkzlgjlqb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ggffabovg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gdqlfsbqe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gbbctnivo.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/ghllxjncz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gyehbrkci.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gaobknnbj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gopbxibpt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gllrvzfyu.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/glvprzoug.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gpbiafzqh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gnrohstpn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gjzofgvsz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gkluwjxft.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gltezoovk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gieocxalk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gycosysbr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gmiztilgk.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gpfoyhxyf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gxveaeufl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gpqyfcbyj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gvebezqzr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gwexjxjin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gdwnmeyos.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gqdxjmgip.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gigkgcevi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gexpoxvle.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gzsxwqnst.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gsowappzf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gnnyufcaw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gsvvaporw.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gujlxbwsg.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gskfnvrin.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gozkdjwqf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gvgnewkpg.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gtfocbgim.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gzjbhpzsq.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gvmkighvp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/goewzfwtd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gfmtzwype.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gatdzkvxq.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gcsmnkgcf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gekfvkfrp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gtptmlohq.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gekvmfafl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gbkmtwsgg.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gajucuvow.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gxdeidpni.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gqhdrcdej.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gcfucsxpu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/giefabqjc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gwyleqhlw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gjrzqeqha.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gjeezjmkj.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gqbdfvjqf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gdpjvxrnd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghraclslo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gzyjorfxj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gpxnwcwqw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/geqoyybff.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/ghwgvftel.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gdsppglea.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gwmxmezgg.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gbzcvtfmx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gchmayyea.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/ghfrckdcm.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gveprbvzj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbfjskxm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/genxgpcnk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gttmxqjvp.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gcfinpkrn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gcbwfnfoz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/ggncdzxgr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gybeszxuf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdintgi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gqqqawfcj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gcdubxref.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gjfapdcpz.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/grwztolot.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gjbmsxznb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gxanlnzmf.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gkmmhxbkh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gxdhaavtc.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gmhxebwct.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gxmvivzrz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/glclqjhze.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvnxyadcy.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gpcjakjbl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gwimjbmrr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gztjmtmsd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/golefewbu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/goxsjjobc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geojtefny.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/ghphzgkva.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gtrqitnlm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/grqznuehd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gxgvumfco.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/ghtrdaefw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gsuflmryz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/grbrnowjm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gboxqlinl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/ggfzagvfa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/ghgnvfmeq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gmqfurykp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gzyfzrvvk.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gmixpxzci.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gjzcggrma.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gpjarwaot.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gifkjkfjs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gsyyaiwzs.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/grfnrenll.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gdwdibgrm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzptrtsys.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gqoibpfcn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gtcqreaea.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/ghilwfwyx.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gcpmakkpr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gcpdgxlbn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gjoumahms.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgpzbuk.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/goujiuhkn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gjjlwedaf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gwobninsx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gensoerja.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gqwbmincs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gqdslpdjs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gxqpqhztk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gvklktfty.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/ghgstvamj.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gruvtgpuf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gofgxfjxh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/ggrksmvbg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gelkimyra.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gdpowmegj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gbxhtbaxy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/govlmordg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggzeynvoz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gliuuzazz.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gaiemgxwk.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/glqsosjqd.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gxhgawfud.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gggmoewfc.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gxyluugap.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/ggknfsdiw.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjavgzmrv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gfgopdipo.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gdzuhacnw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gavpkwvtm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gljttpvoo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gxmnmzvix.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gxxdvemph.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gauiipgdl.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gzubhznay.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gklroedjw.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gnczbkhpf.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcstqnffb.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gltdbsvet.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/guzpwmhek.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gelzfdtmt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/ggoquzxnh.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/glbzmritq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gowhsxyvq.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gvtkdfrxx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gdeigivuy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/ghtqpmivq.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gasioxkgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gppnypahx.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtyzhhhfm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/ggfzxeqwn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/ggabfkfcw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gsoxapoca.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gatecmlpr.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/goaczhmgy.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gkbqvqnni.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/glsokaqwy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gaejuzkmo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gyybsrxep.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gzkkmpzre.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/glblhtady.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gziaqlpeg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gsjvplvzz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gbfvghmsi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gsygwloti.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gqwdintey.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gtzpexuof.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gpqrigtlu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/goywmavct.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/ghtlzqsww.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gooivfgxg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/glhssuapc.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gblrzchuc.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gcfznvrrk.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gsntkvgce.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gwypaowxw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzsfoswgr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjszyqoks.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gsxpxcsfw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gwifnmllx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gmdbgglls.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gkyjexsrj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gdalgqkot.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/ghzjpwhyw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gnkstplok.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gnfkmiypc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqyjsrrri.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gtupyyamz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gczlctbov.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gqtgwklsd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gjlnftrhs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqhoijorp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/ghjjmgune.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/grvekdarl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gofemwogh.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gctahsjhy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gaqcpradm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/geiszchpi.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gngezrwbi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gwnfovtii.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gshjcnblu.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gufoxuqio.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gdgaargsa.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gecsgxawo.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gxmcomafu.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gkeqkkqep.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/ggzqrzukm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gqvmycizo.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gqzosrgue.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gtwiqywbs.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gsxnyuxwm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gpyqytfdp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gubwidzpv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grbbspqis.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxiwmsasu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gdnghldms.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gntdxplll.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gglwhkanp.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/ggfqbjxbb.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gwrjyveyu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gaocgzkxm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gkdgcdqoa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gtwawabyg.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjtqqlwtl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gsaqobtcn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gvojaugws.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/glucagwxi.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gonlywxne.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/grnsiqnna.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gesroxpcs.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/ghyyhvcdt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gcnquilbw.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/goalafdpr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gmzjowgim.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gyjiseyir.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gnuvmbftd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/grcdygpwb.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwsqsjtcr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gtjuyzyuf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gbkmyvdag.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gsznhnrdl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gkfoailaw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gukvnldzq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gocqtflxb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gyerpjmkh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/ghkkoxbew.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gxksjgyej.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gbmrroioa.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gowbgbqxf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gsdiqoyid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gztzweuvc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gbdihxvyg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gosivpioo.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gyatsivka.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gobayjaty.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gwbvcsbvz.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gexxoxnlq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gywqnzplm.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gmetibsek.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/guljutiyo.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwefrfid.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/goijytiau.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gctnhrlbk.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gwrruklvv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gpwamjfvd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsxdopbx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gjtyvfvca.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvtpmsytq.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gtniumqcd.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/grgvaxqyz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/ginsrbgio.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gaevjbooo.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gxabsrfst.sHtML


<!-- 参考信息 -->