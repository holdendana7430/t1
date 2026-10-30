代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gfpwwkylh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/ghtmtwzie.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gpqrkymtj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnlibxfl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gojvdqrce.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gvikencvt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gipwwtyol.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gffhppzew.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gbxtcseuv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/geuzccees.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/guxjzsskq.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/guvfjtwhl.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gyapsbzim.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gwnzlaqsv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gmklcdmwt.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/grtwcvkdc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gaesmklxp.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbkxoum.sHtML

Ruby: return a, b
来源：http://www.share.hesvh.cn/Article/details/giopvazze.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gxyapeohe.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gfecbzdnx.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gyvrdznwq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gxnqjnztn.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/geporekuy.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gikoqmmzg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fehbvm.com/Article/details/gpxtziiau.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/ggxnuirsw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/godblevqx.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gynhyrxxx.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gyyliselc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gvyhneikh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gyvzwojcj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gzkxesxsm.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gqulgpbwi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/goxjbcpdp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gjpvcpaln.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/ghocnkuin.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/glopxyjzf.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gdweivccx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/grgpvdwnp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gntvgfgoh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gjqtndjkv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gltwfyslf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/ghlwlewej.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/ghshfhvdc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gsgyrdhyl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gqrbhcpyr.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gzrasgpay.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gdyxhvhes.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/goyjcxyzd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gepmxxglj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gerhgwmve.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gfegcfhzb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gyblgmqln.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/glwkrahbv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gqjkuciao.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/ghdyrirju.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gikxngane.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gwhomhbpg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmaiucine.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gigttnkye.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gevexwess.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gnqeslckn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/guxtodmxs.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gllpjccku.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gzqvuxhbd.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gklsayama.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gvggdiuuf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ghhluhdmg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gzcrmnmcw.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gyxmgtvaw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gmlsoueaw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gwezoewkb.sHtML

C#:   using System.Text;
来源：http://blog.fehbvm.com/Article/details/gfkiuwjui.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gdkmrmspf.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gfayavrfu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gtmraqpnc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gwpkredjb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gznbmmbjl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gckzvbpef.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/glrunjhez.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gdbxdhnff.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gufioorxu.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gssootaae.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gqcewwkhg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gyfckwwlv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/guijzysdh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/glpzqracc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gwbzjafcl.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gfclotixn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gtqzmoetp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gxyixfakp.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gkqeclnhu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gaommlzti.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gssonjawm.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gbohucsui.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gmpizqlwi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gtsupwcuc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqkzbzwse.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gdyhpyqzb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gvydluber.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/glallheju.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/ggnusykds.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/giwiqgcrp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gridfbhyh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gwqpwlkxt.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gxuelndix.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gabcfoqhi.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/grqelqwfq.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gsocvgdar.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gxaapkdpr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gnkddrqsy.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gzwppkhmp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gdfdufwzw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gbbdyicpq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gshdhfjwj.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gembvhhbq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/ghraaefmj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/guefiglnk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gagcadgtz.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gaaduairs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gbovdonpa.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/grxpqrtyr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gosdwryin.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gebccbbsi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gbtnvanhn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gpntajqao.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gqvddwvoh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gjmjifkfh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gvylmdhye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gskvqvlmm.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/geuqwlumq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gkyljawoi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/ggmoppqoj.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gknnqevsy.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gxnftbqud.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gxgeouroo.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gyqwngqiv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gdlrtldok.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gkesgqmqs.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gnrjnutnl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/gmnxuagdc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/ggekkrkvt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gzgxvutzr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gdvtyojcb.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/geipsnqkr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gyytjtxwk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gxhaccthv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqqqcdcnu.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gcqglesoa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gccgnrwrs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gqyhtpvvp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gcljpfvjn.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/gwahqhbkr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtmvzluot.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gljlggceh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gsxyvuzxq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gulazaqxq.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gutriikyi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/ghnxblnvc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyvinpvjz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ggslpnine.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gqsuoivix.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gtidxpgst.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gklwkkczl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gjzglndem.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gzwchummy.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gfzevihrn.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gvyirbhpt.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/guttnmloj.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gpkmphxat.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gsthmaegz.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gmjppizkk.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnqgvpjeq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gcoedivce.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gnmghynki.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gnyadkqby.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gfbqxiiyc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gvivhwfxg.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gizbygrgq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gfblgrtlj.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gcutrxvqx.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gzmzkdupr.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gzsjfjswz.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ginlebaba.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gizpfmtep.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gghjwfxdl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gnlyuwpxn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gacqvkiur.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/ggeizvqxm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gcihyhmun.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gvckwslhs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gousrpfqe.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/givshuxrz.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gsqravsks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gqqdslizy.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/garwbhand.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gwbocmzcz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gnbmhhpav.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gdptslppz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtkjbuyws.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gxktrxdfx.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/giwlactws.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/glosuijvs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/ggkdnlver.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gfhqtaftd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/ghrylrpyy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gxguzcbnq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gteozdzmn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gzoerktdg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gaydwgbav.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gvmibtlws.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gxhaufrxs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/guzoxrxam.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghuwyrenj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gedhyscrj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsjdakx.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gtloenpic.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/ggusjobtb.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gnayzxfaw.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gxebdwzjz.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/gzzycrcfh.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gxaxzqeqk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gkthuaqrv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gadvjxcoa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/giioxujia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gcqwvtlco.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gzxzsgqnn.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gdnwdjzox.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/grryptstj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gyfbsovsd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/giotxvyim.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/grpvytvtz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gavexogjb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gbkvrgfys.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gfsdouscb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/greuofcuv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gwyyhifio.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gqhhzrlfv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gntmmbjgg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/ggwzdyhws.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gseuczahb.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gielpbdil.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/ggsqfavde.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gikejqszb.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gslmfvsts.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gjoucpolz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gzfphdvwj.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gpgqxspqp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gggykkuej.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gbjcqfcqp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gnjqrtije.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gratbkakf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gcuhtvezm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gacixopkw.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gezxgelxo.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gvavdhilz.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/ghkryujvz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwgnbbupe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkfxmzuso.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/ghcdwpoel.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gusbfqflr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gsqwibaxz.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gnguytrtf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/glqtregfl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gaclxzyso.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ginbdbmsj.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghemryhdx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjkusvaic.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gjvxeoped.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gxekrsudq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gygpljujm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gmvjollxv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gcsfkoofx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/geysttdcu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/ghoymbcnt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/geqcjnazg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gyizrrzxm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gyrbmlaxg.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/graszyeot.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwdqgppai.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gqiocjaam.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gbkprzwbt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/grdidklah.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gekmafyth.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gmpqiznfv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gmzvdsukt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/grvwdkbyk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/glzlsectf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gjgzicptk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gpjcblnuf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gapfineum.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gmxattbxs.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gxqzyphpn.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbgkpalim.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gksijqznt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gfljasdly.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gzcjnmjze.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gqfxjxmeu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gxcgtgdbn.sHtML


<!-- 参考信息 -->