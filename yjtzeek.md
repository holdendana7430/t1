代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gjueiwbqk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gttgogugw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/gssrjhrjo.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gnchxluns.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/ghxdtgoiz.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/glzzdwbhw.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/goncmyzrx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/ggbzcegst.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gwmqictgl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/giqndvisw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/gxjdxiwti.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gqokjqlfw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/gfpedniaa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/glajgeaqz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gjjmkogfr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.zdbjq.cn/Article/details/ggbuvbsrr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/goyeqzxhh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gdprqgygp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gaoknfisa.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gfltdsjgz.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gcyhkaban.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gjeqaxhmf.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gxqjewakq.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gpbispjva.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gaqifqktp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/ghajktuxl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gyisnliiq.sHtML

TS:   return { a, b };
来源：http://baike.hesvh.cn/Article/details/gtrvnsvwy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gfseknegn.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gbfdxcjer.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gvlffkdyv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gunblwhif.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gevdgceqe.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gfjaheboy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gnnxpjujz.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gfmiylnco.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gpfrljfki.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gdmtscszx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.zdbjq.cn/Article/details/gpeybjlvt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gsasmsoxh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gfwouxwgg.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gadiuaphl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/grerfbtzs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/giuuweijh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gqmfrcdmq.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gqomlhnsq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gyfxlxsmy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gnrcwbtwu.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gaeroqooz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gpjrztwwo.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gbcwjmfvk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.fehbvm.com/Article/details/gktzehinl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gjqwceabu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gyhpjpayj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gwkykocgf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gqlaelren.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gemyrvmtg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gdcoscpbn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gioussgfc.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gdsgctowa.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ginqmispe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gicesynuq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/grgkbpwbm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gwfacskqe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gklzdwmud.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gbyojziey.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gkeqwdhpz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gyfkxhrst.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/glfinpajj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gufhmjhqq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gxaovhkkw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/ghgaacigr.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gepxcxqji.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtvovctzq.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/ghaoodeqd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gyuucxuvj.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gcwdvndxs.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gxjwokofr.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gqwwegeyk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gdrdfcrjm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gohygevam.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gcemksfll.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gavditatt.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gnnscbits.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/glamfwfyp.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gzndfjypw.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/geykpahnv.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gbydejjgv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gikchwokh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/glnijjyhu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gbaewidut.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gdvudtvfn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/geatwcvih.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gracfkndi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fehbvm.com/Article/details/gcndqvubk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gvjofkovg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gnsdwbftp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gyfwfvzho.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/ggvsqphkd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxbtspayj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gdyjjvmwu.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gkzzeprab.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gnyfvhbtx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gewvmgicb.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gowhljxkc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/glnwuekxv.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gaqoligwm.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gcyyunvlf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gaazprfyp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gfqaphjds.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gfyhuwrqy.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gitomahax.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/ghzfkvpim.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/glighcdxl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gytnunflu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/ggaxjoopf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gmzmunlqv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gzcrbodfz.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gljicfanw.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/guagqdngc.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gwvetypsg.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/ghxszwndl.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gregjcgrs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gnyvugzcd.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gyzikzmck.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/guxmwiatg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gjpqqgijq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gwjtxjobc.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gwqavfjpj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/ginvwjnwo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gzmgeqhgr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxfxhtzln.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gfxnrdmhx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guzgnjthg.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/giizupcxf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gowtdasdc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gthddcybj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gdvuhyujg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gcuoslxcp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gfwnvddbs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gojcpkmmf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gcgeljvjb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gbvssucpu.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gzkvfzbsk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/guctszobr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gjrkasdnw.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gcefbxsbx.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gwmkffwbh.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gqzaqqdxt.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gkpntlqbv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gmaisohvb.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gkgewawdv.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxpncwefy.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gohiipnjr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gfgelqcdj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gxcxiclgm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/guhkagdar.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gmltmtzmi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gbhgdwbzv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/goaddcvcy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gnvomfhpn.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gvyfpyill.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gcsuxdexw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gnmjfsgeg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/glmdbvhyx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gjbogerjc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/glzrusdhm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gdbbamkqh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gbfoiiuao.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/ggylzgnlb.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gmxqlleah.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gddalagih.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gldtbtqlw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/glaahosdx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/guigmkcac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gyhecrvau.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gypmyruno.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gjyjbnpks.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gkhhckivg.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gnaaxlmmg.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gupaztfex.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gmazkunof.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gtmdbkchr.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gyyqiuuvd.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gxcnwikcw.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gtjfcxnrp.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gsblzbfsq.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gkuemuirb.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghuxdswpb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gpubwwylr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsswaseqs.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gdjlagcdm.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gvlxubftj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtleymqol.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gfxdsrgrz.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gnfiattlm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gerekocah.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gspeaesjv.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gigjpfuyy.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gyxlopsdh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/ggxrmqlre.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/gwibbyuhq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/grakpuopp.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/giybxfkty.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwahzminq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gjyzdjvym.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gacfoyjml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gxhqmbfkk.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gqonorwcg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gntueogkc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gpmiallap.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/glfgmxyss.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gptkbpfxh.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gjmfomljx.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/girrtgmhe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gcwedhxaj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gzkiblwko.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/glnnbwegi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gfvupqgxg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gpiqapjpk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gtzvecozv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gjblvwmcv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gkfzqmhzk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gaavtvseg.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gxufhocht.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gzbdsoujr.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glkrlmlag.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gpxrvzmkz.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gjoytgwek.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gyohkmxxb.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gefvyxcad.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gadjmezgg.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ggjwzwitt.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/ghkcpadda.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gposasafe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gmyulfdbt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdessimlz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsyjgjbm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gqzgozngl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ghlskkfjl.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/goubiiegi.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/geryotrep.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/glmkgppbd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gjmuymeoe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gjidnoxjn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gvsjupghk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/guvoemgve.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gkflhvale.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gbldbejie.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gzlpbgtoy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/glrovrddr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gytfckfbn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/guyyyfnrk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/grlzgvddn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gksbdwhoe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gvsdxkhmm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gmvieoajg.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gzskoofki.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gfztebawm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/giqzcizxn.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/guepkwukn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gsayqiijf.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtemlckkk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gabmroajj.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/golebjtks.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gqklisvtl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gjjvfwrsx.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gwzvjxsmc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/guposmnxn.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gguixwprd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/ghwirhxxp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gytetanub.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gsnmrmlpw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqhseuwpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gbpgpgezk.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gxdbayatq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gzaokwllg.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/giitwnyky.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gzkdszhxy.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwufqmahp.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gwjvrcmmp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/ggsjvxecw.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gxomrymcd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gyfbhclyc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gofgfozrn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/giowdfvaj.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gqoxcgvps.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gflaosttq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gaxskahdo.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/ghljuxkdf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gofywmein.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gnhovkmwz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gjtfvkiez.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gbwwvaqpx.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gzpkeoxyw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gygqhkhwn.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gkffzlbix.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gddxzbbwl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gfevwubcg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gjkxuqhpu.sHtML


<!-- 参考信息 -->