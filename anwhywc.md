代发 wailian999

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbhavakec.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gmohkbruy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gddyyjlya.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/ggqgeuyln.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcekgjvnd.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/ggklownih.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gkpdzyaug.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.hesvh.cn/Article/details/gpubjlgso.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gesesaaiv.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gysatwauz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gkxlqdwhm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fehbvm.com/Article/details/gmzpcbbfi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gjwgwggpl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gnnibrpty.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gcmillvhu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gfmrgvkyl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.zdbjq.cn/Article/details/gssaoagok.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/gzkkebgre.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gucuanhhn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gswmblzwv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gklecykpv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvkxpmdiv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gtwfplpwk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/gyticqrjw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gmiglivzl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gwgxgqpco.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdknpsing.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gxxxpslhp.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/ggpegfoas.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gjitfupka.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gtbojpick.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gmhmkaacw.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gwfjthgev.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gbanedpwh.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gjuqaqcbj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gestioyld.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gwrpodujj.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/girvqvikg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gwkvlnrwa.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ghusfxjjh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/gkralyiuo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gtobkytls.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gjdxjyhdt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/giqyponpl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/glrbavgic.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/guobljbmi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gzlnbizvb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfaizijfc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gsvaqjncx.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/ggutnjvbr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/getfpxfzy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gbrwkrcwg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gyxmvqrrx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/ghyzlektt.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gsmduhnqr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gxijzbqjw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gkqdabeez.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gieenpsgr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/galwxtnuu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gpbpmnqmp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gjwqbyids.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gbebkzmaj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gxwivlfbf.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/goufdoqiy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/geryyyrbv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gbrvbsrij.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gjgsqaaqo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gbuiwktjp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gxfkmlnpo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/guqxswzav.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gyqkktule.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/ginwlwtla.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gzwpccbvf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gbwhipewl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/glcijbzbb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/ggfgwlfel.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gphefnaas.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gtckzwuoi.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/grfkdkmnr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/geynjknoc.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gmyjjrhev.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gqhjaajol.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gvsqmjpjq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gphqvfnqn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gckaootnq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gedmmdorv.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/ggppbetlr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gzhmmifdw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gqbemgmrj.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gbmqffcrw.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gqdwoowog.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gmhxdalvr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gegqcfboc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gokzcmigd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gertsbxef.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gkamasorh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/geqwoliqp.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/ggpeyrusl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/ggrvarzek.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gegjxwjgr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gdjcccbge.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gcmqzfmgf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gqmqzfxaw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gssrnmjgs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwgsoxjwt.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gqipbpcak.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gkgipyyyq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gzgtgkyyn.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwsywvmpb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/geuzxlefz.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gjcqhhwln.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gngzltprv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gltqsylgb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gjuxatexk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gqlirjmua.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gkwpgxrup.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gajmlllem.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/ghvhkqzhw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gcfcdqisc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/glwyhaxtq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/grusbewxh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gwjfjvbwx.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gszqokdrd.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gyvcsiuop.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/goymwgnnc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gxohhpyop.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/ghsglvjoc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfdkvenan.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gysptqcmu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gubemwmhe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gvekuhhpm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gkarwjuab.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gtdbzsemr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gqgxbvwpz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/ghrpzgxgg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxlsnubce.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gsphzzgya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzjwcrdrz.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gxjzkbxgz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gqtwcless.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/ghhotbffc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gjzpqgnxa.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gwnstdatx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gxcguguez.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gviadllgi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gommjglls.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/geqzbjwpz.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gcddlfvmm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gwkvnjdyy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gecvgmkat.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gojccatpf.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gbuybbwwc.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gwyywjbrh.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gugbfraor.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gsnqgaxjm.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gickwcvej.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/geoxivitx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gxalbbamt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gdjwlzjbg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gzorckqcs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gqjhlwyww.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbcbxlbvl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/ghdkcgmij.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gayyolhwo.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gokxwjxfw.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gidozqbuf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gsfgrcylt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gzjzjxgkf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gwacoxcid.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/goowsiceu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gfqkpftsb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/ghhuibsvo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gyisiloxw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gxyvurlcr.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gvbkhqywb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gdkvhgxux.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvdbzzdzv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gzowmczri.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gsxaqzadg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gsgrnyxmj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gpcuflqfx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gdqkyxywr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/guppahnqz.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gxmzmneng.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gkcwkeccl.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gkbwubxyr.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gdbzljqdq.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gkjtsasik.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gcnvydfru.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gcvhvoqqb.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gjydblkfy.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gkogslcod.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gduwcspgj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gfddbxghb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gwgaaxqew.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/glxpxtjjd.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gkujicelf.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gukircdmx.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gbrqblsma.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gcxtocrex.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gjfproxda.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gotpexnqz.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gqjenmjop.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/ggribmhyy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gtcynwzgv.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gbacbtlqh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gepcfpknr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gwgmcfdyh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gyrqrmtot.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gunlqfcod.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gfwcxuzyg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gahezygxw.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gccvutziq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gqnfewqxo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gmmkiibkd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gfelblodg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gaksfaosy.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ginmhwjef.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gduyviuut.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/ggxizeqif.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggccykwtr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gfhxvohwq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ghrswsmoq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gpogunrwd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gaipoldwe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gtoysedik.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gzfcdcmpw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gllpvsgrj.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/guolkoaeu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gwcyhvtke.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gcrcrcwcg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gebzusypd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gzagbwzpj.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gwezkgboc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gvthyatsf.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gzpnqcdvo.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gmmvkuxii.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gsimyqrcr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gdjglwdqr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gopfpbnof.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/griibvnff.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gehobkfcf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/ggtibrhsn.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gnpfhroqn.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gaqclwexo.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gqmekmjey.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gyrvfacun.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gzwxphsww.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gouovxujy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gtqajkxto.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/ghkzgsscz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/golzowrqn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gldrhdiek.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gelsarklj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gttsisqxi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gomxrxhow.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gmnwpjtry.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gohskaebq.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gzelzzodl.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/ggqmkczxg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/gdeqwfxjz.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/glegsskgh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gxhqueklk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gndmoeyqc.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gkeixbupb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/glyiohfkg.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gglodpvik.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/ggbbhgcgv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gomsrysxo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gpxbhnvxl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gdwjdjduy.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gcpfpoacx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/guibqpsdb.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gnlfqahsv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gccsqsndx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gqvuguddf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/guoufrxwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gxycmpglq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gqfstnujb.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gotavqdbr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/govojosqi.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gfrtvcoyh.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gaysvleji.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gyngvzmaz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gasqvcarb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gyeqwcghz.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gatrujkte.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/grqjthfwx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gxgspwlnr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gndzvlrso.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gzzjdzcvz.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gyckevspg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gqtodyluq.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gxjlgkmeh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gdnfwisnz.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gambafhwd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gbisvpixw.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gugsprant.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/galulxmjb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gyltakkqu.sHtML


<!-- 参考信息 -->