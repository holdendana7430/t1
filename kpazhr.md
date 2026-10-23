代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3paikbofv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3agpycrxv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3grvsyfiu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zahgavui.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bizdooid.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gjueaaog.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rpkejkfz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lfuhpmeb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yiukztlt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hyfjuhir.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ykyfvhib.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3msmtjekw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xwcdongj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gvlyswkp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3udfizadb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3jsjxacvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3stbdemtu.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bdkmodwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqmobvhb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwescree.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zcgzlqen.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkirajps.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxkxtzrv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uplfvmzd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvoiccya.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ielxwwau.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ukwxwlsg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibkzwxdb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3oyqvnrxq.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gucnslqo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdotdiid.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nztyjund.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mkirahjt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wkyzpjzz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rvlqwtno.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3sndraitz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uzncpfjf.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3nuajvslr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3oaafkpwh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyoztrov.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyfnbkbb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrrppmtc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3wypkajpz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xxiqqwzt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3lajscznc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lvbaolgx.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bggcoxox.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3bpaudpuh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3yxqyoosk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nelfuhuj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cvtypkoa.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yivfdedq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3tpusclxr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdbumre.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ftlocdxm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zdvnjdbp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3shpwtaxp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3osnxhrod.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hfzokxml.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fgsjdoii.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wgldnlhj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3uiswymbi.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3iwgtthed.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3skifwvis.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dpfgfjyf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wvxmtrgx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3wgsdqlte.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sklozkap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uhkgidqh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uakgmbox.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gugwctid.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jhllfzbo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3smxvxvci.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bkrecwdv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3drxkzbsv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vjohuncw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nnjufjab.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3affhpxzc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xvmqrlil.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3noikpkql.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rxuwgblv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lljrmfzx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3sqkbujaf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ciwnjwpa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3htyuqpsj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptaehkgt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rjyhrzld.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ueackfzl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3efyyrcqj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3bcxmjgnm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3muhquskw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3uafyjbuj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdhamxo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpvuugpt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pfxurima.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3umrlmatu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tjfqpakt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ongrmxdk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kmthdwkq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3kisjgqjn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3bvmzyquk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3lwjheaso.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kkfxsaff.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lmfxpogc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tskloccm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3irfktqyg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mamyzdqj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vojjhnyq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gpkgzbwu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3npdrntou.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3nruhagap.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ozcztzow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nmqsvybf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yxlhlyzj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tndugmir.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ttlepopp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pstclfhu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3npfvaqrz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rbbhmwca.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3veqmzjkl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ckrjlyib.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mntityfp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3snmsfado.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3uxmcazok.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3cpohcrqv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tnttpims.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixsdxjjy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qcoaukls.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3sqfbnbxx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruvwbiot.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hemvjnkl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vtqqnsjl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mqgirfsr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xixydopa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3crtamgyf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3iemkrppl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nmydooka.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rrdfycmh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3poliqdem.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eauzjfms.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ijshcyxv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fptmabgo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lkzbtkwz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ktrfjiis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lhooabta.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkbsdhbo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rlyoierx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jadhajee.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dyaplsub.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3fqypxwlp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eyvskode.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jtfgoeou.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3tpjujand.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ioygznwq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yfywgeqf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ekgiizzi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3tmzxxszg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3cfqafboi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jropwezv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3iuleojme.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jbumldiq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fpdmnkdh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qtlmcxit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctlkjpjy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vmcomnhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umlzsrnj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bfvfhzca.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cshnhogu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ycauwxtt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jhqmamki.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vszyyyri.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3raovfvyr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bxyuclll.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3amreiggo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lepojiqu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pdzvmxkn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3mcprshit.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3nvhvtgyy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yrbcctdp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eunebqgx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hottvkjs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kybdtrpg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3rslyfqxn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yhpipxwi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qykqihtf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hhvunvum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qnxemgfh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mhzfgghy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nfnqxxsh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rnivebew.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oafflksl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fkfebfnw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hsfmdxzw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3istmxbur.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgfvqvls.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zdczjdwa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3phnjsbip.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mspbklxn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dsdzvjat.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3csuugmok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xumsjole.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dypvcwkc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3eotkokug.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mgiabien.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cnpyghvt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hextxrvn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3wlakstng.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3stirzujc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3svqijeds.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fuhdgqbv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fogojmqv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3isjdinxb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ivxajfir.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltbvyyvg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wtmzwjlm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ckwvldnz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zphozdnn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hyvsmfov.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fhwynmjn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vtxprhwy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dfrjzqne.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hkeqzpgv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3urevfwtb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tgucbqhb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lwdyflog.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xkziefdk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xbmvdynh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lmhiexdi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3grndaddm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3iphbkqqj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qweeicoo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jkxamxbf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ervfzlzs.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qcnejdnh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urnabtqw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gkjhnxfn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3safnnbdr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3crvadcmg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jbewppvy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ojqkjred.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwtyoahe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kzgigebp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xdtwhnth.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3zwcvkzzv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hewrzptc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mqeyecfa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aspunhmf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3dcekdzec.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nvmnwxnn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uhmsuuug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cpyfnmil.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pzvsuaoa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xnuolfch.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vixaqvgn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3sumhewoa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3igukzpjq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mdubwcof.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mxgeauwu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifkjfrhu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cvduhnex.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3amvgvrly.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lyuhmkja.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3gbydrwrf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gythinyj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3txfvulqd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yfjnwvtc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lobkjgwd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pzyobgth.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ujuobidk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sblbpoff.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wazkbiyk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fmplfngf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3pdqkrgyq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3goiassno.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jnxigvni.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fhdsudgh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cfxcbchx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xpdgikpx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3szoiercs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tbbaosew.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nsdfzfnu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylxzhsdk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ahhrfyhc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3krecfxjr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tzwlaxmz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbijwhup.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfokxxjm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dwhlfdmp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rkygwisu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ywruejcl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jlbwkdoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mpmtabsh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uvlfqoyd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gitlmgar.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wlfqnnek.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xsluwamb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hgfglrkz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3acuwnkhg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kmtcmjub.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xyyxvqbo.html


<!-- 参考信息 -->