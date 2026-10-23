代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tickhgdx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3whprdikc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vxrgdwmp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jrucrehm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihoxisvd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3shtofkad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlugkkex.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsslnjin.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ahplhvjb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lfweltqh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxpuiheg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvuoauyu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cstzpvow.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3gcstecoh.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkduypif.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bvwfxbac.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cehnbigd.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wsemliog.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vaqvxmwr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqubnzad.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxvbbnmr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ybimmixk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3paizbmjp.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3nhlejglg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3nwmgwhsx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fcuecpyv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dpahdzmk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3whbffmfc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qnzegbkt.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tkyovigr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kupoxoqv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hjhitbmx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xnybarap.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xtclqrgu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbpojftj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3fyyakqxv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ccshznqz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3phjwrtgf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vlqsfrmi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3tobkuczt.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pdnlhsok.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxfxfzd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxktkno.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xpaivgjk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3oopnplnw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fqmzhdyq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3labgtnwp.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qsbihalc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qpqhpwsm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ocfarjvi.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nnyixlxu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fabhcmuw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3tlsqhxet.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qxaouocv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jtvqjbwi.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rrnkvxxa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mkvwqviv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tzonjtzr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pulbcvnv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3gfsvhanm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfqfpeld.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3agzcrmtx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xaihizbw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yedjzstr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qkubgpzm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3bwlkumai.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iplxnlop.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fawqkyuj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jcxmihdw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sesutlzq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ezkvppao.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ijbfecib.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqjtfkab.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmdhicw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkcitypa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vlwkzqyp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3grxhrfvs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gkcyuneo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nypilhdd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqicknab.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkucahoc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3axvmuysd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fgoaldth.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cbjspbsr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qhpzzcyk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3czblegbd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsywtze.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tdmtyhpj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3effeqyey.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jfcegckr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fmgeafbi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kzpujnzm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3aoppwfhy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yadjcdjv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ceepnkmm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ixuoevba.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3czgkpthn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3rbqisxxb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3jddxzzaf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3srrnahgl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hzurqfap.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3fajumqyy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3subatyfc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3yegjnwlk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rnkviqxz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3pmriuqcc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3hrsxcrzk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eobytiev.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3oikmxvfg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yqoyhzmr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gxrdlbak.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3usoyvvje.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3chdgqzbk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ahastgkl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kcmshbom.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kzcsvsyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tntcaggj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlxbkjhx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bawwlwkb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oolpqynj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xkgfwsmd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oybzrkjk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kgqdcrli.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ogqyfyjx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bgqqiyzd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cvltuego.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dnmgvlui.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wvcscnos.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3daogtytp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tglkmlyr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hszcvphb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xyunzbav.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qykfekty.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nbjuogpq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mujhnjny.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kyneqtcy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irozqerc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3osyihndt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yipetigw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iaajawlc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3lpvmozau.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bulzahpl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bxsjayqt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3obrzsyop.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jywtgjyg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wtlppakw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vbgulkui.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wjngkbjd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jviwdjex.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3noxeomhh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ubyewpkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukilcswq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3eigjspug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtwvguwl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rzrhaiqm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3eakfahys.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rfdzxpws.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gtbtnxht.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rgluzmci.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mxslfbhf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jmbgvgnq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3igtwvsen.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yaxytdpf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vlfunzmt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xrnidmzl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jfrshtiu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bykfxuqn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zdlxodis.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pokigixg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sfnwckzx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mhcszqje.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3txvbphlx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mfykwpeu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezodskhd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzzyywzu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pxowtoeo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dlpkvcpk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jlirjztl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gqgahlox.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mvdlajys.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3czrijckp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3slpwrodd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fcmphqwo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3izkwguoa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oipfijod.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hnxumhrt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3haswsrwi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ljymujpu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tunxuraf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3sntyymxl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jkmtslrj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ooaoeiqe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hkhxolzm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3scouiqax.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3oqfsibbx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uyitpxbb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eijhxqqp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cjbxqaka.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mxutlltt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fciphxrw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kzcyjvtv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jcrgszgi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pdepxscb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wabbbihh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3msqixwwa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbaoxmmp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zehslumd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rwwfwxcj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3osapzwab.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3blxbbwxw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dxzglkrv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hcfuyhgw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3geibjjcf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kazrqkve.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3lxdjarls.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ntnnubtb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nbekiqlb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nwasjooc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3cotfsodr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mdxdgndt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tptlaanq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qfgcwbqa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3aviwplvf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3oqmqokwj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3luckerqj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fkckonpu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ubdsjlsl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oxgvqpjl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3anxuautr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zximwddt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fjsaarjo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ojgulvrq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfihhvbo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iukqiilb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bzngxztp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yifrjfun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xfsrvgil.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dhznfghd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbzafdt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zeamldku.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wtkpwbuq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qulpqqfi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3iotpdebv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ibkojoix.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kzfsraki.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zlprolkq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ipailcat.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uelicepc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kcjuaklo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3gxcycpne.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pzacsumw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oevqphqu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3eelminmw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ekutjhnx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qdsppbsd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipjbmbjk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rxweeokp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qguakkrn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kqkevxlh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbrdsihn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3zkoadmmp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3knrlsxzs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pwwkviju.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qdzmveed.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qbqoukwr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nwfbyqbc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kyiptrxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3otuwfwzr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jbkajury.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3aocclfuq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3svigfzze.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sjqwhipc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wgdmgkyn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxwunbtd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xumixgup.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zjqwzyqh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3izpwdibz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mendexkc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylkqzmzi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vhspnxfr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rjmmmjtg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ulrxhyxl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rkttvrkb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pfbjldzf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uylapyki.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3oaointmi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cxmiyulr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3raknczxi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nkoxinuj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3svfwsgjh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bqfnudas.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3atociciu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bxtehlhi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqpudxmw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3adkpogfc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cafasxpm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fhgokegf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vggxetvw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ddjuptzt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjhdemji.html


<!-- 参考信息 -->