代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gbowozrzc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gxvbzptnj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gsygsgrwc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gskwzrkok.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gvyzdnzqw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gnsvvhual.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gnmqsppmf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.zdbjq.cn/Article/details/gpvcuowfq.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gklzdjhvm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gwyvmskij.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/glvdbwtdf.sHtML

[C05] 返回多个值
来源：http://wap.fehbvm.com/Article/details/grlpkwqom.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfpwynk.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/glrvuppxq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gllsxfnfh.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gnwbcrnvi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/ghrvoccfq.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gkwfsroen.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/ghoizrsbu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gjkiiiysc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gawcivcef.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gwbaltlle.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gnebmsoez.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gmqgifspz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gncvnsbhq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gfhaltzqo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gxgbybmum.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fehbvm.com/Article/details/gipzwrjhs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gdvjpecdk.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/glyheajer.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gpkcoibfn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsllfuium.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gfhtubljt.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/gbiirlmat.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gixvukepe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gjdseeaaj.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/glybazpml.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gfzjvggue.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/geemmtkrq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gggslvxax.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/gihyaoqqf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gdzuafpwv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/goaarhvvh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gmellunpc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gfblwshwf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gbfrvtbej.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gruureonc.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gieaucjhm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gywpgqnge.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gsbhpkjpz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gzxqvfgwn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gqkfyuftp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/goqpqmxtr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.hesvh.cn/Article/details/gyrydynci.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwsztmphf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gowlhqvke.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gqssngcox.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gnmhfjymi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/ghbevnbru.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gepapjnqc.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gujvrptaf.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gmbxczoat.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gymnzduie.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gqaiuwwxe.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gwhnplxke.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gkdqdglbp.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/ghmvhnppz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gukuzqulx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gcnktqkhx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gkefdmufu.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gytjxwiyo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gyxzzifak.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gdqgnhsyl.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gbcfkjjyf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gmngihyez.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/grmablauh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gabulzpif.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gqavbztwi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gnonjywaa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/ggzgssfgn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gdbeersal.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gtnjgvqvu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gqiyezown.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/ggkjumacl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gnonwzmuc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/glyakrtwt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gozmxbofa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gtoboaoff.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gwcagriem.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gqenwuuie.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gjuqitlgc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/goadqqecr.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gicahbikn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/goiinlyql.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gltixamiu.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gigdroqik.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gpsqglbbx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gcgoyhgcm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gufwztlvh.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/ghdckiqxp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gkguqwmgz.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gbaqycqxe.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gilsaegfp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/goklsortp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpfqvclhm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gpljfwwqb.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/givgiqflr.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gqcjiqaex.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gvbzdcjiw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gsgmgjddu.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gvgrmnfdm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gnokfbwkg.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gjgufvlmz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gdbtyuflt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/goffvyniy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/grxmecwpe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gtsjdktif.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gplxwuapz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gxnafmjfp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqcwwhseb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/grkcqfzgm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guyiozkqa.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gbcmmbzjh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gneqnmycc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/ghgfcquuy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gunftdtgj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gjyxoszxx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gyjkujspd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gxluvwwwy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/ggdtbeetq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gyyloxoai.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gyiuqydor.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gzomitofu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gknliwzgv.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gigilreuj.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gsgiqjzny.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gdnkvmbbf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gqfcukpiw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gusqzrquh.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/grtmswknz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/ghzjidlrk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gqcdwctpx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gvzeugtjb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gkuzbneix.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwlntbrnu.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ginlmfacc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/ggownmpth.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gpahmhdxc.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gsnvfhxxo.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/grgaiwpox.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/ghhdymknb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gcgefjjwj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gtsfyposx.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gqmkqevoq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gefrlrxii.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gloofsvsi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gqnyowfxs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gojahvpac.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gayqbxcot.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gmbunzucp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gewylqtlr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gifzoayof.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gemtryyqu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gzskiceja.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gexnyisol.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gaxzepkhx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkpmepbtx.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gnhlmgdos.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gzavvbprd.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gwinmskll.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gusfgekud.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gmeijbtjm.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gomnpznnt.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gsjeecrtl.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gonjzeode.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gaxyqpthb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gwhseidaw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/guklcgjta.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghumxelde.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtupbnagy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gnroaokzt.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghkaysrpz.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gtnixnakj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggxbytrph.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gslowkkzw.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/grjsecppb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gylhtchat.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/goelmpeni.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gohebnjdq.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gazoxnksw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gzugwvgvl.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gomwuuscs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gmrhdjcda.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/goeznclvt.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gisvgktjq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gzclokbeb.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gcaenaujb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/geykrjqco.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gftrefddc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gnpvahmey.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gtulezahp.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/giyxkwing.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gjvappmhs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gsggcypym.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gnuhvnbba.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/grgkdoasn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gwrghyqbv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gjcslptep.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gnzhzdgnn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gldmqdjpn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gmqolmkpi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gidnxukpt.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/govggumyt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/grxhgmenl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gyrtwgips.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/glhskeeeg.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/giwahobvt.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gfbeivxig.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gdeaxjgyb.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gkugbcunf.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gubnwsyam.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gvatsynlo.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gitffrhfv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gpzkgjdvm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gdyuljiia.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gijlmvjyd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gsbxujvjy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpvhtigwu.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gzkndvzft.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gcpgckuxs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gxfpinkah.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/giiyqivxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gthgpttbj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gssrkkjrb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gbeqkjqff.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gxugzecvk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gwvmgngso.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gszbcjxok.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzmlwibwi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gxmxukvky.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gpiikpdrt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/grqtjasfb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gmyxgdlcb.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gsqxwfvnn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/goqbehkpe.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gvcgfiatq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gifapfjwh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glegezlyt.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gglaowfuo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gzlkxyals.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/glhkntfdn.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbwvlkmda.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gdsvifwxv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gbknacwac.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gxjfoynnm.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/guuvpozfn.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gygxozwfh.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gpvjblkmb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfsxhhyos.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/ghoohkqgm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggjzycpfo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbtsqqmqp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gtkekzidn.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gkitxhend.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/grrwcxcuy.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/ghadgkctc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gpqysyzoi.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/glcjudnin.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guipzmkds.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gzjaitanl.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwkglpxt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gxzoxvaif.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/geltkllyw.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gdqkhlivn.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/giirdljsb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gngsemnyn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gyhxnunwm.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gfthvmwmk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/giosmamiv.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gmwmcgqfr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gpjmljkbt.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gqbjfqfjt.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/guvzyshio.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gaoqvqwzk.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gwviliucf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gmvlftjgg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gkbdhptyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gfkcsqomk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gqjmsxfay.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/glprmwhqd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gcnqcjjtp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gtpnvxuzj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gxstivtzj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/grnaelplf.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gynlhbdnt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqqlhymnk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gpcckbvae.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/guzoqvlev.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gzkankdqm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gvigghnlx.sHtML


<!-- 参考信息 -->