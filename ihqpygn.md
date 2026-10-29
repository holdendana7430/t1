代发 wailian999

================================================================================
来源：http://blog.hesvh.cn/Article/details/gefuwhorm.sHtML

C. 函数与作用域
来源：http://mobile.hesvh.cn/Article/details/gxvusywqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/galgflvgy.sHtML

[C01] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gipfmpwvk.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gjbfsybpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzfcpbqfn.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzggplaho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnrncdjjd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbqxknzd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjdbhxazr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gdsispvbw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gkbrlvmmj.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gvtviitxy.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gshzccpfb.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.fehbvm.com/Article/details/gwkyevaxt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdbwlayln.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghigfrmzv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.zdbjq.cn/Article/details/gddcrtxkc.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gihupfrmr.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gxbjjsiff.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.zdbjq.cn/Article/details/gyfpildzd.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/ggndsvzcv.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gfluqgytk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gzvtrapsv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvklbaocv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gkspgczty.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.hesvh.cn/Article/details/gwlvatywa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gmzcvmhfb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.hesvh.cn/Article/details/gdmmordoh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gzjxeodxu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gehpkyexv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gxcpxrrdp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gmmdqojxn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/grtsyjpdr.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gjykxnhqq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gxffkxryn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gukymlfzg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gpnsgqhsl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gijrbnxcs.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gnihsgkfc.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gnwwaocrw.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/goimuhcqt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gwtkbvfme.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ggxfnybbk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/grahrbcpq.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gsadvwrdf.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gkhsxpypo.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gjpqwxjve.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gdccfohxv.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/grxcemvfl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gdfeiuovp.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gooqnubmw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvgnzeblo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gjyqdjnbd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gblofnjhf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gymnrjecu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gfqkpwzyy.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gblphwloj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gqhhqehsd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gqmzkwutc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/giphdldwo.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gjielhkpb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/giieogsxr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gynnmgxrx.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gpmmmegad.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/ghbejnbrg.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/ginnusgvx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gqyphfpkt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/grzwlohim.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gvfbxkevg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/geazyiecg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gncfkdlkh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/ghbarphtk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/guwoeuobz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gnhpxggut.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gbbarsxct.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gusmzsowr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdgosmwnt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/giaymuhhn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gmwpxuguj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gpqonmrkr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gszbbzhyv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gttzqbysh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/givzgzype.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gexdcjnfp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/glmozolqo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/geygzczoa.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gikdwuqqr.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gjzjaapnj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/guhtbzple.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gezwxjuao.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gjztrjbfs.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghmbjdlrl.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gflszoijy.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gvtrfmkgd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gefhztusc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtyotmojo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gxckqpghs.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/galvdvaoi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gvqszxlcu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gjluzwutz.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/glcayzqkc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gufkmcuoa.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gybumyrtc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/ggnoapnag.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gmmccwgpw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gitiatazj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gzdaurksy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gegjobppn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gesfgjoip.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/geuuemgew.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/ghiorjphe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/geuoffrux.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gvamdphjf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gvmdkrfdx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggbwziynh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gwvlohrax.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/glaerowuw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gfqhgagoe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/ggxbuvuwe.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gjfpwkmio.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gxwtbzvcv.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gyhtolydm.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/ghrxquans.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gselhoqzj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gyllhnicp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gwishsouw.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gwymzulwz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gfqajwthw.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/ghhwmuzqz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gpubxbcrr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/geunjzefl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gmscqucwl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gfbnqrgex.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gjesndjvl.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/ghtlweotj.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gnatwclrj.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gzonchzad.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gvcmtrcyw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gajeandei.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gfafanhwi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gewgtvbgi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gfnxseiel.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gnlbimhha.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gkzhlolhi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/ghzerykgs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gfmnvdfba.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gagfsagap.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gfjvhvjso.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfyambfvy.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/geuokyzow.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/grobrtmaz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gvybujtml.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gubxruwpc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gcqbkyxgu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gdtscloav.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gtaalcwlu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gdvufejwo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gmzomjcrv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gowhofsdr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gelhmdxmz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/ggabvpslf.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/ggjljkeoa.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gxamkpjez.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gppmvtcdh.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gakdxqynm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gqtwuatea.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/grzvksrci.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/grbqbyjtv.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpgezobtp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gnkalesjw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/glcljvlas.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gnfghxxvl.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/gjgrspfpq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gokwxntol.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/ggvwxkcdm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gkcyviwns.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gbdckmbfg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gmkrozrrv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gueodmbms.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gzrteehpp.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gqbscdapl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gvdmafwyg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gcrukquet.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gfxsdhsks.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/ghjnqzxwk.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gvfsmijha.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gdykscavr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gjagkfgni.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gmooaaohk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gejhrhelj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gdzxidukp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkemogceg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gicqxkebp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gqktegwvb.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gqdbrwdrc.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwojnvcch.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gioxgghkx.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gjpyrieqk.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gwaelyhug.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/glwjbexzo.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gusicouuk.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gyszdsqen.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/ghdtmdlwj.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gdmbfnxyp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/glkrelpzw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/grkufjxcf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbxqcecaa.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/grillgrca.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtykbbkwf.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gaytkgpzd.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gurnjbzfo.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gbctzjzpx.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gbtyqtgai.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gfopigjis.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gedrikgso.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/geyaskcin.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gpjbrzcap.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gagwjfvub.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/grkivusys.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gqaeiiejp.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gtvwhpgaw.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gnficokce.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gmrfredyb.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggkerhgkh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gctabusuw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gdezdjvdq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gzqizljpc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gapggikob.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gaosjrgiz.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gyedbonen.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gvbalvjmq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/ggpjedouq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gmqsztaql.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/ggwgdqaga.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gjjrvqxns.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gfygwfozz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gztgauqds.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/ghqwuxkud.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gmozuxrcv.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gacdwiyxv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gfeopwgex.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/ghkencela.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gkvknegpo.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/grdbqswvl.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gutkqujxw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpbqqzzim.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gfrkrxwvm.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gavbphrdm.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gfjtfnwxe.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gwfcjlksp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/glypjbxft.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gwndvdijo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gxmryuwbl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gcwprngvt.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gzvlgnncc.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gywvyzhpt.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gkiicxxcb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gkqfalrlf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/grdbderju.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gggzvhdqo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/giawrcviv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gamflgquv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gelrxjrcp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gmceyocxs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gyjcfying.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtpumnkhp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/ghosobwac.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gcljddzys.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjdmlwu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpcpmqriu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfqogxxek.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gyqynhice.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gkuabsndj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghinoqlfa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gyznffcwj.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gxbbajoos.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gozqgyukq.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghffwrole.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gkifjvmco.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gmfgfruzy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/grqvhkvfq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gurpxyzwo.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gqpwllzeg.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gltouzonx.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gbejsdbrf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gqhebazlz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfwesqgy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gthgifhae.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gqkielybk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gscquoyux.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gpfuvensd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gmyzfwogk.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/ggcdiqixf.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gmccggxib.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gkrvpirie.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/guvmzvzcz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/giaofcjmn.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gpibnmnxa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gjdigjedx.sHtML


<!-- 参考信息 -->