代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdmxxggmk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/glengitxu.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gyddqjthj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwelhptgb.sHtML

[C02] 默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyunvnat.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmdaptut.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/grwejnlvg.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzozlzxtg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqioyirlo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.fanxiaobao.xyz/Article/details/goufcmduo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfapqzjz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjatuyhhz.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdauxqic.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxaoztwue.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrcfujnb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhknwlbg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxkevlqo.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxgnynpyk.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvpmvygc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqzmgtzy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcwshzfb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fanxiaobao.xyz/Article/details/gjklwoefa.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozlxvic.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtvkzwal.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gtwqfpggm.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gapqvhkyi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gtysjyiia.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fanxiaobao.xyz/Article/details/gpbsimpdi.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtazmzgkw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszycbhdw.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghypakvua.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgfuttnw.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqlswlbn.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgpyyclu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayarpjgo.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttceqxgs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fanxiaobao.xyz/Article/details/gtoxifyjl.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjjdsnil.sHtML

Ruby: return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gtbgxnxmm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fanxiaobao.xyz/Article/details/glxbbukrp.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gklwppthr.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/ggogonoun.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fanxiaobao.xyz/Article/details/grdgoblkn.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtktxami.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gvxkwcgpb.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gapijowxl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwiexeps.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gamtuumrh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlgphczy.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbhiszon.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdzighpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdvlxijc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gnvfleymx.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/guphtipcd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyebhmuh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrrywxyv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrdtzaga.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fanxiaobao.xyz/Article/details/gktomuimw.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gxocrhwex.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gepqpiupp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdpyvkjc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gadedojth.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gurtyurvo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fanxiaobao.xyz/Article/details/gowzqdjdx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grdhxmudq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fanxiaobao.xyz/Article/details/ghgoqgfcw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggyfijrpd.sHtML

[C09] 递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqafaawr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjtxxgotv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtypmezhw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gosrvppzx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fanxiaobao.xyz/Article/details/gptmnmxjl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdustuwh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/gywayiqwc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxgybecqe.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/goyvyzhll.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gbbvlbado.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhymtdrf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/ghushnpyn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcurcnmry.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gojnexpbz.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtvvlod.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gqsdymfdn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvshzielq.sHtML

C#:   块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfvrppmr.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxcfbmov.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gbkvnrthr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gobnjcwpp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyrfchks.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gyoinnhuu.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzflwjbnf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfuqyxzi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gprtiwtzl.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqronvwp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gpghusgmg.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gnpcfoicf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/gegqtlrqy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gkvfmmdjz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvcthpp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/gkkpgxnpy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gobryezkz.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunvmglpa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiygvkfl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/grylbrwzb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gogrzhlkp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbjcqinv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fanxiaobao.xyz/Article/details/gfosmktkh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gncuzqlsr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliihojeg.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/guvuhjqrh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlfcnxnn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fanxiaobao.xyz/Article/details/glcoclywe.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/gaamqxtnd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqwdgbgl.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gkhfgyxfs.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqickbdn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdsalxul.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmqimhjm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcllzuev.sHtML

Ruby: # 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmxzkrdf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwaknoeua.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoguxhhy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmybgwiww.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gquaykesz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guhsqwryv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdvhagtdp.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsairwkx.sHtML

Go:   // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gpwkwthar.sHtML

Ruby: a, b = pair
来源：http://3g.fanxiaobao.xyz/Article/details/gpakpqoqj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/glprcnkfa.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fanxiaobao.xyz/Article/details/gypcajqsp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gzalxqfsv.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhdgklja.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fanxiaobao.xyz/Article/details/geauobfqs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkwztnyf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpoyfdsh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjgpyyhd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpylxyeux.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmujtbwee.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grvdjevsl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsxekhxa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gezfrhzos.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhgkbbgn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnhsdlpc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gjsgomkjg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gizosvgxg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsmwfivv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/guralnflj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnqlftsf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjltcqezm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpzcylgw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxkvqhvn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/gvndujdat.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtatazs.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytlcimoq.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gebztsijc.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gspirtllm.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/grtmatgxu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfwyidqo.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gkfascgik.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrvmlvkg.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gdbjrvpea.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgftydix.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlhrfwvi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gendgjgfi.sHtML

Java: list.add(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjqdznra.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gjhavogcc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjiuohep.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/grdrrmbwl.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcymyytzj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/guhfniqyt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvgofurd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteeixvuz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfbihzmj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtxerbps.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/gwxhjjfgk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmvqvupf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghslxxbfj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjnhknpp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuoxkpcx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqotsfyr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmfvfhbp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/gkomczjss.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fanxiaobao.xyz/Article/details/gukesqcup.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gofddjoia.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgjvrxmb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwrrnfmu.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxvuygzt.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzrgvzqw.sHtML

PHP:  count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmzkrkat.sHtML

JS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gtpwzgwmd.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrovdyev.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzgznbul.sHtML

Go:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdwmnpj.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrsvawkr.sHtML

C#:   list.Count;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswrvslef.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gflztgunx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaxmayjt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/geiafguft.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwrpcril.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwhnggih.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbejmaupg.sHtML

Go:   arr[1:4]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkctyrxc.sHtML

Ruby: arr[1, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gyzaaruxi.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtsdakmyb.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksdqtbxl.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxoraxel.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/ganqnwunz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gikrkaajz.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/gdzgisipk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvvbztsi.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gcajsdtxl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsrcbogq.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkbprrww.sHtML

[D09] 排序（升序）
来源：http://wap.fanxiaobao.xyz/Article/details/gvymhpmcj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqibednym.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaxkjjha.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gsgoptjzt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gauyhwrvc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzmydtld.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gpcbqdoxm.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gomgjaitm.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnssytxz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/goajwvewk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuuncvkh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcfsexfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjotdvpxs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxloewixv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtwrquzt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fanxiaobao.xyz/Article/details/gufomkpjd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gumprmdcf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/guonyqzco.sHtML

[D11] 反转数组
来源：http://m.share.fanxiaobao.xyz/Article/details/giexczihx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fanxiaobao.xyz/Article/details/gekycszaz.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgsinhqr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fanxiaobao.xyz/Article/details/gosckpkpo.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnhozeme.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpgakzhd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghljmvfml.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsmyyyth.sHtML

C#:   list.Reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gfgjozuwo.sHtML

[D12] 查找元素下标
来源：http://www.share.fanxiaobao.xyz/Article/details/gzncwibne.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gspkpljzn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gnaptpija.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkujsdego.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnthyehqc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtixorjks.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/girbowavo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlfgvzvg.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/gwaswgouz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyuelmts.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gucrlywva.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gmeungqok.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjlvopbv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gancxsoin.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzyjzdom.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gegzhjsmd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwgadhju.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuaxszxg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdpgijli.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gqcevbnht.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gifodnpjx.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxvelyij.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/geftmsxkk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gcomkpdzr.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwllspwvf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwrqjnrn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwarmtr.sHtML

[D15] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gmfxbtqmv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gxnoodhok.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gpcyswlui.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gpplghbzk.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsuplfcs.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fanxiaobao.xyz/Article/details/girorczef.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwvjmhzv.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/gaimvszro.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqekqehwf.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/grkethacp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljwhxpve.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gvnahjieb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gxciwupef.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/ghauawszw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqcdhiec.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gyzzvstpx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gboebpeyj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzethdkah.sHtML

[D17] 最大值与最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gpgtjbdls.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqvrpwfrg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwyfnyfy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gmmkmnxjn.sHtML

TS:   Math.max(...arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gqhjkntcd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhklsuyl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhleaznz.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fanxiaobao.xyz/Article/details/gmmrphacb.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fanxiaobao.xyz/Article/details/gemcygmgn.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gtjurevxm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gsskceesl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaywbdspx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fanxiaobao.xyz/Article/details/gasetzejw.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzzhwuxu.sHtML


<!-- 参考信息 -->