代发 wailian999

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mczcezje.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3clvbkyrq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixgrijen.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zsyoslsd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vvqyvpov.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gagvtgau.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gmonmpfe.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3srxhiyno.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uxvbazms.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tponsfps.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bskopqpo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wrhntthp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3scgvqbty.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3iqxwwnmj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lrdjlfbp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vguhntri.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkmcswft.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3fdlnfhoa.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3vawtipbr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3rpttfafa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3obtimyjs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfbhnbsh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xidmzzff.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3evcxozvn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xwozqtuj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lvdsaonl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cwyzpvcb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mwszmjrb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sphwkirg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wicbpysk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xilknbnq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tlbgvylf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bmqthxsj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hnjcnylt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bbcmogka.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3umcktpnz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3cwyemrfs.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3vimjhgwg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhzzpcxc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ylrltcsy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ukgdgipt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xnqrrnaf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3jnvdjerh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zhrdfhra.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bitpdvgg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3sbtiddhr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3xgotqelm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3xaydraqp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qxjhveor.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xlivydwg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hngdwctk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xcvdaxvi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhovcmr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3iegbgeww.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3uoyoljsa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ypjvooyq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ndlsrllb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bcebqifc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hvwrjbqa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3nbjhmall.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3skgouklu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wlmifpeh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rejxyjhz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wppyxmat.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oerniwdi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kyzdcxhg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3awoiwkym.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3swkiabhz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tgbbmadt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3clgovvrw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eoyytbkx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ksbubrjf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xuqtwfsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3dhbubbta.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nrcehwdo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tcbqnxdp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3orwjtsou.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ksbsnyjn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uexgbmvg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mcmdeaxm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3evuwlwko.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xqvbcwvy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3quviogou.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tfbrwoim.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gxonvxvd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3olsewlpg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3cxkdsryy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fnnolloo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rwigoair.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3arvldvpo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bqvhxrnd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jqetobxx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wexhgxnt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3oepvgmzd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sytrwqqr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3yecswhqf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3muyjxewg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uygjsiym.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ridxvzpq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3sqximtfk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3fegwljrf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3axjsckiz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3notiakab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uomnbdwk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3flcmnuxd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nncqmtpq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3decqpwtj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3iecprfdb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3oorusqvy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3izuuijrc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fqpyrsyr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3abyljtav.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xqmkjkhd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3leqqojbj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3adqezbmo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jtmpvzzw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3srnoremo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uuwcbmqx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xxkshyis.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qbclkwed.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhhuxqdp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkyhenxt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rodpiydw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tfrzkchc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3rocbrlcq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qaknukuz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3icjixrss.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3afdtnysi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ukiqykhx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3snsxdzfe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xeqhxydy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oymuncku.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qsqwoimm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uuufgaye.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3necfkbvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usdsqzrx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3winlfrul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aoewszxh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oxllpjxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3xygirmxi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3aacvglns.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fbxzvsyx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3njodzcrf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rdhucryp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qmfhqpjf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iqeithlg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dvzlbfsa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mjlqijct.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ggnltyow.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fhiaoyph.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pvrsihvp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fgjglxlu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3obtnqkbp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rarvcatx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ehbnbfqh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3puocrjfm.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ubkejgeh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ojjxiiso.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ewtbnkss.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zqgbvfab.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dakppfgn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uekityep.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hebldsgn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gnacrlqr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vnadvfhy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3smtzgijk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3feanghlx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxxhdrth.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bpzfgofc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vwjqnokc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3irfgrpdu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rjggsjtk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlsnmjhz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3oilojbaq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3znvrcyrl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vvbeuaqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xwepaxtf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dzjxvive.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wflpcazi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kxhtltzq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vismzltn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rfhvrcgk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dfeegylq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mmbtupmx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pyyoawxj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcmsouaf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gykdziin.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mlymngoi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3polugzgd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3typynjbk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hvewisej.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3olxlwnlv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bdmnlsuu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ynuczxfx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rauyfwjt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xcmavdnv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3okvbsdrg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nyskxjkc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ourmnrsm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gyvonzmr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3japnjjou.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lflbqlze.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqsuqjl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bxkerzha.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tkmdxaxs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3zvnczbek.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wnkhnjpa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kkrsoeyn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3taicncbx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtnhrzyl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mmjgmssj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dgbaldwc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eoppsqnl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3npwexvyu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3durqkeld.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3qmdgagpo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3blttojga.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tmzvgqmp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3quagsxfz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yayaoblc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbwtlyf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iytlbdvd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3makjmaqh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zxeaurxu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ajncciby.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3onxhqgkr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3dqirztch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3leyrqgut.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xtlffizf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3azbqnqlv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3clqjkceh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3idtakzse.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gqpqiisd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nawqvpzr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ktxjibed.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fjcskhao.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bwdqthrz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3afonczha.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fezbibsm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uqsdocny.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jlwrnbbe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3picertsl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nrwdkrxm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gpptmcxs.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pnuihayg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cvtnettf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3insabztc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zycsfqte.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kgxzfzuo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dynruzzp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gwtpyoul.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3pceiwwey.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qakbmgks.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tgtfmpjw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlnkvvll.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3olkbvyiu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bifzwzko.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pjrvbnjf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgbnuekv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qqfrkesu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mxkeniit.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yolntpjz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gicflada.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3clqfatte.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ksklzkuw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3twwpbgfu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmizurc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ysgxyprm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zhgwfuns.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3cmcoixvi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hhcwombr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ckjzmqfh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3mbkenzvk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fqvfcltt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zbgrkvtl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rpkubnka.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kakvrtnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hamqucdp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ropkwshu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rmkorpyu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hrttgfay.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jigfpugl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kawmrbid.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mixoofwz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydetofou.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mvpsbcbv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdeqzoir.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jvqoklhk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zkyxywuk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dhbyazju.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zpdkgkjp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vxmbioaf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cfjbcsfd.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3edyodyqg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3elsidigq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ntxnirra.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3maongauv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lugzeyth.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gplycqqr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tlwijucy.html


<!-- 参考信息 -->