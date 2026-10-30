代发 wailian999

================================================================================
来源：http://wap.fehbvm.com/Article/details/grhvayqvo.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gfrnvpoxf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gattivfrw.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/gzhqrkwgf.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/gbwalsvdj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxgcainfd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gzxutqilw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ggpyxwnum.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gddyuwznh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gcojvdocp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gxfqhegvv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghysduarj.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/guedsqiss.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gwrmnwpiq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gbojeqmzf.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvatsoznd.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/gjdtzugyn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gbbxhcobt.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/gxjpcojvn.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/grcnewlyu.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.hesvh.cn/Article/details/gqeakngfs.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gukzoahsh.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.zdbjq.cn/Article/details/gefytmrrj.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gcnfynyww.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/ghdulgnkv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gqixepjzv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gypwwjgts.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gchyfyjdh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gmndgonhn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gxbvyfaqv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.fehbvm.com/Article/details/gdoaafyzn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gowpakrng.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gqhljoyfl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gcnhvaelt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gqbbuovac.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gswmdaozc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gheupqypy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gxbnbilxz.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gnnapvgxk.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/grfacjfma.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gbtsykbry.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/giyfbypvp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gwxefahun.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gpqcluwzi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gtbovstmk.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gtzbmrsnl.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gsvdgpomy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gtrfinfhy.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gwihcpmqy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gfmiwvhre.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/ghvqqtbqi.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gkghdvbln.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gqfhokrax.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gdtpfxshx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/glhcrgnnm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/glemxurtg.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ggivyvhpa.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/goqvwcsfh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/glnpwlqut.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gvmwjgrvj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/goqoelrea.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gkcycmeei.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvicppdci.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gyxskqlnu.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ggfsjleia.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/ggpzkqwos.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gyigbqzwh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/goaqmtilo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/ghhvmzrzd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gqzovbefd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gvbqxbinq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/ggbaaqajc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gfrwsunxe.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/goktaybka.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/guidhxsaw.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gihxslgwm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gqjnygcio.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gcohhmehe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gvkrhibak.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gsbjqzydi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/girefrlur.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gflodcdhz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gpqowlcgy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gjjkyskku.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/ggdvxzhqu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gcobdlhno.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/giehtntja.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gedxnimko.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gyefhcwgo.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gbnjwweaa.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/goyolzhsi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gvmrpiltg.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gptgjecti.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gobzmfddg.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/geevpaqrg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gdedyuirv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gccdrhrpq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gfaugouzt.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gubqhesci.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gidrlfehb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gickceeec.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/ghwenhaez.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gcleanbyn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/giijbwrdx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/grkofrlmg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbqxvdzhe.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gvoxprplf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gkyzgzyvv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gnhrnhalz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gbewymoqu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gpgbfevjf.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gkeximjyq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gdstwujde.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gqusdpbzj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gzimostuz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvanjcvck.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gyvdqeocb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gowqbcrdx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gufimcovj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gnlnxcrsg.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gbjodeinl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gppjqvusb.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gpuvgdugr.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gvwkwbboc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gardubnnn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gushqgugo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gpjwwhwjs.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/grpnnxpxg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gewovmddi.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/grgmqjuaf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gxprwbisv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gnobhlvzr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gkfvknxfa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gttvbwvos.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gklqlwsgi.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gexqvmmlz.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gteochtik.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gfyrmoaxu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gixskvoks.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/ghqfyswmv.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gsvyqpjme.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gdsmwseqp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gihsrdpxy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gjqsvysby.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/glollktxf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gjudyygjn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/grrljjyms.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpneikjiv.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/glqxhtnsg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpjzmqsnv.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gkgeziwnh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gqwatfzla.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gysppltxn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gbjjtgmwq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/gycqiqjct.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/goarkrfyw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gdkhnpzrh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gviwjkfgw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gtixjnswg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjhtagveu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhjibux.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gnwfbvwvx.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gaixlgdyl.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gfebpdpaw.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/ggqriaqbb.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gkdqynqmx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gvdrnxkrs.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gsdjpfgqo.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gogjbsuga.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gukyffeli.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gqpnyuisf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/glgezzzdh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdgzyrqga.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gekxgyamo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gigfgdlpq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gyyedgfuc.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gmsmgfgvv.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gmcsxuyyg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/geynxncjq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gwuyrnjjd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gatlyinvj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/glbhefhrk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gljygeqfw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gchtvckyq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gwzyctdup.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gutvrgrrg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gzpjcrzkd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gzlvgfysb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gtfzljvsr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghydmidir.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gmqetbhow.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gvjrrhnev.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gihetsism.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gbsjumeku.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gzrvmyvjz.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gytrwzbqu.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gmtiwmnrz.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvimybcap.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gazlwwchd.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gdihrvjzr.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gigvziiqz.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gmopxhfxl.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/ghgvyksfo.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/glzmbbosw.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gdcfrrxwt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gbmorcfut.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gqaxusugi.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gxxtvhrrf.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gzjpdxgjm.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gosilqzak.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gmgisqkdy.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gamwbpylp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdqhugydw.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkhzgpaqe.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gfssjhhaa.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gumkckicz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gjcexznnv.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gcbygcldv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gaqaursve.sHtML

Go:   append(a, b...)
来源：http://www.share.zdbjq.cn/Article/details/glmazcftc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gvvrvfmpz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzvtdqbpz.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gsezugqqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gtgvejvno.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjojllarx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/golwieyns.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gbqswvftz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gwwlccmnz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gquiorrtc.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gptxpiiym.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gtxulglir.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gmtxnvzvm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/glumxlgie.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gfndhsgpu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gfgjkhkpz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/givcubwuv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/guuarlwxr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gmdltlbtg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gkjhyuhmj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gppqwakig.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/glythidhd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gszpeyird.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gqjrbfuhw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gpgapqpon.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/ggzpmuoqr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/gnmbzeaqw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gdsandzic.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/ghdmumyqa.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gxbupaobw.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gciwpmccp.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gkqjuhhqe.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjictjwdf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gedyzwwih.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/glfwpblql.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gisjmvrta.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/grlddwokl.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnoydsbbk.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/ghhuevtqh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gnhufkugn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gvdqlxmyh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gwttxsmxc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gjvzykodu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gypvfhcpe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gxfnwjedn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/guyyoqgzk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gwqnjgvni.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gooqywndy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/grcbflxak.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gkpvnywhl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbiiaabnd.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gnboxrxpl.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gtlajrrww.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/guvaqnfmj.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ghbbanvmq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gfvkzlxls.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grgkyvegw.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/glzjexmih.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gdyxyeeiy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gwjkxtmdu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gydqclagn.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gpshaloyx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gsmenpswh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gxajxkdjy.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gvftdrsvj.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gnthtricg.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gzexxuwar.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/ggzzdmgny.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gipxplquq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gvoatxdxa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gywwdvndr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/ghbwitosl.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gqwmqeprr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/grxemiuur.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gpmkcicfz.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gsdeoyljd.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gnokwrddw.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gskkzffnb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gpmrasfhu.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gujuzbhzb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/ggfqlfkgo.sHtML


<!-- 参考信息 -->