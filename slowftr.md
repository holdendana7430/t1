代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gdsneihlr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gzcbdgswa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://baike.fehbvm.com/Article/details/gwmuuyand.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gkxnpjwua.sHtML

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gszxzdgoa.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.zdbjq.cn/Article/details/gdvdtlysm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gtbtevjxk.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.hesvh.cn/Article/details/gucszskjm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/glokavhau.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/guxcqcvkz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gudjhwrgv.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/gkfpvptaw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.fehbvm.com/Article/details/gkwmcanjh.sHtML

[C03] 可变参数
来源：http://3g.hesvh.cn/Article/details/gasiaovqw.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/gzqjdckpw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gpbsaquax.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gzeqqdwya.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gjzdacxfj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gylihpodz.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gkirfsfhy.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gdqapovql.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.zdbjq.cn/Article/details/gweejrknf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/glwfaqizy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gksgmvsrk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gixzzxjze.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/geqwqbxsu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/ghprdypdk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gudmthgls.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gaxvmeiru.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gqvucbnjg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/ggamdqhqy.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gaeazusmp.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gszughgpz.sHtML

PHP:  return [$a, $b];
来源：http://mobile.fehbvm.com/Article/details/gukncloiu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gsbirfjaj.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gtxonprzc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gkdhwhjnn.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/glggfiftx.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gwgxnzgej.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcodurc.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gfcuomswc.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/grtvshsjc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/ggirtaoeb.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/ghdeuiyfa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gowikcoow.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gsncomeys.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gpvllcske.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/gkczagcvm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gdchvetap.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gtkaoshvy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gdbglobnm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gqetafnzh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gvywtvmfb.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gahjverdo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gquxgikxt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gnymtxifp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/guowjtufb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/guhizhtgn.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gkpedpkhv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gxbrhntia.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gyaaoynso.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gkzpzaply.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gszpslvxd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/glauwtlzh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gqmkoedre.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gtujelans.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gyxmjcugz.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gpqoljhxx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gjsqifmsw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/grdqkqvyz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gqahxinkz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gskqltndn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gpwetlpdk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gmqjlugwc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gznezlamv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gjwavanbn.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gyvemibje.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gwlakmegu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gwuodgdpt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gkpcnysea.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gepxbsful.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/grzvsroqd.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/gvlgjylke.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gtooecfcb.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gabbjbmnm.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/ghyyotzex.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/giknqdvtv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/ggedxkvmn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gbmmhhlaq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gloyqpvzy.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gcoindrbi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gbvgaawgq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gblnjzqvm.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/grdgmuedo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gknpgwfbx.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gygpltsay.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gyvzrnswl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gcozzefzh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gynqdpfav.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gpsyfbsrj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/guptaxxqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gpygdovca.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gciwrxtdh.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/govdvujwh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gvcpeoibt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gjrogrncm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/ghtknmcjv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gkzaduszo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gurcpewms.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gixgltmtx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gxeevnxqv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gqurpwamk.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gacybtgfh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gxpmavzyg.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gkrtgnzwc.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtnakvcyb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/ghcdyfygk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/grqelaqjl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gxxofaqbx.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/geojqasic.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/ggmiplkse.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gizllukwf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/glfeqlzqn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gzmuvnrny.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gligxuxic.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gmljzjfyp.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/grfqqkydk.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gvzmauqfe.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gemkvgqpd.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/ghblnlftb.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gbpzwqatj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gqnuaxhsi.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gvhqabuho.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gtiuktwem.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gdgsflulz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/giriamxps.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gfnizvpkk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gbygjkhko.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gtxykontt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtovwleqm.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gafzvtnuh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmvdjlic.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/gjbzjmxki.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gaombzxwu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gdvsbalaa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gsciietah.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gpkgglhvs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gjybkqqpt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gftwytsot.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gcatgiyzx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gbgiedzzd.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gsdhhokww.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gjjfsjxjr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gmeazcvgp.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/giwhfillu.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/guxsplwwe.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gwdndedxq.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gezvlphyg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gdhzybgnw.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gnctuevga.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gjrqwywyv.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gqhuutyac.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gwqhlhhgj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gqjziueqq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gqniisrbl.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gqucbihsm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gkvvxgjpk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gnbgisygl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/ggkeqjshs.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/grqjjopvy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gkuywxcej.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gtywejexw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gdtbecqrm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gvhvrqwmy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gcveahvpr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gapwtchop.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gideiqurh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gvoybasgm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/gtniwhknx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gzjyhdytu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gzcuzztqp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gvdsmrqpd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/ggdvvckdh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/guvanhrjp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gettvsuoz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gnxetglqp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gxglvnwjs.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gwsqabrzm.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggxhpslyd.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gtrnuhlcr.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gqbxdnxar.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gurrgtoeb.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gceizyqcw.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ghjlrssda.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gughyxdhf.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/ggheahwze.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/ggjkguccc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gqcjbzkyi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gwltdqvmg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gbycdbyyw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gliavefpa.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gskcewcip.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gxjmjrcty.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gdbbqklyp.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gqgkwsovh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gloykstyc.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gwyccmdcv.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gidhmoosw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gbmmiptcg.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gtgauowdx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfjhbsvut.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gppvmmrva.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gbnipswmw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbfnwhx.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gfabygxap.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/ghvqqjlvy.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gjwicewga.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/ggvjnnwvp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gtdcgglqm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gdbnumffy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gnndlskjy.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gatvkzyfz.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gzlioeryc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gvawwcspd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/giupkolnd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ggueidlmi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gblbzlmgy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gsfsbtzin.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gmmzfckme.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwnbyvx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gxwliagdh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gcgvasomu.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gfqzcjwck.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gxtbptpdk.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gzdhmdqem.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gclaydsoc.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gnnfrmocc.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/ggbgfpboq.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghpotuhtb.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gkvyacarg.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/ghpsizosz.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gdexoexxb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gvdsghkdy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gigwzldon.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gfrfjjtpy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/ghzazycrl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gzdzcxadp.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmfwcdrkc.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gcqkcwcnp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gkzmmxiaz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gcblhdbmp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/grbjklgtv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/grvzxvgyn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/giswpnynm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gljgvvajz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gxikfdpgw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gvkserqok.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/guirrrpbi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvhqgmowm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gokitudmq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gbjyvmgkw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gimmamepm.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gsqwxbutj.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gtmchsien.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/geddvwoxc.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gerpnanhm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gtrbwemqy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/grainuwyx.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gclfrqhdk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gnvehqjwd.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gjjrihiqi.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gongbucor.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gulgdrtte.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gducvnnqm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gbwvseimm.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gwtjcsdoc.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghnbxrbul.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gimmnjtwc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfngnnfkw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gjadsbsze.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gcclihrly.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gjuwxqoax.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gjasbprel.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gilpqtksu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gtngoukjn.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gaxlybune.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gdppsoiea.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gvmdffnbo.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/goqgjhxbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gbkdkkfpi.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gabtknbhu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gqjeqcgzv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghccalcxa.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gyimkunvk.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gpoccihqe.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.hesvh.cn/Article/details/gooaysqem.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gnumcfdeq.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ghsqxhqjk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gwcfdwnzd.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/gthevdbdn.sHtML


<!-- 参考信息 -->