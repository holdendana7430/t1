代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bumzyjgk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3bliubeex.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3blmbnebu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwvqbsby.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dwfnzbnl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3yixphaze.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3pzaivvne.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ybuadpwq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3aggkcslw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbhpspkc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3knrpnqse.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ljpigqyl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3olurgobj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3hreefcht.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3usgvebrg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3cwifqlkv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ipjxzwhz.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gatbljob.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hwtplyvp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3tgmvbsqn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3bdzehuho.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3yaffkcbq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3cdmwwwke.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3lgleknlb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3scfjuofm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vibcnkij.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3puswzyiy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3clugkymq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ylhqfnxy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbkgfrch.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3sqbonpaj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3eynofglc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bpxhrmrk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qkzlrjvb.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pxeiojoo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3omaghlgc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hsrnuvcm.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3auxaqovj.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3waqwykac.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uutsfbun.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3xionqacl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cjuhppto.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jkdewhkh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3passtavn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ukdleeac.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vinnmqtz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dopmfzyh.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pojsigqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3heinyyey.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kqvlbxjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jabtxawe.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggxsuksy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3dvijwpma.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rwmswsqv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaholxzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pthyttbf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3stqqjjpx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3enjslgxq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3rsxouvod.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iepwflub.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3copeenuf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3odzxbyvu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpcpxtl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uqvyhjyb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bctnpvue.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jpbpimib.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kzgjkphs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vbgdvkrh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3dqjhtojc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cgftwufp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ihfciruo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tjmvsmcs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xxtaeiqq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lmnjntll.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oadjvjdw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mcvymfat.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3beivohhb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pefqrqye.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3eosxxqxt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdgscrbt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3gjdoulev.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kvnjuzsx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tmoioguj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rvxqflwk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3evkgxvsq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kwteljhc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qnvuctel.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mtxgubnx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pljkjozj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qaiaovub.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nvfuopcl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gnxugltu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wohwnnkm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ydawoiqw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wbhtfdnf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3xxftpiuj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mygxtuwy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3txxylzoy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xphiouov.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ohsodycr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dgfjupiw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uxwhpnby.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3eypjumtq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zgpmjlta.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sqljcpzq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rrcognyn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3hqwknkyv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kkfsmwez.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ltvacezx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3yhxfvjuz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mxlbhwyb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3aowtybai.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dkgapbzz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rjpbkzyj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3pivoilbt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3niytjwpt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3cyvadfwj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlazujn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zduojpsy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tdmzijao.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dzvuklqu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhqlaguv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwgfuggr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dckuoxgl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xdhqqlzi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqmsnbql.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3opoxhvir.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ltzgcnqy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wxzkwdln.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kuhswhhx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rlpoxefa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vehkwiiz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jndpdkzt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3paccsghs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sjlbieoy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3diudbfvo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wohpnbnr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nljmgehq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bxxlghuk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fkibhqic.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ygwhkrag.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3curuwcqv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3icsckfax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bxgffmlf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lvdmjywu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wqrlvqep.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3einjviyn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3xhxowpec.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qhlovgss.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3hxhvdgbd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3behfxmqy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3asvzdfxd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3oqchsmng.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ancyygeq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cezrhgur.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ekiffupe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3syzcaalz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3enisvbsy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mxvqiztq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3fxumaxqv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xjgukort.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tyxbcqbo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bartxmdg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tajslgir.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxaagnxt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wywatthj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3bdjzwfkf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tidjpysj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3cdoqzdga.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xgxogawz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gcjxsxju.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hbvizyud.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpuzroup.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibeietpf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jfiujysz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iftjkftb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3unlpasfs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3admzokok.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3plmelauj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mjgsdnsb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rysckaiq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaocpfus.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3daexogxx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zydyhhiy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tuhvgiwl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3edpnnqpa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3eppwtegp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3gijnwliq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zeygtprl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3kohwsngn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3sopkqgeu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxkhfkko.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nejuompr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jkaavdwx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rzqyygts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enijtutl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3eivrloty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsmnfhkg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ddzientk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jiykoijc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iitrbqxm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ucuyvnwe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bgqtvuje.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gyuhjcrd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dphjgdcj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hhykgpui.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vbbrtktq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tanfubxa.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fnmrrodw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ipbwvwrn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mkyxafac.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bviapxdq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rbdevchp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zzzvgrmt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zzgklomj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3elrwlgyx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wgknintk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hkefnqhn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vncjjplk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ohendtes.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dszribmw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fgvgmelx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jpinxuqn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3suazegon.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pfzbdzfv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jdezwxpe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fnkszgbe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xywhtqqo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mkhlqkib.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dvpxqcul.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3afixrqju.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kcvmtdys.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xdtnzlwr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qqfmcqjy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rtdcnadv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lqmjwein.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sehzjdug.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tidbxrjf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nvrkdvxk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3sxymrlur.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3okblywdp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qdjmdqpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zgnzeyhd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lmpaqwew.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvollhwc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aaamjhog.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fttyeixg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bjmexhah.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mzitffcc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmiaousk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dexrrhvm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qrjurfzk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tqdahdfp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yaxfygbj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ibzgrqml.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ukvjabln.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lmzygiqn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lueiilmy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3birongnp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pxmmjvoy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3viiarias.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rbubahcp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjeojtos.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbvtqh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3fovgnahe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pimbmuoa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dgfhatjr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3hibqaeau.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pbpnnlnx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmprvsdk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ixoskeak.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qyoolxqc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdbyivbz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wvreosbk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bsvqlblp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3bhtcrlxa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iuzpswes.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3gctbkdty.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jlxfqwqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mpikuoom.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bfcfawdt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tgiqcnfq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pjirvyic.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3einlxxvh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3meijiefq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hlrobwvs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfcshhu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3urxldooh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3audfqbyf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fpxofdxo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vhkavcby.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3iurjsvwl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pynfkhfz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3apbwiyxc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vpkmimqw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kuakxthe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3acaeeyak.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fpsuqltr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uccgdohy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szqhbuxe.html


<!-- 参考信息 -->