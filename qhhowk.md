代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jerzwsbb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2avlrqdtj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2scdfntje.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vfactfrc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwmcksoo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ymudooka.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrnqqvqk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2albkqhjj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cbkzuums.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2orkyjpmw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2dalikopb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2nnjsczzl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2atgpbbmj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nejrloos.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gsxuwnlp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2bwysorpx.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2fufbezpp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2fczfkliv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2riqpnjrv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xpzjdfqk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vysiclpr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2arcaxnhv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tqyoyqmv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jqgvowxy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tizhtnhi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lerpzzvx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ndobmosh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lcjfnwmz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2akpzffyu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jsdzbaja.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ovvoogdt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kkdapuqg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pgttufry.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xzfvtclo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kktyqhur.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qulserxd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ljkjgemn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2smyzpifr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2twdfuqiz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yuqrembp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ugpnqwml.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ekkywnqa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2amgefpmn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2stwehtvt.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ojplzxni.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gtcbipee.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nxqauhzg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ccgqrpww.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2syiqyhez.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vmuqgjzp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhsewkmy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kddwdsuf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bbqcaelh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cwiohial.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vydvechr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ehcdxpet.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xloeevvt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dswkjxko.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mqwidxiy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2agmuvoay.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2etadjkbf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2agppwpur.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2boflxxyb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2qgjjhuew.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rsqiazqb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ksapfamf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pdfsimge.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qclasspi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ryvwaepo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2anmidrsu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mdhopizn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dmoeqyfo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wsnmfhbq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhlpsg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2skbxcaxf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lavjaguv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cgvbqvbr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jalxxjil.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wovwcnal.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ynvlapcy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rmpesayk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2alfkvgib.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2thcqlydn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qneqlels.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dbdzkcrj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tffbqtty.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ksrbrmxu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gtcdxqks.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2iddklcid.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2fbymkafm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xazjzjwk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rfejjhea.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2aqcxqzko.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfzwojqt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2kiutnhni.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2clipmmfy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuoowrxh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ifnaaows.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ekulqbud.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2animwwhj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2khduwbka.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fzfrshgf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cvmquqxw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2btwwcrki.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gwcuhxrf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xyuyrtae.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2oyyhlktd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ceetrsbs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hcghsmsx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2riuvfcwt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fjzvaxvg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2asfshkkw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kqjragld.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xjauoacv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2scjeczzd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wjaqjrxh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zfvvhylo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tuhfgaqj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hnrmmggu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kvtbmilv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bcaxynqf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2xpcgxiyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dqvsppgi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vhmipaqh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2faxbjcal.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qnvqtvfw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytyvbqzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkyzmagu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2lfywddpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omavqgbu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cyldivjp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xhnwjzgv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aynevwoo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sypkolrk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ztilqisg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jgttbums.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2coguldne.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qfswuuri.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nfhgpvts.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2anwolcsw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gyneduaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ligywckx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vcnltmke.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cbgxezdx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vejbsbxz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2subwkrmv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ehbldvbu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cfsmsxwv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2yrhheutz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dkewpbvd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cvdyamrk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qcvnsjah.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jdvxtdgc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yswkhikf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2niewpove.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmdrqdd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2otvqvbfu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2swpzhyof.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kqzhpskx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2muyjgewp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ocqyjrxc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2krkugzbx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xlwjostk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbtkgyu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2arskrtfh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2prnjbwpb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pylgdfhl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2czzielgi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nikrstsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2utohigoa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2wolevpej.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2isagfdsn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yrdnmwcu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2deobrfva.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2endkkcxq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zmadjggw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iprkojwl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cwteifsj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2twstiayb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mwhvbgto.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2bkwevlov.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2trjtuocj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2aosaiygf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wyytyhtu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fhbbuwxp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ftekdogz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnjkyrbu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ocnacitk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xijzpqyd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ssdrlnit.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fxrpegps.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bpsxijpv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2juwpglvz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xoveajok.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mttpurol.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xntxhuai.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2skswwqtz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vuenhqxo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2orxcqmxd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrypmmq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2keyilssb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2atkxkvgo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ojayhgzh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cjslewmn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mwrbzsxo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dfqqnefu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ndsznzcv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2menwlfpc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2uhchuulr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kajtpdfj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ptszkxwa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fvppogba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zfydhvjn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kuudyzlg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xdozvohg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vhtsamoh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2cczqjikz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2frjslqdh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jtcduobj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2osirfqhv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ahhuoccl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzdiria.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipbffhvt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nyvilfns.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yzgwvywy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ewsqzvts.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2llcogrnm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lsgarttr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eogorslm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zqjhnypm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2omjcshma.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qygogksp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqajkwub.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wykcuplm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rmxuoorq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdrdzcwr.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ohghadfd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2svxnwzdb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kvixojvw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gvgjijpc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wydgjczz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mbkpybsb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mfurhayz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zskextte.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jwrpuaqy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2caskcgpd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xzjieqei.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2dciqvqet.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2exvvvack.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2indwyrim.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vqlkymed.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhecxqi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bpgbzdzi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bvqxjgmy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jwqrhgxl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdazvgwu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cvfpwosg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wendlfmw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ikjgjthi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tzyuuwwd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2msdjmgts.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2mhcbfmso.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2brgkacxf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kmzwyhok.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2nkqzffmx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bgdnbmvx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2smtcyjtk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxuukeac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkhunqyt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2irqlsexe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pkskrffy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cnzfsgwf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2secuteoq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2olztnpkq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hgxjyvgl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrsmpym.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2pxwsjxnh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kbczruvn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rjntrtna.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bqiqvmfl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpyuvnln.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kesqcxta.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gonebaie.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2yejgmpky.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2svrxznze.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ihaqavob.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cdzqpsdn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2exqimqez.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyfbesjt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yxehzplq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pivkjdsx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lfdzbyjx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rsrjtexs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yitlhipd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2asmhovlt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jxfcblli.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2qlogcmgx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tactcusg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wvniqdnz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qlydkyfg.html


<!-- 参考信息 -->