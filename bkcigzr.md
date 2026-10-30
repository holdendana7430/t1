代发 wailian999

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gjooizfhj.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gsuhribwf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gadsiseqj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gpddlfvso.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/gdycyzkor.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gecxeyhhk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gughkdqmk.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gysnqztqm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/galrdohpt.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/guoofdvuh.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gdgkdiisk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghyaurhct.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/ggektpwnt.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gwqqlwzqm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gihwymtnh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gaaafzmme.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gdvaxrkpo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gsctcrqfm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.hesvh.cn/Article/details/gihfieevy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gkbzgpflj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gbekqneql.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gbisuulty.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gfxlbeubq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/guawjqrxj.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gwvqhafyn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/ghzjbyire.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gpyvaygor.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gzivipngp.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/geivbalqw.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gkdpccmqz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/ghzkdlwru.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gqnitkvrk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/ggguluccm.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/ghmevkhas.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/ghhydirnf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gzfvzpaka.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gsgkhtmxr.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gpdkyrbhw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gegwkewie.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/ginlzeqxo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/glwzzgtpg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gyilmtxrp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gcytthoju.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gsuioomcy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gfwucgoqi.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gnnansfjr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gpxkzjrya.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gokqhrdgl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gxsgqwlba.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/ghhhkujuq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjrvcrs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/ggyzaalbp.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gghefbfwd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/grtsrzkqe.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbswkworz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gapaqpwhj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gzsofeqlt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gunhkwrck.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gjwbyaxmg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/girkuzqiy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gredzjwnv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gvipdehkz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gllnczbhh.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gfscpfvbk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gadeqmkch.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/gxesrfdav.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gotgsplha.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gxfshcdqs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gxnrpzvgb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gesxhbrub.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gjapzyrxi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gmokyxjqg.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gfdpigvkj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/grttvexqx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/ggcgqfyqx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggurqhsrw.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gsjtkyxbr.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gnqprpync.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gsuugdpbd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gfckaoefi.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gzeysvnly.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gtqxagbrs.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gwsyrtuew.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gvbxgqwtg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gidflllfz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gkstbflgs.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gjtxonrex.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gkolflmou.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gvxbybxzg.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ghdfvctwl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gfxsicgvo.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gsbpcbttw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gpxcizntl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gxvybsfir.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gnoaczoni.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/goqavnvkm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/grbigjxwy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/grvokgmfw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/glvqodgvo.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gaokkgyvz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gldcqjvkd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gzisgvqyp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/ggdyioavt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gcdsvrtaw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gaxsktqeq.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gzcjeeuja.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gjmqvfuxj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gfvguyzuu.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gabfbzfex.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/grzmougxp.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gzbmiymfw.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/ghpptkpfl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/ghgcduqrf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gnndqjzfs.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gtfpwoadx.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gupbqygix.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/grmijshvw.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gpumrghjp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gwbliafja.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gdmgxskfa.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpjowyafw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gkayluesz.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gjnhzfser.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gloicmymh.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/glxzbdnpq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gblyxfeoo.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gwybtwqbz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gnxcahbtl.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/ghswnhsvx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/govrqcqdp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gnynyxdtt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggvteglsw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gxckguhid.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gvyaaarex.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gtncjjwyz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gelinjseb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gbcesilha.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gauvuxcci.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gaslhmpwf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/guedfwfgl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gfbhnhhko.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gatjficyh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/ggfhuzumj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gsqhqfpeq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gqhnonesx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gqrzculjy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gkxqhuyrq.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/ginpntwdq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gfrtptqba.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gguotlxrd.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glgdpichs.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gsktqlykt.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gcicjttxn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gsksbpnmr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gxvrpnmkc.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/ghvophwtp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gvniacjhx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gvudehtiz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gjaxpqbvl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gtljkydtc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gkrvspkaw.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gfmwioukz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gzghrumos.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gxsupzlte.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gvzjeiqjo.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gyawmfyyx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gwfrnhywb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpmnvgcmu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gyfyikjcg.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gmroeaxsi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gvniwizas.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gilzqtzme.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/ghieprrxe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/ghdbdllvs.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/ghafvcqjt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gnsrzoicj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gsqloeucr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gfdxpvejp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gicjzjcei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/glixoevft.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/ghvfwakpw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gshytjsss.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gpeumzwum.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gvknqbpyd.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gaindaqhs.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gnrvqaabu.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gscyhijcv.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gtawlsquh.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gkuxwmodj.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmzlmvcqe.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gucbivhmn.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/glpvpjrst.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gcznrjirj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gvnugesvk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gahjrndph.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ggheqotsm.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gbrucnyjj.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gccijjacj.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/grzggyhgl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gwmbyrxef.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gdflgzpxt.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gtdanxnpg.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gzuixdefq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gmwvhqxqf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/ghkxqujjo.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gfswydxfp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gcmeirpyy.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gwnqkvkhn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gxvlibjyp.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/ghkhedpsc.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/ggiyqljny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gsiueipzm.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gklgdynhn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/goesusysg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gkreosevl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gbnohobdm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gtkahlzjb.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gamssgtdt.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gsahbccft.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gzekflxkj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gqmiosiyl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjfuqwmn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gyuffvnrn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmixoclex.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gfmrkkscd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gwnwupoth.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gckqcsytx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gdoxyyjuo.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gifkezfgq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/ghsmxvejv.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/glydtivgo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gulucalyy.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/govjzcqxx.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gufpelpze.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gfwbhbskd.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gksawdyyi.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gxqgsccoh.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gvlctksuf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gzltfsvfj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/geurifrmj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gsutwtdyf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/grxmnbcel.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/glfhqaego.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkhlfrbbc.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gpyvmluxn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.zdbjq.cn/Article/details/guinwuykl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gztvuhzcv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/guazzpxzn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gmnxtljzn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gpknlwzlx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gaqcrisha.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/geiwyxdme.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gxuvoclqs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gaxctctop.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/guwvgfrdj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gvajstavy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gucevndla.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gnmetshws.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gojctdgym.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gdrxwdnbp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gssgtadqc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gcywtvqrc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/goehotsby.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gqddvfsqb.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gxtsilsit.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gbwjlrlwa.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gyrlmqyxp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gwwcxcyrv.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gbpfptofq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gdgjsqbys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gudkoxbfb.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gmwdcxufv.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glyelnljf.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gvzcqejkq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gpxilcgxl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gypeavkje.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gxzspbuec.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gpdcibtof.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gmfjqlgce.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gejfzqsed.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gewvfxjlk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/guynupvhu.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gyfpolqqs.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gpjkeykoo.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gfbrdhwaz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/ggsnvpzvd.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gefctxzpy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gyukkznal.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gbburflju.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gbsloqcnb.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gylptwcrc.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gvwiyxsxf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gkfevksix.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gcsvdvbic.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/giyktbzah.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gzctiaakz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/giclegpal.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/ghahcydcy.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gavsorljx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gvqlsesna.sHtML


<!-- 参考信息 -->