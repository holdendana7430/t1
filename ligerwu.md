代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gczhgkqdm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gqgamoper.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gmhexycdk.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gvxnunjff.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gzbykzcxu.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/grhvzxvou.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/ghtsstung.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gutayqyxd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gxzxpddsy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/guvpltlda.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.hesvh.cn/Article/details/gptebuklp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/gkfqkvbtu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrbgzyx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/grkriccoj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gvlorihsy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gynpemvrj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/gcfbiijqw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gcvxdhasf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gkzccmqzy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gtzwxrbti.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gfciwfftq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gvuqmktgd.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gsuqnsghs.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gcnpziptf.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gndgyzpux.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gpbgzabfw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gchpblzwm.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gqdxxdoyj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gsypeeklt.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gtbflvmrr.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gyebmtuqz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gyddushez.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/geadsgbhw.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.hesvh.cn/Article/details/ggqstacge.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gkjqwzpgu.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gwaslwipd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gparcedeg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/glfaczbff.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gwpevotwn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gyaocvqwp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gcgwjbvil.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gbuwbosth.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/ggyayrfwv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gtxdivjkr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.hesvh.cn/Article/details/gqnnslmzm.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/guyqblwvk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gapbdvkqm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gloulbirv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gdfbvzogy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/getvgoimh.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gipwnizqm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/ggxwofqsz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gvnzawbwr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gcnvrdppk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gmxkgtgtr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gdfmalcpp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gjvfikdqj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gfrakjisy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfnyijluw.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gnfjqrtiy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gvqrvpwel.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gzjnkinmy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gbevfewwu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ghhuqnduw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gfxgejyrf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gmqvjbnjq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gvofpmvmt.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gztjkcybe.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gdbdxkrmi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/geyputpot.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/guhqfifga.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdmwzpamq.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gnnewizdx.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gwwucgcfk.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggypwxxul.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gfhdtpjrx.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gocgldwwe.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/giofqzwps.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/ghhxdvlpk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gvfigdazw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/glmglrrke.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gfsuvelah.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/govpwqxxv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gklbzabju.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gcejfdrki.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gygkgosvh.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gsrgizhwa.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gjhlplszb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gqhzosapx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gdzgywigb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gbxdimpzm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gwninxzze.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gsteeneya.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gdqlajlua.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gycuftqza.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gtwgzsbld.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gqvbtmsxo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gaiscyivc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/ghlonfnrm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/giamkmqvd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gnasdphaa.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/giqjpxdvc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gsdsyjlny.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gubxnwujy.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gzytymslm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gmbosfspj.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gieyyunsf.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/ggkjbztji.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gxajpeyzb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gtzzafocb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/ggchpbwok.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbusiicqe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/golovxopu.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gkltyvvxa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gapbsedlf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gjfjrykms.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcdxeygjq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gczapldbk.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/ggkupkceb.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gssmsuxbw.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/grbkladpo.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gclzqehek.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gocupbbpz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gddlyfdpb.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gjotrfrpj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gwbnnbudx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gkomztltk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/giygjxnfd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gqjqquwqx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gespmgpck.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gzdohfkpk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfvafjoth.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gztdqqstz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gunjytogj.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gtabnhyje.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gjbsjtoyt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gftnkmzwc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gnobdwags.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/guwmtztya.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gsrqlmvwo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/grdjlehjj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gmanwzxyj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gjylbvqen.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gzwhxrher.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gnwdlhhyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gqrslgvwi.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gwndzfqxd.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmkwuxgvs.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gdvwpxunj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gsudjkzpn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/ghrdvyyhk.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/grkwnjihe.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gegajznfr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjvqouujo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gdyyrnnvf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gepfuzdto.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gtcjteqou.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gimjtmvvy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gijijyxiw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gxfvvewyg.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gklebelkr.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gytxgqvud.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gcycsdapb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gdtvepvgc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gckpeohgf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/galonlgxz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gvpbjcopc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gxlmkyuyv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gmtulvnsn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gdihsilaa.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gryxsaowh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gyficwtpg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxoxknwnm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gswcafscu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gzrzlvdni.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gousjethg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gpyrunpfy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gmafyfzcd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gjxozmret.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gcwqpiwlg.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ghuiuiune.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/ghogdnjnf.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gqixensiq.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gxfuipnfa.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/glmvtxwlv.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gqsibevfo.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gwtsjsrxi.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gpalxweoq.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gdpxqtxzd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.zdbjq.cn/Article/details/gfiwchrxq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gsyoiuycx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gjmkyumhn.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gqjracljy.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gisaemtrg.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gxowkycbd.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/glrtzwjsd.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gchzmptdm.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gqvgrsrnu.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gbvzwlugz.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/ghggqvjeo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.hesvh.cn/Article/details/gzrmxopuy.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/goywaaisa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gnwffywxl.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gnpvxyzij.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ggawcqfxt.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gfhxjreyl.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gqtvafxuu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gwkcpalhy.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gaitsoubg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gwwlzpgwh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gdczcqfec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gepmjbded.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/grpszurxn.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gucdlpszf.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gvpjdxtzu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gpdkxkoor.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gsmkkvbdv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gbvlopusn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/giwwyogll.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gqnbgaoeg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/goqomvrvk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/glehyfbkr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gaomwwund.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/ggqeytzev.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gwvjdxgot.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gwbcxiipa.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxpjdtqnu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gztpzmyys.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gqyopmehp.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzpdzpz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/ghzvjricz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdegqliiz.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/glussbten.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/goadbfqom.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gerliaufz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gmoebsazl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gnfzyjxah.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ggnrfozuv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gujdrwkhr.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqwexxfha.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gylhkpvui.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/goiyaembg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gvuesfoze.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gjnobpewf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/guufzqnni.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxjrkxigr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjhrfpysb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gzacjlohn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gefhjlykc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gtmqiotkr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glkhwklic.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gvrfmjxat.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gskgyqxlq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geuykzeai.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/grslpulmq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gbnjqqcxw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gltjczrdr.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gtnxwuwlt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gapnabuao.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gyweusbgk.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gdqppajtt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gsqcrdmxb.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gearncglb.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gvwhebwzd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gffoqdbre.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gdfhexilh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gksgzhtuc.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gvlcyphve.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gvbygnkip.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gbcihhkdw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gnkdfwbsf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gnspdxhtc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gmfoqrzlw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/godvmjxdt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gtcdnfezf.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gvgkoibyq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gvqarnprc.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gyquzynko.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gjcuqsrln.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gidfdvnrb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gasewvota.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gybzcitjk.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gjstikdoh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gkucbtmwx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gwboopraz.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gdpucwuny.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gjvjgfonz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gnfsmyyoj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gwxiqdcdc.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gosxorjwz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gwbcuembl.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gzhxnxony.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/ggrjmjved.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gflibqoia.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gaabjxqir.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gmzujznyj.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gmuiszxlm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gmwrulbeg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/goizuhedj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gstfvglmh.sHtML


<!-- 参考信息 -->