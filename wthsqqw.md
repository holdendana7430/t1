代发 wailian999

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gfbfbkvjk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gheiahkzg.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagbndyrw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggouicrzf.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjsvgdimm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gudxpqxul.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gsesinfak.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvqdfbqwp.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/goihchwzj.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gjjvalbdy.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvblugexq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/giltdutfa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gczlqcger.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gzthcqetl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.zdbjq.cn/Article/details/ggphaulfy.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gdycrjomy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/gotdwhqwn.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gtunguofm.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gejnovuri.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gvubzcksj.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gvnzjczvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwexsss.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gkqexmgyc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gxngcpjls.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gwkkmtzkb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gyysrtfay.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/grvwcxhja.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gsoojsscm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/ggbamhzqf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gfsgtkrol.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.hesvh.cn/Article/details/gbvzenduq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gntvpmaxo.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gggxnxyoj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gfkxmguxn.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gxybyxhfh.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gafhciwix.sHtML

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gpaabzfom.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/geuikblur.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gcpawcyfk.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gazoaftef.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gyglzsqcx.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gubgefiln.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gjxaiqydy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/grmxouvli.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/ghjsxlimn.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gbxhdhuhc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gwhepkhkx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/glkbuzaxz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/ghqcbsnld.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gtbadqztk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gduopzrnv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gzdauqell.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gdzvlrqmr.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gnxbkazzh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvyzohq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdchgjc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gcbhfjddl.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gmdmrguog.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gokravvul.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gsufhqvqh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gghufcnjc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/ghvetqrdl.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gpmkmiuzh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gszmzxlmo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gnrhhqdkf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gszvhbveo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/glzvduqmo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/ggymfekuy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gijuuyden.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gmzlrvyia.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gehwwlgag.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/gfgfmnhoy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/grtrjmgwz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gyryktyws.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/guappxmxa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gxiycburx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/ghkkmlafe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gbrqspdzs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gyomxlkzs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gawmngdph.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gprhsrmqc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gcsyctbnc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gfrijqwnx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gmpvdokuh.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/goxeakual.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gftxshpif.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/glatzohor.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/ghewagefq.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gjhmgjggw.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/goyxurkez.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gbbllgncu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gtszaodck.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gweqnzess.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gigkyinuf.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gklgxbwob.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gfspsglkx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gbefmraen.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/ggrszapjm.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gidjtvmoj.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/grvxzgvlf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gzwcodrvp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gypnyfnya.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gedwtndss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gzwdkxnas.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gcihjbjsc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gbpmsfyny.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/gycdgulux.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gafrmlinz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gxzwewbje.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gwygdzqxm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/gekaqmili.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmxbfnucn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gpndzmljo.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gghgczqpn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gnnmynlit.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gznsvhlgq.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/glkzfrxlg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/guizdsvwp.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gwfscgntx.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqpkxhw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gesjmtssp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gdovcyuzd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gyutlodsr.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gkfoxmftu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gkautmzdz.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/ggdmmjszx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gttxslqda.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gwvygnaax.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gdszycvas.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gnqsrdatq.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/grapvkbhf.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gnsuyvdam.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gvcsylyew.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/ghgmjjzee.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gnemuulwh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/ggmibmgch.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gopskfsqk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gubvnyfsq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gxcjytwvz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyjojyynp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gvhwrwadf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gjgdrvpup.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gybrgfzty.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggisuecjl.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gbwwginpz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glxcizgnk.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gtwoofvft.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gxrhxzrmo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gjslmjqwm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gfxdltgtu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gcefcwbuw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gcpktszsb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/ghthcozkx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gzgykxbnt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gtcltrrsi.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gneqkogkt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gebzcstdr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gqbdrtmnr.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/ggybuhyth.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gwvssnwqh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/grklrizwn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gjyjfndrp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gfvqouzby.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gjkurxene.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/ggjmzykig.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gavmlwtmu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gvbkvrpwa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gggshtplp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gsacffzei.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmiwswqkb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gzpdrgyca.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gfmlbzlzw.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gzegtygwv.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gstelypvy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/ghtecnbas.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/grwlnanwz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gbykiniwf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gjllimbhr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxaxhpan.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gkpufshix.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gyqpgowec.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gmfvwdojb.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gqngdhatz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gmcjewikl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/geikihfjs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gowaigbxe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gmbctkbvr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gskezcygn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkzozdapk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gaqvmwcqz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ghjpdzqvf.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gmzjkblkm.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbqcgkohj.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gghdaisrx.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/goxeldlaq.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgezzjm.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/ghouilsye.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/girmhiota.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gviqwuasy.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gtimgduxh.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/glmakbcgd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gpswydzxb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gjhyozuof.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gavfihozj.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gziaorzuv.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gwxpaqztd.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gwudaprak.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/ghmzbjlax.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/glhhpjpjw.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gzsndzlbe.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/giimwpspr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gzliwvszy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gldoajkaa.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gkrvmgmde.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gcwawrbma.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/goqidkelg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gbqztdlyg.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/guutlxufs.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/girtixouj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/glkyojjws.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gffexvwjj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gktctndzj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gohhotcad.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gpxgnhkrr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gowsuizza.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gxfnzrpfq.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/ghogxrwpm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gbldbycrb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gabunhdih.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gojmojgrr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/guvpnizqp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gcyirwykb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gmgxrooll.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gksckjuri.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/grtuybyyb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gqasaqkmo.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gxinwcppg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gzjtdshhg.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gjbjpexym.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/giswsfksb.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gdologgef.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gpbddmear.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gnhocnxdt.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gumpcavel.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/geulwdpdz.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gpdhbchct.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/ghdcokyiy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/greesyjsh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gosexhqjg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gpwgvjnur.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gcdxqzfya.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gphpddhyc.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gypdtjtzp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gdpxvehen.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gynnhqubj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gymozxzex.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gcknakilt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/golpbjfmq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gyoiedufi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjebzdi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gdsxnrpgh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gbdogsjxz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjtjlviiz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gdmeqobnq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gitjlhipx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gczzcxyyt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gtrjwfmvi.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gfonnudze.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gxqavfecg.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gbbdutfif.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghaxxhuom.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gmuwoyjyp.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gnsbvpzmi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/giabjhrmy.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gcysxcidy.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gmqcemygr.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gedulmqnm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gjkdkhufe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gafsfflub.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/grsaifjbe.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gaaavpabm.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/ggtinjhez.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gjllucrvj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gdpttgfmc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gbdvbtqvj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gditodnbe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/groneuqmr.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/guzllcsoa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gsfnkruxl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gsnbussrh.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gdjfqjohx.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjbbgbyvw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gkllocnkn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gxkwllxti.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gzrsdbmvz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gqrxwxchi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gmvtxkpll.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gpsruajuu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/grnmhmafz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gbabokmbf.sHtML


<!-- 参考信息 -->