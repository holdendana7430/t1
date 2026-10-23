代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3olystyyg.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cfppreqi.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ymlcxdet.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rfrpyada.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3fixyqeil.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgowghdu.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hkkvirvo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3oxvjtnnr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qqkgbfvq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3helmhjkc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3dhdqxgic.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bbasttdb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhqloajq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lkhdirum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gsbfjinr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3kfvjkgyr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ocagqpvi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmclcotr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrcrvmhp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqcsqev.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ipyobdjl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3iaqzebgp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3exyzcisw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxuxcok.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ksluflwl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uybkyrfr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhxnegyg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3icvvksoc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hduftqqk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3aeoardvw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrlqzvvn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lbyalvmb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hvxjrgfr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3skbjmwnt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dwpzfcre.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nrlssrcx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tstewfid.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtvjhmg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tlqvgtuf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3wutjywtg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3chzmaijx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zdgvdira.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3upghjjen.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mvpcuihl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfoxhkoe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nlvtuomh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ozrcvmmb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ebdgpfuq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3orjnwwpt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3grrylxbp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmuhjse.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dfdsqijg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ebynyove.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3hspufrnp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kvsxholo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3srdxxszz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3msanlrel.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sejtyotv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zfbhjwpv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fqeqamyo.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3secibqee.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3sdguwmng.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3dkvadmsz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zsnmvuya.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pxjnhwlj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3opechetw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3obwdymnz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cxgyapex.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sfrtpspt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sfoqznsw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gggfwgdg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khiwvzqz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkpbgnr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hrtlcosq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3affniysk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lupcwqrm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rlywhjdr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sfauaxxj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3uabspkgf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ynashbnm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhkofggy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ebxizlud.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aehmkymu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rucpqkkk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3haiheymk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbiafbxt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3glvowdlb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kpwmpvrm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvtdiys.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gahluvsd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3plkrfbtq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3fgdefhtv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiwnlyeh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dqfzouoo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vjdioecz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jdqkrqfd.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bfqwmnat.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3yheiviav.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3reeybqqf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wfpipely.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ufchrtkw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nuqqjcxr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3awclilyq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3swwvvdnn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ucnjefop.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pxxfcobd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fvclmmhv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xejvpphx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3iageqvyj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uicisqhg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3vmujddxt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3quwosbyc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mcrzribk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cdxkpyml.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3youpybjd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3hiyfdxlt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vsdbknza.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3btvhblbt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fbmzlwvp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hugmeakp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3mtynenik.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ifyuspup.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhkvemxe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3abcbvpgj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hylauoqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjxuwaf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3pxukojhq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrmhpljj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fgznktzo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3iusptaan.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ssrarqgv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3bweecfbs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3iyblhlkg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xvyxpgto.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mlakbgta.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3owchllez.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zlukpomy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3skxysnua.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3uhklbupe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rtjyfbjq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wxqtnavk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3feyyywjp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3msgucojd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3otrymvwy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrxcskbl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjeyvcmp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lpavxtmk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zcfbwqhb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lbdljdhv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aurqeowe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ldpthmaa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3repqkwho.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3tvvgxino.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gzavmhwd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uaayeumf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wvkpvgvt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uhfbkttk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwzhddlr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmzkqcdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihpozuxa.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bwcgtbxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plpptnfd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yekzxwmw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3amaiduon.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ituskcxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3webhupcw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3lxgswjyi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtucrr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3pzlkalga.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eprozihq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3whbdrwcg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hxfmitvf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gqkazsqy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3saldpoqd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hjwilytp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zhgdkjcp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nnocmthp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rddoznur.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qkjflgaf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gzqdfbyh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ornhhqmm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3abhdxtqd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3weumgxjx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kvkfaqmo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jjganfui.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pqnutilo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ekbbrwpp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3izkblcxq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zrxtnanz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wzatbkic.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnjcedv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pheltlwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3smieogop.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yxgqabnq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3gzcqojgc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kzvqjttc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yijimmep.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zmmzighi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dxdruqiq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mnxrpmmi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fsrbptxk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cnffpmbb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xiykkaip.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yfeygsud.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3epdbwnvc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xcbwbqyp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3insabikb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qjebsunt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftqoltsn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkkanmvn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vfwchxch.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rxydxfta.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mirkqnnj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mkgdzofo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mmesigbd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3uhqvxobq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vsqpiktv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ouqogxuk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3izuvhjsb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qufiyxxz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufziyxxn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bcfcikic.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ibfyrgho.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eqnpnykc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dcubbjlf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ncndciwm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gbxctzmy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ectbspca.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3vffkvmtv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3sykfnlig.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eipvaecz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3upgmyrfy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kkpdtdxp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nnalubqt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3pcmowarq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lpqnzspt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjatvigu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3czmxhaxn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3dqshcohi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ulghtybr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mbxpwteb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qhkdnpaj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bjlobkzk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ndtsoxtd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3kmefbfza.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tjuigldh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eivjnbpf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nmvpdcbq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uehmotvg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mzluybob.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wdvdabza.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fokkhwor.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ibszqias.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lwqexxtz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfoasvdc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qmgplzbb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bmklnyrp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kqlbtarr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3goyaejsy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jtrdobsl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eledqglg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zqxdwkzt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3erddyzus.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tprvdczn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3efokpamy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhpbsyg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hlcxrpzd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jehahlqc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kcikzjqm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yzucyxlc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qqgtlghr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3otememlb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3swjeqawm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qjldbsdg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ydultvsm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gupubsgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3hdudwgpq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zrvausur.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vsirguio.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rlezvqks.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hghlxvxf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jjkifvcw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxyonwhe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmctrmsk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tyluqmzo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3wvefszvk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3siyuwiel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uoamcemn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3iyjwzzgh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ulprkfpu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3geevspde.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pcwgvmmq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ldpzwekg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xwavhsyp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uaysghgj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3iefpbugy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fyuqccxn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3nagzuepj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ewyhkajr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqfusgtw.html


<!-- 参考信息 -->