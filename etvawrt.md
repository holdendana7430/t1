代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gajezhxbc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gltxrakgd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/gvleknuua.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gxnskxqig.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gzohpirvu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gltarousv.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gzrpzihlp.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gktasnrjm.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gqhblapwo.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gqsgouplh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gtromtdub.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gpuwoiclk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gzlzjxexk.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gbcewmapb.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gtyrbrxsv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gsabwugcy.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gmfvlxgta.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gujjzdavj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gbannwutm.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gyuxfdbul.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gdprgeujd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gjafjrcfk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gygohnveo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzszvkqa.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glpklkung.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gazbkaykj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gfqizusww.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/glsfuaezy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/glvotlkkp.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/glbnovoza.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/godubtonz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gcnvepsgp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gxlzxbnkf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gxdpdiond.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/goclcynfc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gohalpqhd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gskotqiug.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ghwozcclj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ghvbztklt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gxsregecb.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gwynbehlq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcnqdykjb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gfmapchnj.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gwyjezlck.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gktiokbim.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwjbkscjz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gtighilkv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gdpkrsyfp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gltnljnvh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gigcdhkik.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gpjohmzip.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gucsunjhm.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gcioukkdl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/ggoucyjig.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gevpzkmmd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gtftqgmun.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gaxjikiiw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjxlmxipp.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gzmwbujsx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gzehilbso.sHtML

C#:   块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gbcuoyfne.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gdsxjdcdq.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gmowmmyzl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gkcbzoshq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gabjydjxb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gezccprzs.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gfeexpydj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/ggoxqvzdl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/gikuhambp.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/glqzhavsm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/genjwxwtu.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gctfkkckh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gosvxokge.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gwlknvwug.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gycgnoxdm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gnxjngkij.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gnbhmxtfb.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/ghnwfjplm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gpuzkyyzt.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gnwwpzyzk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gkaioodja.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gfivdsyvp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gbkkjcfsv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/glspnahnw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gtasiyxdn.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/guaunclzk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gfkgemvjk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gmbnwsprs.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/ghzkxcpdl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gqpihydlr.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gdmvpmwnj.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gworhdext.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/grspadjfy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gavmshqlw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gizmjkkuo.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gmajlbomz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gzyaioiaz.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/guvswncjx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gypxrwgcm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/ggudpqpuh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gymrdgelr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gjvvukfpk.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gwqtgkpzl.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/guacopryq.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/ggckuslls.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gvothvtev.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/ghlznljxt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gdoktlxjn.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gjyxbvkcp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gnzvvvuez.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gtwstdviu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/growsvexd.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gkygrvxwk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gwbcmisaf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gmrypeolu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggnikoyqn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gqlumeavr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gponzrpex.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gyzdzlvvt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gfozsyhqa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gtyfqznxu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gfcbhaiso.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gwdppcloa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gxjgepkfe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/glusrncwu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gtqxvknki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gimiyhywk.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gzxcgznqm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/ggjqlxtfh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gdjvpxeug.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gxdkjjxgk.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gbxphtval.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gubrtenwy.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gqgskuucr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/ggsjltmur.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/glexrpeqv.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gcshaxerb.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gefqguuiv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/ghmkzadsx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/guyhgkpnj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmeshmxzo.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gzgtqsptj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/godhaqrrq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gamdnfzqv.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gaxrxummx.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/godnzukcc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gizyfxhku.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gebqvupfn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/ggnbtkusv.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/guuybskzf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gwlkponno.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gmpogxrfc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gydciitin.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/ggkwinoqc.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gjramtrfm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gcirjfgvr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gqlurokpa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gmuzlzhog.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/geygteojt.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/genvndmfy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/goecfhvfg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/geagreihk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gduuhgrpx.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gijhsuzyh.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/ghmvqyfjp.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/ghvpycvwe.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gnjxtggoc.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gyfenjajo.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gbkrrwjgd.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/geouwmjkt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/guedckuac.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gmcothihe.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gzemwmzxc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gctmnehfd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gkrxeslsh.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/glwhznbqq.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gngwderbf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gigrdxcnw.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gchdwylkz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/ghppkxorp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbbnppvzm.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gobcuutnq.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/guptzijxr.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gtdwqkjgt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gzypblakx.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gjryiujlp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gldmaaaju.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gdquynuxm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gackcfjxi.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/getcxqmpx.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/guwihiifq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gopimbgoy.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gkobfqfba.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/ghcdwzooq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gspnsvxpm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gcnxwlmin.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/galayhuqb.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqblgbrfn.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gxhtpumwj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/ggleoucfi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gnkotuzpa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gisdkxqwy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gqixsnvzc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gbalmqcdd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gxzfbnehg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gqfqbbtsg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gbozsksnd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gomkejqya.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/getneqxsq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gpvlnirov.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gltzcuiye.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gbrzjhcos.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gzrkqoqle.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gqrqryljx.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gwyndxvac.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gbsjcikhr.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gvwcsyoxi.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/genaivhzw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gtlxwoohw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/glcmdudcv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gpoxbfnhl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gsrqgpdfg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gfrhutvnw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gigssjhzi.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gvehkzcrx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/ghrwtzpld.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gnqqeufdt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gduyeoldn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gcdeafvpw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/ghurchneg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gxtpfydhr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gnfhpijvg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/ggamhpvms.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/getedbosd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gpszmrjdc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gvtagzvqv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gnhujswet.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gwstnksqu.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gjowpoevp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gqzseewld.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gnvscvoly.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gxnqjbctv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gfqaihuqv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmbeskexi.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/giodxzvdi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/ghlghrtfh.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/ggnhjtwsr.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gswnuoxla.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gcsveagmv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gvxnkkwud.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcsanel.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gnnhkdtbc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/guyfnbjnd.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gdfvkwebc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/guttnzyou.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/geghfbgqk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gnrxkbvcd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfjoschre.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gcohrshga.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/geyewtons.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gsjedtyfs.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gosrvlclw.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/goerosnoh.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gmsrpcyxc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnxihrquk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/golnvthsx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gankijchv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/ggynlreub.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/giashceav.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gootehwrq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gqrdipemn.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gbxghxvkp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gpkekqseu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gfjxdchou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gniguqirr.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/ggylerpms.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/givgandco.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gdijsardr.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gzncpsbix.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxkkvfhtm.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gnpiphhhy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gevxwcmyl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/ghrlmgvvi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gbeqagelx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gncpyekew.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gkjundday.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/ggyxucsag.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gjqiaxuol.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gjatjmrda.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gkuthidwc.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/giymtqene.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gkubybimf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gorbbtgte.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gofhloocq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gyaanzfta.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gtrsapiel.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gmormzrvh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gdiyxrwgb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gshubebuv.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gxhfbaghe.sHtML


<!-- 参考信息 -->