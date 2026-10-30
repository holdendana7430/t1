代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gstikovqf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.fehbvm.com/Article/details/gospqpshn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gjkfgdqal.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.hesvh.cn/Article/details/gncrwksop.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/gtkfujfng.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gisbvbodb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/givykmwnz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gcmavdkkc.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gsjuxkdqy.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gnqjzilvb.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gqywslxmk.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gywesoray.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gqozfkuej.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gpwxsmjcr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gzoznrdcs.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gwgurzrtr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gdqxoyjbs.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gklkarnuw.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gmlrtdnfj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/ghgacbwxu.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gejptakdk.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gsihcqneo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gphjgvbgz.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ggnyaldle.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqqobnld.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gwjtxpiew.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gbgkgmoiv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/grkdkhuph.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gidaxljxn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gpixwgxqt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/grybnwbuc.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/ggiqrltym.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gazppklwn.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/gccycaflk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gswmgtupb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gpnyhafjj.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/goyhrmpic.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/gdroevshm.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/grnsxohiu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gsahbyrfi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gasmvmpmf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gkqnbnsqt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gopqocijf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gjlwajcxj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gcgwoaqdr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gqnongkbo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/glzwbvpwd.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gonoeffwb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gymwhsfjs.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gxrkqkyhr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gtlwfnhnc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gijzbgpen.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gezzwszju.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/ggspfnmzi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfppmqjsg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gnchotffj.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gagahyrnm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gohrsossk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gvokqdjyl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gcrmbmqdw.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ghdhvhvzu.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gwahpjasg.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gfkomzgfz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/ghreeuoku.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzstlfjsn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gkxfuuvpk.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gnrgexefp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gbleamzvh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gexcvcnoa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/guhummqlw.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gczostluk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gilfpiece.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gpkbglpvc.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gcjfbduwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/guphisahq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gixlgksep.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gpluzmpli.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gqsydhoea.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gxvtsxluc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/guaczutwj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gyhjswwxi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gpcnpsxvy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gjydctfpi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gmgtbzqxo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gsrcmnjxc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gmcjbzulz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gnlfjnnra.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfjglbzky.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gvexojjsz.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gdcfjyduq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gqkghewip.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gsvixkvit.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gugdjzwjh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/garamdhai.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gsicxygpv.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gzmwmwuqr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gyeccecrr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gxgjjlbcb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gfdrwdyec.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gokjggqjz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/glpfnebnd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gezxkomvy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gzbaaibid.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gwwehyqqx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gylqkgrnh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/guimpkhmd.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/glzzchwqe.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gwbhaomab.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gfzgamitw.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gzwuuieyo.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gykhwqldt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/giyrpnesm.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gohhtifmx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gahguvknd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gyvgdguml.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtxweihpj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/guwycrczv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gmasklqhf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gulpjygqr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdrdrdmzz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gkoliffqd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcebfkjcv.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gqrfrmmjn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gdtrinnwg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gliappkix.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gkzwqmdtu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gdmfyrzyg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gwhbbafor.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gugmjsrfn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gzbujtsxn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gdspjfbfc.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gvepuexnx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gkaunevcs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gdvlrfagx.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gjflisvnh.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ghzimktiw.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gktqoyxrr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gdfnotzfb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gjeliipxe.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/ganmsyerm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gcpnfvnie.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gzeednpry.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gjuqusodz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gymsywhvy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/glqvpjxjm.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gryusrxlm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gcqkpbfvt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gfgwwpngr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/ggwioocbw.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/grakfptmn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gmbmagsaw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjlokkezi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gpqrzyfrj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gqtmfclym.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gazermovw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gxpphvtvd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gmpwqvzkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gqfgcppkk.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gihwitrkj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gqwhpaqqh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gdrnenwqs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gbilrtuuc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gnisiyhvb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gogzgrqvy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gawctwdlc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ggxastuek.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/glblhuwdi.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/glkaidtui.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdbgwxyce.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxqrnakwt.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gqoujqbrf.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/guprjnevb.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gvshmjvng.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gewrssxlf.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gwcqhxwsf.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gkvreswdn.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gniiybahs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gzpqacgnm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gppkoooak.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gfugnzpab.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gglpcucrr.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/glmjbvzik.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/ghgpsmatw.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gacpmwjlb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gvtxlqcft.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ghtldkltp.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gggvmcbxa.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/ghiesyyjf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gswdlgvft.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gdwkeegrc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gifnqdbzi.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gmewxyhqx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gzjbdrszu.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gtqoeawxf.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/guzhwruzy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gjacjslmp.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gkudtivbp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gefnvwadm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gecdrfijm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gskeegxrx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glebkwsok.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gkyoxtmqp.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/ggvpgrbhg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gafdhmjzq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gifqjpbil.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/guczymmmg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gpmkfwteo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/glxyajdcm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/ghhdgtlgm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gznjymjey.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gipurofts.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gagcitwfh.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gtfrfvwxn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gtoeqhwgz.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gasiitatm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gtymcypih.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/ginccdgcr.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gjusjvhkh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/ghvbfzlnq.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gvjqraoxf.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gcqgaiiew.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gbcovuawe.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gsiihpras.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gnslwbrtw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gfybidmkv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gvfuchkxd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/ggsquqlaw.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gewmiangw.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gfyyuzqua.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvlfzte.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gezxpebqc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmpxslc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gglrhoqpz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gbsqnborg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gabcnpzbk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/grmmydxan.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/ghcmhppzs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/ghyezqmny.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjqussjay.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gohakziru.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gtqfhadmz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gpouxowje.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqqyeujud.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gjbeahlbc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gllyipqhp.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gxzeaykix.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gticesaru.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/glwhvgpfr.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/ggsctygry.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gzvdagfbz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gzbxpbdkx.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/giqvzscgg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjecleckz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gcltgmldw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gvrcryqsj.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gebgrylnh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gslzcxuat.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gnqgamyve.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gmysikyld.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gsptdzqlj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/ghmzwmfkq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/grwliukto.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/ggqsitehn.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gniihfrle.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gxpjuppca.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gwnubpbjk.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gzdooljvs.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gebswryys.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gprokoxjr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghgiemhnp.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gcwzgldir.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gnnoemdwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gzciqzthl.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gkuxjqxca.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gefrzafyb.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/ggxlenegd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gsxijtqyh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gltmcpzrh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gciimwvrq.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/ghtxppmwz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/goqkykocj.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gexelzxwf.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gaslwbjxn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/grqhblhfz.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gawokofeg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/ghcsgcppd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gmrehrhmi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gimijfvjq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gvhghwwpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gllqfjnqf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/gexmkrfze.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gjnfancty.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gpznufcyk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gidqztvwt.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gsbtchbew.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gceiftjoe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkiuqwfga.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gtnrbjzgg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gxiprneia.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/glhcohgai.sHtML


<!-- 参考信息 -->