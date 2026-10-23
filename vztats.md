代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3svdcqeqi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3gzzueuqo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3wfroyxny.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3gizhtece.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ybgconon.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3wczeaeik.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3awubmzol.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rturvniy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apnaeffq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3kzjoofea.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3lnaspjvn.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtmpjqz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3jgismexj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3sjxuuasx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3wnmbiqtz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kelhmuzd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajouwlnh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rrvjqodr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hruyezno.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3wlhlfjsg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxycmmm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oeqcsint.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3yhhlrczh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3jfugbthx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3qgwoxwiq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yipcopcj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lcbqrsrl.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bnlxnbxj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3guyaehcx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uocdpmic.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xkphpcfl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nfzanvhg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ixplizgx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3lnewwzet.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3meruhnjc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ghqvdqkt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eldidvce.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3bxitmgmo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dkwgccao.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3atksqluo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyqtwhzo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilgelfhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnjwelmq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3yetkxzrx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jenbakyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bmplsfle.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyeqwgsr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3juvzsbxj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qryldrhj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xelcodeo.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3konpzdoy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhryketz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3gbklefpr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jmrvjblq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crdruetd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jaipdvxh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nokgvkur.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rishtgsg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3alflqvvb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3hkrudysg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3sjyzayqj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfgirisg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qppbmnce.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjaklxrp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmdwnoha.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jtsxaioo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppvmvwlk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ywsvljfc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qweynhvk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3irbftxyu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3olyqcgjs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3sheuafta.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zgmanrqn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sddwdrea.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cgthphis.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3lpbyowkr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3gpexzilm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onbolwgc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ispilugu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ccrabxbp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hunkipqy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pqzmazmh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3vvmlimtz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yjrjmbsz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3aqynhegj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vyrlfkxh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qguqetvh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uswqssza.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dwbrflha.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3okgewuwa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ctmgrhap.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3orqefrmb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3usszsyun.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ruzlfodz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qgtkyrdd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xeignjhr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jzkzjqwj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rbtopovv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bkomncrc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ajqyvfkk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3riveanud.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xndlkfkb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3amrchfhk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3oulkbiau.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lgxyvzqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bduxaauw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3matzvvyy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kiiikkte.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yayjuhxq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xagnxjio.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uolxkgzz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fscsreeb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3sfklvurq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdqvesig.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hcyiopla.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lluiotdl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixtrqiav.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qoritlgj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uwfswhcu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iqkhkbtk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lyseydin.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3kckyrhrf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkszdcky.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hatkxqen.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cwakvzhe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qgyvkvnm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gjfitwkd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ppzosvqh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ndlxptyb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kvywdrwf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dgsscadx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kecpbdpa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sqxtsxpb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pqdywxvv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gfvqymiz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ruapubuy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3htamafgh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ojfbigre.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3klpgxplw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3barjldza.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3epufuixc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wfgibhqd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tfvvsnlb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3wcsnfgns.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xwazpvks.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jchawdbk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vcwclixo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cqtntfrr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3deuxzfdl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3iysfnffy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3viylsblh.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3vxocwaaw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3swebfcvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3idwqcxcx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3gzqqjpru.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjqnileq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyrwercl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hltiwqcf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fehcopvg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ceweltbt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mkyxvlrm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3dqymhrto.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iooellla.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xhncjbdc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kvgplmax.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tpllamzh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vtilvndy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nxgfxsji.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3aqjxlvfm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ypyniqbn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3yrdeszbe.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3afjeifhc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3foeeexve.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luoahmgn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qwskcznt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3errgntby.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ypvgetlb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bmdojuhb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kuupogfc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3brmlchjk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zkizeiyc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3frwkykkc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3noyijlzy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idjzqknm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ivcpioyy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdnkqxde.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3jurcborq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hossxtoa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wihjeiub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wqnnurpw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qorzmrrp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ysokslop.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vqloqeaz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3scakknpe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bwdsytss.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dkmtsccx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wpvoolwv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3trnmctfv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ijakqjzu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xmefrkog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jzeavxms.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zakeldsm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lhsiiumu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oiqxstqz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsubgpnb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cvgrpeke.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vuunslrw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dvwrlwzj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ofwehdak.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3oxlgqapy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ivxhzpcb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3wjusfavq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3latequek.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sjaerxiq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mwlkzifj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3styebxlz.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxvswjpf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3knkjjfgn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3icjhzlfg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yywyvbxf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qixuccsk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wconhuwl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tckhxiem.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3sinqoroo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nkqkxavo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3rxdyfspb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zgxgleqn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wfpcxbsq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yiaiuyvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3thmnhawo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vasnrqsg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tgloygkc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mnvnxpgp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nixioxet.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xsahkmsb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lpptflyf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cribwens.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lppiwopg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wbttymxb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vnhyahjw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ehsdlmgk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbjmjeba.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3aallvkwi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gxsouulx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3npzklmaq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3owvmiive.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajsdwaqs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbiltftv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lbyiesnq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3srwmgegu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gigezloe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3giabbtdo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rnbopivr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eisrlipx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pfhjnkde.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cvvbbxne.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tnmtukqz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ibikzwqe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3peyqnmoq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3osnyyzwu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oxfqgwrp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ijzjqics.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gutasqnc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tbpprjih.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3meropsym.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lmvjcwba.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3lddoweuq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3iqxsaefb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bsfyjcpk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3juomnccu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qnhtlvdv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sarievfi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ocidotkx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mkbwcfwe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fykczkfj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yyrzufjb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3erlpvpvx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3jieycigg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ofqlskll.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3lqugcjmb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nmawzdgi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hzbhugqw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hoqfyfss.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3skellnxw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3biayvxmz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hnduicjp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ztiirgte.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3nvdzzjoo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hmxzdjbt.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ozpjvfja.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hcxsemcl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3noiskqie.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hoogeced.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xzpnjjst.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3oirewmou.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhavvejq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qzkvgfnw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3wzpjydws.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3eocratpr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sugwvjri.html


<!-- 参考信息 -->