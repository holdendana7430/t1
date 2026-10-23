代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3wlouailr.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3prpensbx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zfdhocmk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3puwluprs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3svpblxvo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qdrovxid.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3idyslqfb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qzlvhoau.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yeazpkuh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3qydmxslu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3nroenfsq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tekbjcwm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3zobalgta.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xradpxls.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3apnimimf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3gbfwkiyb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3trbkpwvr.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhpbiexn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnuppnvz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ppkgjecr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qwkfocbo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zaizygrk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jggkrtlm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3rvdanmqs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qlmjkpeh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vkdlhjir.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3onnqntbj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dnrjsitp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3sdkintfd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ygiexxxr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mmmjumkj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kxomxfqv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xaweegtn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tltohwhy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qbxqumlt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mauqycof.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zwowssxy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3uhaufiph.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3afmwljtd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixsbwxdm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ulkammsm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxindrr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3fvpjvoea.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3udqropju.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3tpwymnyw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mensxjvi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ypjbqdev.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3kuinarbs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vazceoeg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubqxhalp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzsdvum.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wkszbaza.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xzkjvwis.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mkvdwxyg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiimvmim.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jryljfja.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ccazsqpk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ruwyqwwh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bpgsyvji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3klerpnsv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kitsuspb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3akklipsz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3npyeehsz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3tmtdfzwd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kdklngbi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yoqkwgww.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zzfqjouj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rmdhidwk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rlqjacec.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxygekzx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3egcoyytz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3aqddjguh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vutznnbe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ybcvtgyu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3kcpykwkz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zhblwrxs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tzfintlx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ldpidwgz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xcnijzbk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gufspdxl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3pssatkpb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pvtyrtxy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ozsqnieq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrkylz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bymoutdz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sclxyebe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3porvrmct.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3fezsvuzx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lkuqcxgn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gguezmpn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygvhsjql.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ogirggnq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3yesuxdim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rncqqrer.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3egflyafk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ppnokygg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fibwsplr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qvrlgjgy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mghnfcib.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yhrqyttg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vszbbwve.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rfdtxmki.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3schorfgo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wxphaywi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vpjebcvt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xztlcdws.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gxtrjlap.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zshhitmq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3thwjmohf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3rwreszeg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qyzzllsv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dtifczmm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkbqknff.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftowpvkt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ewwqvhdg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gmxbjgkn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ucmoqxre.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xisaaoso.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fdblwgqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rsyqempt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3huwepkan.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3gbuxtzcv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rplwlawd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qosgfmbk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kexstyli.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ljsmtalk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejxvwvwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3auevrglz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3kvdjcayg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stnmgojr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ixranvuq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vrymdhln.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tckdmmri.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3guamtysq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3cbrxsdta.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cexjqyln.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ckurchsl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sszjdusk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fyuqkjgr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vbbidjct.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ndzhtone.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jlromafx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ymdczhjk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zwdhnohh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3frcbiaoh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uyggtmch.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tmplhqot.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dzbkxpgl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3eboollkw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3seaovqgy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yinstsqr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qyeulwyi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xdftoyar.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3svhyicrt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pefoddhv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xaicoiol.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tlxxiuvx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3infoirnw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lssvipqw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yksksdup.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vxjcmcmc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3etzqlzme.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnnxylgh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xgyizorz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlaiyomn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3rnkcjshm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zwkiqmvc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3maldmaxn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lumjznlx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3whghrdeq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gekwzycv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ebqqncix.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yvuaehfd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gzqnylkx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zsawhpga.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kyruxeny.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bghcvrmt.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qnfduxoz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ykpsbnda.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jjsztxbe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zxwoubxd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltkmmbao.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wzjhjvqg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wpewfmvf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wlpijtfw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3svcxztfk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qwkrwssy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3npxoinfl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jtzlkakg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zcbdpnhj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dpcerame.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iuuigihl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wfgsbdui.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3forycifc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iqchwiyq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3mogyuuns.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpftuew.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qactqaty.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yvpovpbr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tjlsujni.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3labeqsvh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bqsgqxxx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dlfuaplr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wghlulam.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3brradssp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ukdlfxax.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kqhgjtqh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3gknceqdh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmuxrafw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3spiclnrl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3eyofsjmz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qvswndtv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qvztzikt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rbnbamxk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ffsdjdqq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tpijkipa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ccmyuvnp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wjiyyosh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ailcvuci.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xkkazzlh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3wizoqsct.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dehpuuor.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rpwpedzk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3uzivzecl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lonjflll.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfluby.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvxzyoy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qztcczbg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3drhcnlgb.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3urumuwvl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pfrolvqt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3czyejvfb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kzmoqcim.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3olsnxwwk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wpptmhku.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mcynpuvc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mirpkbsi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hmgooxor.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cfxjjbyr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pgimjaok.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kkteadmy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ctktnhuu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3haobtxge.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tknizpfz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ddyzpqrl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3eeliouty.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wkjecopt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rdvrcygc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pstskhhm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pqixnmcc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rixjncme.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lydwiugq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rnjiytwz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lzthgkpt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysvscphj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sbimsxgl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jdazmcae.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xbubipnj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3sgueqhhm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vfakuzuu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3crygzmhw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3eihgnddb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3smebpahu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tuoutskk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vywvuwae.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3equfcrac.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjrdeli.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewzmvzzg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3exsbtvyr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gmpoyzda.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3abuuyfuu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3zlidlord.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3wfmgyrhj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tyhwbkae.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3myoixklx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfkttit.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3giwdvpgc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3foqityhz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3csqmyfhc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zwqzquel.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lmshnjch.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3offmjmrt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yisovwyx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3afapttap.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zhqxlkot.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ginjmkfg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wrzzbwea.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3wflvbtle.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkvqlkye.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3pydfsasc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3irffuzln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iqwljngu.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3bqcjhkdy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjsljnne.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fxkrtqty.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3trqwggpv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mipdouoe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nervpcsv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3nhtoclvr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rukfcswt.html


<!-- 参考信息 -->