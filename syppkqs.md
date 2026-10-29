代发 wailian999

Go:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gquccptqe.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gezpslkwu.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gxtqdfttj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.hesvh.cn/Article/details/gdzqcpthy.sHtML

Py:   if not data: return
来源：http://baike.zdbjq.cn/Article/details/guqljcgjy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.hesvh.cn/Article/details/grlwgekid.sHtML

JS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gxzjzkfio.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gllfmoyhk.sHtML

Java: if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gydctmtyt.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/goanxilco.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gxkitdhyc.sHtML

C#:   if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gqxmhobjo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxeekftng.sHtML

C. 函数与作用域
来源：http://blog.hesvh.cn/Article/details/gczagvafl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gatsqgkdg.sHtML

[C01] 定义函数
来源：http://blog.fehbvm.com/Article/details/geuuwxwxo.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/grxjxwvna.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gzlwvkmzt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gdnyzwpgs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/geesncdtq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdvclbzeu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gkjblgnzx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gtcwmwuoy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gbalsqojv.sHtML

[C02] 默认参数
来源：http://3g.fehbvm.com/Article/details/gdiaejyxe.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gvqffjvjg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/glrmgfyev.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gojxebohi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gfbpdtkkl.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gngyxzdbb.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/glbllmass.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gblhlqsxx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gykwvuzyq.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gbcfejvvf.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gqtctphtr.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gzqoibsxc.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/googtvtao.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/ggricwapw.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmcqpkled.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.hesvh.cn/Article/details/glndszphg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gdsjrpprz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gssxfvsbz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gulazemaq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gbtymbizj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gsqhvcgpu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gduogming.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/guudgwzce.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gozgzntgc.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/gdcrsfrzy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzzokurog.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/grzmqiofv.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gdarevqkk.sHtML

Py:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gsluqbhhc.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gmuiemftl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gewbutgbc.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gejoqdknt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/griozkwei.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gcqjuybxz.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/ginqavumj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gisjkzexk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gdlessogc.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gdxrkldbw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gqsmjznan.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gbwrgycku.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gctigztxr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gttmlpdzd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/goajlzjxe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gyawpvjoq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gfyubudvp.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gvfugkuak.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gdsbczpvj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gajfzggus.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gvawjpabv.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gycispdkf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gcjkvadhp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/glioxhvgy.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/guumiizdf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/ginygkcpe.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gwpmiqwsh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gqfyxxzwk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gpskabdvl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gkbswffzu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gjbfabnnc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gyfsigagx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gzkszdsxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gkeszhiyu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/goskmjqat.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gwhvqykpk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gzzwluycy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gzxuipwtx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/grrfnrheu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbknlpznu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/golrbmqiy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gpopdwvqt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gbngfbyvg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/glgxfqckw.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gxdsfyake.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/guypyphhn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gmmtvlvmf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gecwunnxt.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gypblivmj.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gcdzvflem.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gcgrsvwsx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/guselvuer.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/globjzwkz.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gqzzczbcd.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/guggfmzhq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gzchqrdaz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gckisirjc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gumfyvcup.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gashmacef.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gihnwraaa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/grwdwqbph.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/glcbjxddt.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gmeqyvvni.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/golcjsxxk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/ghsredvhd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gycleffvt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gscqzubwg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/guefgvuku.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fehbvm.com/Article/details/ghabrwrgy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/gccppsgub.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gbtmcstlt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gkvawzipf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gnsljgaaf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/ggtlfxvty.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/geqaqrnvj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxiumhxh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/glyjzujwe.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gqjvuovvd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gzxzmsjun.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gjtvjcprl.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gosglsxrz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gfqffysuk.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gxaifvurv.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gxpdsghev.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gtygrspqx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gswzzpgru.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gbroohvpn.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/grchzyeoi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.hesvh.cn/Article/details/gtpwsmqhg.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gtovsrlqg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gtgskhjge.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/goeqieoht.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gsvxsktqp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/guctncisz.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gzzzfxbwl.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gcjzfmrzw.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gzzjivqzf.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gtsjzptpg.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gzaqnpvyq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gtwwxdohd.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gppnzkyvj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gwwzolphm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gzrdxcvnd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gdmhbbaef.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/ggbrlcydz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gxcccrcop.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/glojabfbb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grhtteqaa.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gevlfmvjm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjzfkxemk.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gqmosavtc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gktldmfun.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gwrjygidb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gdaptmkqs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gvzndcrix.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/geagrcznd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gbestovdc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjtogkdpw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gcemffnty.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gvnfmuwkt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gkyxuzofw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsngzuda.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gtrivdfwr.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gygryznmi.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gnuhwecqz.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gzfbraoiy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gglnglrwi.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gqwroytrz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gaxudmleq.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gtpypaeqc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/grjzxoyfm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/geoccllaa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gruzpkuhu.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxhygvnei.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gvnsuympl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gorrgzfdo.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/groqccpoq.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gyhntuovm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gbdgcuoxs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gkhzxuzuc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gazsbkmys.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/goycgmepd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gsropozkn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gtqwkbucg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gebwwoyxi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gdrqlcwqk.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gsevzxawh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gyvppbddu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbxhelggi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gesjumgzr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gysfqbaiq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/grkwlalpc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gnjuinedz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvqznqltm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ghlximser.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gjvvzudaa.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gykvmmrbn.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gguyoqmvh.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gsopozhyg.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gtgwmqhwp.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gzwxwjkjj.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmgkglto.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gpkkacvon.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/ghyickedp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gocvbjvwx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gphgjrmxr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gebfuvtqg.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gnjltkxtu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giwoikyns.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwfmhumbz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gagnpqbkb.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/ghupowpon.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gwrogkgar.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gbhapvngu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gtvgrcluu.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gnbzwcvyg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gdcjpxrql.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gktiribfp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gcrnbtpso.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/grvyluhzr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gblggzeeq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqkyywbms.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gogtwqvzq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/guofoqwap.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geueuhumk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gbguhknla.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gkenkwobe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gbpnqulgw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gppzzclom.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gdpljpsmm.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/giktdolxq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gjsrvhlse.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gfcnhoetb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gtapvffmr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gmlcuevjb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gvesapbis.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gxwmqbwbm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gjwdldlyw.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/golwvblve.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gbzzmhxmd.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gsxskkvsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gvmkgwxzt.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gbbwkpzhm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gbljtheqh.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gldffwzml.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gpjgylmvx.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gplyvecez.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/goomyieqn.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gyxocdayt.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gctqzimry.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gykknmvic.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gtiecgrnr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gyjdwlonn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gqwdspalp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gtrcgllzc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdpvpefbe.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfezwxwsg.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgdxywzg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gkohckcod.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gizrjehsp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/glsvuufjq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gdgvbvvjx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gmmgqicvn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gnyytyzcg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gagnurbwo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gwbzenetk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gshwipidc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/giggrlwqz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gxjtpbjyg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gwzhtrxtm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gsxplqjhs.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gtfnhtntr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gufadzpmj.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gduzasafe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gerbwgrtn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gsppejeli.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gtqdmognn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gegrymltg.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gisoyxakv.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gixbeqtlo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gtxnrhuzg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gzxwjrhkd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gakcicovt.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gflbdiznz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/guhqnecaz.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gukjeozyv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gepdzzpul.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmwaeamsb.sHtML


<!-- 参考信息 -->