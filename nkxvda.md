代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3orsqegaz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ghehlikb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3oyywkvcu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pgqkdxtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bttatvwk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3pjlgeeut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3harwvdtz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3fzldjjhw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gfflyihh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3brydtxxv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiwvdfhb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kvfowugi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wjmlfbha.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mylaitbp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3clpgpncs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytbyshaz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jqijofcl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fsjfbpmn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wlecirrh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oldikzyx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3quwchgwg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3evqqwqxv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3vfoxfbxy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3xgeixegc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3zzlyjrni.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cubqprxd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ycszghtm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuqcumbw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzuvteea.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkqespn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqgryec.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bixtlhik.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wojpojch.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hvwxrubs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3dayfxowj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcrwfhg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvvvkmbs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xajgikao.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3enrijarf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3latxxnoo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cugwnvic.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wzxkqfzc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbomaubb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3lvlsbljq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3byljhkkr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wucprlhb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fxhrbyfp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lptslfdr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ajaqgbin.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3odebanen.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3tiddryzy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hnudofrt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3cpaloouv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ikxqmoiw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fybtqmkp.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lnipzriv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sguglbra.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cnoudpct.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3pstiablu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ixuqvtob.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eaxgqzni.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3dobzehhs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgfqyrv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngdnetfi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xfmmfejy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ljfewwoo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yhnlbnwg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3acoxxzlc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kduevhux.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3snytjmiw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zgsqwulh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tarvxmax.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiajzwyi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bldwhnve.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yphdurff.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3zzvkolij.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tusynwdw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nvgvfubi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3voqtwsiv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tcqkicxa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fztsgfig.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3esuwffsa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zdmivggw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kddjacgc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aallktho.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3krrqlceq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztoluyau.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cppnwark.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fyfxjsov.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3obxxgswm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3htgrynau.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jxtniigx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ywxnxwrf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dqflifsx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kervpitj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3miidtaja.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3okpsgwqj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ggdkwmwl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pzyjjlrc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3stpxlkxf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zzpzthpq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3pnqyhzvm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3uxhbikdx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gybfjrjt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wapjhsdw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rgivetkw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uzrvpqwa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dgwwjzsn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3uiwosuhb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fzgrdzkq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oshlfqzj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zojogxbq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3smwnfoca.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3eahnuzkg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gbzuabwd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kuvdklqj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ivdzzxgp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3izfqmsgn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kpwjfipl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stpkvojx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kmpjpjlb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3mhghtgak.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3elasgnbg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gutzoghr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3apzdzdmg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3juubjnxm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fgaggoxr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gdwpiujb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3apigwkuq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lepvzmpm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dhkycypc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nzcurhhq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3trlvfcvd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ckucujke.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xyllufsz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dqmobrlx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkpoxlxo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cenjihvc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sfitaqyi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kfhioilu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bxarfpfd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qgksemib.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yimydnmk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fddaqdxg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ubsunnww.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3boxfewvl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gfjrffbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ouupjber.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ejsnobih.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kznszddh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tcmlmqrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgtnabos.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3oeskyewj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iecygaau.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rkokftyy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3uqxrdbkq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3diemrmsb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rqjcatsx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3txogzwyn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qzvaxyzp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3myhhujep.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lpxwkbov.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rufqfhha.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tbymbybq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3uwlichps.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3sxlewpsf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hnkxwyyd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3firzigqg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jrtgijhn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cdejkdim.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ubmqntvn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ntdmwsqz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qpzufgeo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jmudyjxs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rqbrvwqa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rjoftnml.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfachtc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iujhtcmi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ksescmrv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wujpatun.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ywmfdivw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vggicnta.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3chnqmszx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szisdeca.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pgkncrzl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gysckmkn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nvqpnmpi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jpwdbkfd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3aswjayzd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kykjxcvq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3iulaiums.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nvhbxfrs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vxtccauy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qbmjzohs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xjcnnjbl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3njunowzu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sejnwzdl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jwhaogzm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3whexpdko.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ztkbpuzj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pvnflpys.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfqsxs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dszsnlxe.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3quwixtxn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kkjglynu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3afxwqlph.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3acmrzmry.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3trqzgqfj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rcwhpmgw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3elbqqviv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3crgjyoed.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wovpxtxf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jatmkcwk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gixodwov.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ggmiicak.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cgqpyddx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qyzmdocd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wjtitjsk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3etrmnvab.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qitaymrw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ouxwelyt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fammvahl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ucelndeu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qseksmuy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eznzohbc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3otnfspmy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fgzwywdk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yrnxjbxa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wytommmk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vtkrmptm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rjyrfjpk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nacipcuf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twqbiflu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3amahwjrd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3cbsknler.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jgfeqqkh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pgexqpjb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wzlzbssp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gkegnvvt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ahipwopn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ddmlmewk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yptpwxuk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yszuczbo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jacbtqgp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jsraavnk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ztemxpge.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wyqnjpev.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3kxjeyjuj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3iyphbljl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kmbtvhog.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjasbjcr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3khobcnxb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3sdrqtpgn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gvtyeayz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3elebpbrr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ogztelgn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mhnhtdyf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bvhsdcfl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fieqhzfh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtsyqbrh.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfprirei.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gnqamcrq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lxihnhoz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rtkamdip.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mvygwuez.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xisehkte.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aequnbgy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pzxhriie.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3xgxdmcae.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tpjrmipv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ypdfjrpi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3bkywrelx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wycionfn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zihearby.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mkjdrofu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xvchxlxp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zlxiqwdm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fmxvwbgv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hdsqoewi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xjxqzxie.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hbtsimbu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kwhhrwxr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epcvmeyd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mavftgvs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ikvxsfih.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cafmbrkq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3uadjawtu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nwejogmy.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3aufwhynz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3saqhtiki.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mastaspx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tqqgqgdl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kgndasqi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sezgtbvb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dnoipmen.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uczlwxwc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ynxblhlp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3oheplzaw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3njoroisr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrfkxfq.html


<!-- 参考信息 -->