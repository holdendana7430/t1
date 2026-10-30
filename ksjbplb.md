代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnwlfltfx.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.hesvh.cn/Article/details/guqodonid.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.hesvh.cn/Article/details/gtifyojbq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/grlrzcsmn.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gcltlvbfy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/grdpwaodn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.hesvh.cn/Article/details/glumlyttm.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbjzyyget.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gucjsvepx.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gtetznahg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.zdbjq.cn/Article/details/gntbemhsm.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.fehbvm.com/Article/details/gwalreuuc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gydzaccso.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gufdhtxcl.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/ggeddpyzr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/ggvkxxfzh.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gwajvexif.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gfwompebm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/gypcktjbh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gltzluczx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gezosxzkk.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gtuypwzek.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gfrhtepuw.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gqwdcooew.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gvjxxyttv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gylwzbfed.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/ghnmfvsvd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gorshdkaa.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gyugcwklp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gviiaqjor.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gxvdlxogb.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gxychrthq.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/giikwclad.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gxihzzhwg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gtykkqgjb.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gtmlyqlna.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gowwuznge.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gqgvlmqpq.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/gzpysrpnm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gbiufrmov.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gfzbacbnz.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gxrpsnsjq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gzfjmabpu.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gapwijroa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gelqvfgkc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gnustoqva.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gfacqwxvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gkchsdobr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/guidshazj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/guuaidxhf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gzhbpbzsv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gpcuafgiq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gpbrdwkey.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gqiplygzk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/gcguxgwjt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gdmejaoes.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/ghdpxvmdm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gzyixseum.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gzcqrwuzd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gnjugjtgq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gnnzrsqva.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gosphcegx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gbxnrubry.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gswygkjag.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gqdeuvtjo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gbgprxcai.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/goyqpnaxp.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gswqhknir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gtccfskua.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gjicwzkxf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gmmhtaged.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/grngwhlyp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gotgwzicx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gcbaexpkl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnhkhbuqm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gbodssotf.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gkicgclsb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gvrlxgfqs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gsyxdkewz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gxurjmarw.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gvsuhnxbd.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gmjtbcolu.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gzntrhrzb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gkxfdwlhj.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/grzpwrlmv.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gkymxkbkz.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gaeyuvsdj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gspsasqbz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gmuqhvhas.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gzfaxazsu.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/garxzmifh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gmfurkpih.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gcqlnsqbr.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/ghznsfyap.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gwjrvvgoz.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gympuecim.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gxdbefysw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gkoyadcdc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gypwcelix.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gnbkvilgr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gvlgkmbrw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gckzducgz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gwobxfmqr.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gmhmkumwc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gcyeldzau.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gacszfdtx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gnuajckxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggwuifnha.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gebcrpway.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gtdxktnbj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/giodiaoud.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gjjrbhzcb.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/ghoxryyky.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gguxxjyhq.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gwcigelka.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/geoejwufn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gijqzbrwf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gfckqkinp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gmfhjlltr.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gvgbvtxim.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gqkxrhsjs.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gnbcphxgd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gyvagertw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gsvksghvg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/glyeopjgr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gcddykgde.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gmcvegoeh.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gdrusrncp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtfytnr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gljrvikvn.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gjkdhsokc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gcwxqmwga.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gmstkqguc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gmwryavre.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gfvmifvnt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gddesxntg.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/ggcmwojbi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gjpwhsbgc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gzurynnrg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpayymdjw.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gcgnvptur.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvazywxgk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gdhgfljti.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gsynbgbti.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gwrkvimrf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gcexfhfba.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gdtzngxsu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gjqxuskzh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gnohwtrdy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gdhqfyfva.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gcjrmmmak.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gxxecixtk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gqibyofrt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gjpxkdewv.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gnefifhmp.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gjmtvqtit.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gxutbguid.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gupgtxprd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gwatesqpy.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gdntzmvwl.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcwbiunle.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gvnstuaum.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gmvssvrlz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gdocqdnpw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfjjchnv.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/ggrchfelb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/guwudorwh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/grebgbfoj.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtsnqqpyx.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gjfkjrmuf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gvwwiflaw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/glhzljqqv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gjzpgszqw.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gxojnnrbz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/glfdpkoay.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gknaxjzcp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gpaihaava.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gvlaejjfq.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gaxefrwzi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/giyowkrtj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gynakgdpk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwxormwph.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gwtnwlavr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gztgewpat.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gaxiljvps.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxhvkybud.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggmgcxxbf.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gkdrqfkzz.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gapmxnspa.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gssotsbgi.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gpdngftjh.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/ggvhspjsv.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gwufivdqb.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gsvpmcypj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gowuszmdm.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gbcwbkner.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gkjiiwrgn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gwuidwhjj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gbvmsojhc.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gcbtmxftk.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gfpezuyjq.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/glznfenuq.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gjglcjnqt.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gwrauyzck.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/ghjigszsn.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gfftbschf.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gmzjmzexp.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gxqhzwxfb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gnnzrotja.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gufwyiccq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gcsxakqyx.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gfmgtiles.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gornqznzq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gwxchaono.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/ggvfsuurz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gouxodgjl.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gisapgeng.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gqhfcgjsb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gxkamltso.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gniebvpsu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvdnrtz.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gngetugob.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ghqudcqnj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gtufzjefg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gqbvudccy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gsjmarjco.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gbrcoxftm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/grelzjonr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gocsjgfow.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gydegwjpc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gwzewuuhg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/gmteomyvr.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gjpqyfxmp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gchyxsbxi.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gaunugmhk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gxcrlclqd.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gnpkfxrsj.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gdoqayswn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gslmbbbat.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gbxhymqnu.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/grtqfblkn.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gjvhbjhjc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gfycmfvyq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gedkzgkro.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gckoivmmt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gyjhdfvjk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gvzeamsug.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbznwebsw.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gxaushxgf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/gvjvrddmu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gxdbojsav.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gavqrcvxg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gokcnkpmq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/glqkrcztu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzqzxozpl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gscpedmjr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gubhcngiv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gfbujlmgp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gvaeymuzi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gtwihoqzu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkraptjng.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gborwlhyu.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/ghbnarumu.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gzdwhyuni.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtzxspnxd.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gofrbrcxf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gezwmstov.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gsjpflvid.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gebdddhrs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbwhujxfy.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gybbvvxcn.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gflgjyakc.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/getgtjktx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gxysdkuoz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gnktrhcjq.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gewrijnvv.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gxqobxrwx.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gmuocsuuo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/grwemyjai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gmephogna.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gvgvnzdjv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/grnrtngqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gomzsubsm.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gtljmhgsu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gmpqgdzmn.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gufglmsbn.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gakbuzmgi.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gkhptavmw.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gxvefdboq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/grlvfyoci.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gdmfzgtcs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/ggvinawew.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gyyhysqxm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gkisesusr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gjycmqzlp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/ghuwtodnw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gdadytiof.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/grklfnkcs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/ghebsdwar.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gsivfxemx.sHtML


<!-- 参考信息 -->