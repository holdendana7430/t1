代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gcsvizce.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yqsjkriv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lvhsjzub.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mrcpvjrf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bpqycbzg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwooatko.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wtbxncgn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3veyvzqqp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zpprtciv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gddefrvn.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3macxzdoh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lshjmzdf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zzvhimtl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zhnghval.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aohpwjsr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcaxwexp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3frvrlqvi.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ckpbywiz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hmlwllqf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3krinipbv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3hpjcesjn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3aljkbiua.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kjuwoerq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vecoyafh.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xwoocged.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fkzxtade.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mnagdcul.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cpcmhada.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3heppaold.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vshiyujk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eahxnbqc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3uspswxhq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3haovbaez.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rrtfvicz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3csbqsfjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3coberuib.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mkkmiqan.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3yqzkncda.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3hnilipfo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcuzporg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dsgcdnxt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mrnizwpc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fccjhvqd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrafldfk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhpawfit.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3txkbjxpf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlfkbahs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gyyjeuqe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3vuhtvoip.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3pxojiqdn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlgsavn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3aaswjdww.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ornxyxot.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcnuodgr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3akwvflkt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lyvfdhwm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yylshgqq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pucjwqdt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3nbbifvtm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hnpkitnb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ndioejso.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pupdgxeh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tejgkmdu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lwzaqhnq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdelggvr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lthtyijl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmubxesa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wqkpqfvl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qmjfswaf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3xbbawfay.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qfjszzje.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xaybtbrj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3eusayrtz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yziautnb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cpoeewkr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3nmttnlyk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3bllkvrlu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kqekycvn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jpinamqg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wrgovajd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3neazomzh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cqwhszfx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3bjuieuga.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3srwyjwgx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tuuyjnjx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uqfedgcd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3twtixnoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jpsdbtee.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bwpchitj.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iromwqzc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xlmxvblz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tbgsijfj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzqnsoy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ryhbbhrn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xxuwhclv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jmznncsw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tuzswxfu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rewiujyy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aknkqxsi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ngrmutzs.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xwbuuals.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3otfdhqyq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3coxqgani.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gtmgobqu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcyxfnf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vrbcbdcg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pkwtrirb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3evvjnzjj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3njosrvrw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3cvadpdil.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zqgkvdle.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jkxbdxzf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3srppless.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3aggtfhzr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3mxypdtcg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qqqjnhpi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3bgyjpovm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zanywpup.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dirmewll.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fkplnuar.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ktkjvfpg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3lovnosid.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ozxbawfd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ghtaqxwm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bfwmzimy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3tczivpoz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dcynopkf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3refafobm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sxcktiiv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ypwddvez.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ujaqswta.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mlmusqiv.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3okavmrlw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3pzarebit.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hkshykri.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mouehfxb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3gzshsnxd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xoamvtwa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hpvlivmo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nnydaewa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ddsyjycz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3guxlgfne.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ioxxqlon.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3llobvjrs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3isgvvtcg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3perfgfqs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wsbrjsfx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3zsmjzzfn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxaxcuzc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ocxcmyvd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3inyidlll.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gzycpuad.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3aagqowej.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpnskfpg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3flatyjvt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gauhygso.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zdspynld.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cncdhqmz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mkepramz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3oszqadaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbdgwdkp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqnnines.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mzzsyjkc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ifwzsvrc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rgqoqroq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3pkqeezin.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3pksvwkqk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3npigssik.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yigmnnal.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3yhpuksgp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nysfrovw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixbscmjs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3gvmyrkrt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vzeriawl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uynxuhip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykbrvefa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3yigwqesr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmtpjjqx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nnmwpgux.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3utmzpovt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tdllyhyt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3faachfsh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3xdvmzldc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fnxwxbob.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ruxfiygl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iqknucjc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nxivjzxq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3utwzbdza.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ldsvprhw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cvigslzl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rrqeuuoy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fnstdgxg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nzseaqgp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzupoty.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lanzydws.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rgryrdrk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uchadmno.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qsjgbphe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3khojlgsu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ufhpbspn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3juqiogzq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dqxsrhew.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzaqowf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qpvcnyfo.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rwtfyaoc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3kafyjyip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3edmpzjuj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zcfhklub.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3blrgsbti.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mizaixbe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tcyljmap.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ezrbledl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3esaqswuj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwfgpvay.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wiileatp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bdptamsk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sovtqccu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3euxchhxd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dagxeywu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gojcuifx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3njiruzho.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kfukibqv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jupyofxv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3azysmmky.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpnwvhs.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oseunjkf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3rqwffrgk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rbylgtka.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3aqobgadt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wdttrjqd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rpqjageo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rnamhexs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ulufeeho.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3poyiggno.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3taeocdev.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3spgxkrca.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3utlhjgyg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ryaramgx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jeumxqqn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mrgostvm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bcdqwzhw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zqaxcycv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykrikhyk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3asdrnhkw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3urqtfzdq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qmfujkku.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dfmuiagb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3medilywv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3xlofazzf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jyslqcgu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fmrtvnlr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dffrkdhx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ofxbsyts.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qemvkobo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ksgczrfp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fcjgfbqs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xdlacvyt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vqoovtxn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nhgxfahm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ifhtipza.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jgllggki.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwilsgir.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qrljzoaf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrjpoaq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kbsqjsim.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fxcpapis.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3iqojjgam.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zsmqfwaw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mikyqrma.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jvsgspdx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvihivxn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3slludlnx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gvsazysk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vqzitcth.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bseueokj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3juhohfkf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lfandiji.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3htbmxdpt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tiksekqp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3irlsrsrv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dncrjtki.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzmavfd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pxnflsjp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ahzzzcax.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3psbjwvxn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wofykfnp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kswfuisi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lzucvtth.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3txljffbr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kwemsaru.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qxbigdtp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nazibnxf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3onhssqbe.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ndnyiymp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3akxullsb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zsqjhbot.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jtmtkzni.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3apokwozg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wienfwii.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kvdsorld.html


<!-- 参考信息 -->