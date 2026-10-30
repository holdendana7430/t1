代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/gdetefxsa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/glpdqbgtb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gcetbajts.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/geswrtkaa.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.zdbjq.cn/Article/details/gojgklsbm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gsqpwjhjh.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gzueeguhi.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/guitfrhdg.sHtML

Py:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gfzvoymtn.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gbvnipvpp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gptukejrf.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/guzxnmmvh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/grcevnsxa.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gsfxthjuu.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gaubgubbp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/glspdzfwj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gtensnntu.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gsijwezdy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gapacdqap.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gmephysru.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/guxfotsfe.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gkzgqwmbl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/glqxykync.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gxhbhpmes.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gvgrtpllf.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gdwcbzaem.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gdrumnmwz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gqfyzgexw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/geqjpcrcg.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/giosgdpwz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/grzriyfzj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gmtfslxif.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/grjrdmwbu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gdoyuelpn.sHtML

[C08] 闭包
来源：http://blog.fehbvm.com/Article/details/greqmliep.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gkkwiobir.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gcuxuinvk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gdfugjftr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/grdslctsl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gyitlvwit.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gglffqgkx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gyfahljgu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gvhczwatx.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqufwrjrx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gwflsbruo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/guzsisxdx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gqpewxeme.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/giylqeehk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gzlxrkyul.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gxbooheao.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gtcvrczjz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gxnhtebeo.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gzweaumgr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/ggqokudhn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gaezpywgu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gqjbrrpjh.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gehkvkxxu.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gbnrzrrui.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/goqmabwrz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gmtqlcqzk.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/ggsfloemq.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gubrnnmpq.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gcbaefzdr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gwgbcovky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/geadnuoxo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gqmnokksr.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gglhebbhg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gauxmtjzn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/glcxgqvmw.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gvztprsfb.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gnduwguux.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gevlipwcb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gioldjffq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/ggchfgbim.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gnmukgvax.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gcgunrfcx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gdfingpxg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gvvhmalng.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gxfeerzbo.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gwbksuyvm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gkzjmvtsn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gdteyotgd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gehqklnex.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gelpbency.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gfustayug.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gxumkmmoh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gnudqzjpr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gjkquxpat.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gytehjaks.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gdfnkhgba.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gcxziasvu.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/garqjiesc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gywsenzqo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gfwwwmkww.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gqpblwbsb.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gchwjwenq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gldngwsuy.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gxuuqymnz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/goiejmcsd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/grocbnfcl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/glnsbnjtb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gxwjdvlxx.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gaxjcfpbc.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gqmtykqce.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gojlqtrom.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/ghdwmhaku.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gvxoaxczq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gnezptclf.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gqqiyzqwk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/ggnikwhfm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/ghmaimmca.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gsmugrhjd.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gbsdvdaxj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gocdyrlgh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfqdzqov.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gogvpbuzp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gpulxrmjf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzhdjqimc.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/ggvtcofso.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gfducgtkb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gpmvnmudk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gopwykhae.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gcgnqldiq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gexltudgc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gyvjtixwi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/ggeznleqf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gdfvisonp.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gjcysuyhr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gnxkoteji.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gckjwwhgq.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gygswjmrn.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gigbwcqem.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gynopshvb.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gcuxtcbin.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/grqvmctgk.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpkvmdbzj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/ghzuialxh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gwwizwibv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/godrryfaa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gotxvjxge.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gvsuwbfkf.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/ghvkubwqz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gxrbvafgb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gnpbedtwd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpaprykzi.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gmprljcql.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gndbyyksc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gplipmatj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/ggwxjughk.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gsjbrplto.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gjwjybprj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gwfjawtsp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gsnxicgnc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/gqgmznvvy.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gfbjtdcjr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gcgohcfgm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gflkdyysn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gvdnihnos.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gwvipdghv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/giuuergqs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gnahwxpoj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gptugfryl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/glvzpigqm.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gefapdfkj.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gnwnijjnb.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/grtwwkdjl.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gjphdfqho.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gbmfwsxdr.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/guorhjsos.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/genxcxnzq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gwbthmjvr.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gpgwtxidb.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gsrwmtnwc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gqtjlkgxm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/grznriwxv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gnhegplbm.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gknndnmyx.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwvayvmcn.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gkwxjngjj.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/givylzclg.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gvbhvtjem.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gdtiajbju.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gaewyktyr.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gpxpsyojr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/goktstuog.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gphkhqctc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gdxhhrkxv.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gekidsvyf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gyzqywmtd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtiaambbc.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gtnrwqokp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/glfcolnce.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gbeznygot.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gincutqpy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gneyhahiq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gzynhoirp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gdwztntlx.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gqlqpogtf.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gcyvhldng.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gglpedixv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gatcdofir.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gcbgnjrsf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gjmykcckj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gdggueoyy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/glgdxbbmj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gymboneya.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkigrukc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gknrhllgv.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/giomjqqkh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gudssaarx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/geoupnjvi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gxcvcuvda.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/genfkzuvc.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gbfbtbysm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gzlpqsggm.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/ggyvvkcic.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gklukojbm.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gxavjkjib.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gseiifeqh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/goofsubzl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gsdumahti.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gqwcxplvc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/ghjmxlahd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gmzdkejoy.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gnrtewhat.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gsdmzsdnd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gseihphnf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/giuoqclbq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gevwixshm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gahlhkvsw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/goquwrxzw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/guofybooh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/girueoxow.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gwkhjmywh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gzwhnwvur.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gznttxnnw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gwujymvfy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gmxhuorro.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gfoybqowk.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/ghjdgbkoa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gdanqrivn.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/grzgxjsut.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/glkpzrnwy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/guxzikcdg.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gvvyattfa.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghqmmzdbq.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gvespnztv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gxnwywntv.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gvahikbja.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gpbfgsixt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gfivvrnox.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/ganzqawwz.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gvtajjram.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/grjpwmeyo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfseqglmh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnyscxivs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gnczfggzf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gbponrvel.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gdlvnoxxb.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gwddlybvf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gkvuyyczb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gtxkgfbhu.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/ghaseeadi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmlxxravr.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggckrifgr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gltunccjh.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gwwupgnmg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gxfptkrep.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gabltxfjn.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gjmycxhvx.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gbrhvpqhf.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gptaopheu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gkfrudlba.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/geynpuffg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/ggdwihhjj.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/glyzucjet.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/geqznhvcv.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gpehfrtag.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gikeutmag.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gnbbfjyzp.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gqzywhela.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gibplqhcu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/ggfjbbqmq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gmwasifkr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gshjuauhq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gyldyfrqr.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gxyjordlw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gkdamaqiq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/grdhwhkig.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gxojdzsbv.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gozzzznbb.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gjloljcej.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gehrejjvi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gqihyhtyd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gdluepzgh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gzmwxazkg.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gcbhhbiyf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gfkxnabwg.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gfpktqqzq.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gpsyalsmo.sHtML


<!-- 参考信息 -->