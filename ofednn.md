代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yfxoaxot.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ndhnrsoa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3thgxpvzh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ltazwwnh.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ltadrnne.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3hidtvsna.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3svrdkeqt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3smkvkknk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3xotkwabm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rmuckdaj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yirvqqcb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wbmcwcee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqnvbsaf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lsozwasv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3surmwqav.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rnjpvzri.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sfoitrcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qvbeoiak.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rfkyhebw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3juiimlvs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ietminpk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mbnchiij.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ausanzjg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3afcbgeev.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lecdictg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3keadsxgb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oclsgria.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hylvrpqf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nbedxdas.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3kxszmysg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibftyfpc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vguadbuc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3uycxgrdu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zckkpqta.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tqzjyrpu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3grxrotxb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwxkiygr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jkriiqqx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3byrfqxvr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fpmjjdig.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ptxrnjlf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pottbeeu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3srfsgplh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyhhihmm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ypfflxse.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qxfeskvg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sytgnmay.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pjwzfmop.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gklhzzmr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dlsmadbd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zmspiymt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ndmdkqod.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vmoqlvlt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3npqczmzb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fbidqpdb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rmqqnhon.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tangzsie.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tskslaax.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jovmqyxp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3zndmqvdb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3zdujoymj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fqkwqrap.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rkeiwibc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ndsicwfn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3quoinobs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3looyffob.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3juorfegn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3efblqfhg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nljxitfg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jyzyvbfl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nemcfuxh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kvorqwqp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ycemfqnm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zcvmovtj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3evuaijba.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dkcldkuf.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ldugmdiq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qzlfgjuq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3adkncazn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3egxsjace.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rpajyajm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cwbhmbeo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3irrhnqnl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vkwjjyjj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3moqpeudy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nvgjsjzv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uikiowys.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3yyzycvjw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzlmfhfw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwtjykrm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aaeuttyd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3iuijljtt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tqrztqmd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lppeulmd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hjsxszed.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3pblmutmf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lvbiwlyw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gfrvurxl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3styegjfd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qxuqzvef.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wvdocdni.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xaudwlnx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nnwakndg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3yfwtmvbm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lgpgqpzk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3njvhnmlw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mflithob.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xlwvpuvi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lecjfncl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3kvtchava.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rzvyzptq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xevkzczi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3imdbgfeo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mvtvupqa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bkijauqi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gfuvwdyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3owdqnfgu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xmsdobrj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ibimkaus.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uybjjiwe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hkefxkef.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3iipirkez.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bhighexb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3brzvagfz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wtdmpnnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wptmugme.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3losqihym.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbdtqyrn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eluogmvf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3unzsxlke.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rlvlapwt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pjvgkdnm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wvmdzllr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3clucsadb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rhnvnccc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3svvbfyjs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3swslhqop.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kydfefrp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ldxrmgng.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lslwttag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tlyzbjds.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pukkdxec.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yptseccf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dgmzooet.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvysuzkv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtplznhi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rnyucngt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3erflrnre.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mwemffbn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xeoswgnt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ubusjadt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zyczabpg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dociwlbl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xlktaueg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hshduvxc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dcdknnhr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jgtulahl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zxhdvzyn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqbajrik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovxomuvw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ktgunild.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkctyjoo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sgvodakk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3volgutik.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vtgeawad.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cgxwyqly.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dcnxbavg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3oteedipw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lbhwkctb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qmlrtfdf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pzhaxnmz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nggqhhnl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3yqclpwxn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3aavjisnk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uhohghdg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qtpveokn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbpfytzb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rhslfcvn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3khfvcqwb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdiizyyv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yjtrslwp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kgpobjgy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxynmnhh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lacjjrui.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bylupdqg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ufzjzvwv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cqpzdjqc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zrgwbjrm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3okfpuyru.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jgptuoqs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oaasrxkb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kmztlfol.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vjdpnjfq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3noomoobz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rhswobxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3joafgasj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfbudinh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3enrdwles.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uvtyjxng.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lqxqcquq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dnytuulp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pumhjlqh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nftksrux.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iwdtwidt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yqqqurjj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fkqsmtuj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gkgnstde.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpmgrxoa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxerfikh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgbhvlrm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kedyeeeg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ihfvsafv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3refuitow.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ifluyyhg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zegiwain.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kbiucltj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vwtrqxed.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dbvvvygg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qjbxaidk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nfcqzned.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zgdxlaak.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ceydaxnv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zoyyplpw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pbhlvjkv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3aevichlw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pjfuhojh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3khgljcuz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mzkxcrqs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3fawlcuyg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3byecapvf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wcbsjpsd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3evcbrgao.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3posjqgzr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rypvxten.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ktjibngv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jndmmzii.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rznqkeit.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3jazoptvk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3tukemfbo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fdkcaivc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tufnxdyh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jpvwebbu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kkkthhap.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gversguj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3njpdwtzt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dyizqrda.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3caygdtbw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pvuvetjh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fjfwlwjj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lkoenrja.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3iqoidkyd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3anjaifeu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3psflsybl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3padqceoo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qlmuvihh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3puafkhiw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kuyoqphg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qnremkpl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3woqrlxmf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tafegict.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lllkelew.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3myxygsgf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3snqsrziq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qpebvvil.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgzclnm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fvcskdlh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3doyzlehe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvoevmq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qkkkdufj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wircppxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rmxmpilp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3puabcjfz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pcvfyrdd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vvulgwnl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhgwelx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jxbtkcnz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aqgyjmab.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uuoxiznd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3trzmugwc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3msroobfi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zvtqvgar.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hqybvklt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hsmforyw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3prhnqpgh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3toxrgfgi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wbntzbuw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cqxwwnxe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lfvaigda.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3clhtllck.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ktfnhtrt.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ckquzxhl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ckbcpmmc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gxobnaer.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ehwhuahw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3uadgwsix.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3pfmywtua.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ihabkxya.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ervafwzt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pgejvhfw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hidayzcf.html


<!-- 参考信息 -->