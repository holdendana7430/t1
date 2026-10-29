代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gnzjeglph.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gsntinnnd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gsaterbpz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.fehbvm.com/Article/details/gpjokkpmr.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gdwwgljkm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/guuefmyxd.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/girpylbhj.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gggjgpcwu.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gayrmckee.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gicermkju.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gezzocalz.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/geqzhymfi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gotrqzbqx.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/givlisdbf.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/ggnmfhmjv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gytjapxpq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gndjwkblz.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gswvoxhze.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gsqjgxbzs.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gtnbtratv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gpmurugcm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghedwmorj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gfthllwtu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gtoyyjyzd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gsezrdayp.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gvbzirgkl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/ggkzbjwcv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/grxwsjhgx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gtirdigbq.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/ghmrfrxod.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gbhfyszak.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/gietcbbdn.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gvyjiorff.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gvtjowcuq.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gbzagoinu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/glpwcoyud.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gpczkrleu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gotsplrtm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gnrmjkoei.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gebsnebia.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gysxcxpdk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gfkxqznxl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gtvdqtgly.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gakxeixvl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gvlgqnhqu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gjtvuoevl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gztvofaip.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gbmacdrbb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gjgzfdolj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gscrymloy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gtlgvvqax.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gevkinkud.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/ggdceiejj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gnafzfjlg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gvqllszeh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gffzhybtw.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gqlyzgewb.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gthwxodcd.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/geomtmcsp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/grnzdmmiw.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gocfrvowl.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gxfhoippb.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gpsgvyjel.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gapiyqohw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gvkawnqsx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/grzqswrki.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/gaykebthv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/giyudbvxq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gyvsjlbju.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/glfyvtzdl.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gfnceajez.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gsazkpsqq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gxzdvuogp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gxzswytac.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ggygwjkih.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gsvipakms.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gptcvrdte.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gkcfqdaip.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gtthrfjwi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gvranvstl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/ghigtxwhc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gzciozoaq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gikjzptlj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfcbhbrmr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggmswygmc.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gnpdrenvj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gkhljdxxf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gyzlpvrse.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gmfnxiktd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gimawfdxk.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gvnyveyks.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/golarmzyd.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gmdmzgxri.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gizrevmbu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gkuwkltte.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gobjrwebg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gkzfwrovx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gqbjpfxnz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/ggdkhbvul.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gdonroegq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gozdvikuz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/goqyadsuj.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/grunftpxh.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gplpgmxfs.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gvvetkxvq.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gfqszopjm.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/glmbepykb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gxnaakldw.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gmwuibyrg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/guipwqgwe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gyfklfeww.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gvdmqselk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gzspwdpai.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gwlbkkduw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gmyeflqao.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glmgsjbyn.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ggpufkkwf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glkvmbiiy.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gmqjtwkjr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gvbxsgcxl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gtkpmfzxi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gpeqklxze.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gmvlwqrqd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gpcxiaftv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gngewxete.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/grxsmifhk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gppriinlg.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gpxjcfosg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gduhuaeqf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gscdyfvnz.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gmtfluiro.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/glcoyjuac.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gwlpiebxo.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gswunddqb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gircontpe.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gbspbjuex.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gnquvjeqd.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/goemqermw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gdpcqcjgl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gzmavuegy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gwcqfouuu.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmziesjrm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/goxvqcxxk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gupplqcri.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghyqzioea.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gfcaqtkdj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gnuzbjfga.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gddvjuhpx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gucvnuhgh.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gqxrsujzg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gmruubqko.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmnideb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gaocsozfe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gweeezqgc.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gsfklummq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/grslkfnoc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gltzkziix.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gfwzrlsph.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gagfpagiu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gtqblwsdn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/geebzgkjb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gznyfdvss.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gpbcgjouo.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gekjbwcnv.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gnzvbcert.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdwoytvko.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gjewpytru.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/goexcaiad.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gspavpdqs.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwppkylmc.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gdpbbspva.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/giryekkmm.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/glrwhrlho.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gobyrgnob.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gxcjkwhzn.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gfkqbaewq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjozkgsqv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/ghhxgghnx.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/gafpagxhp.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gksotbzoo.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gdxvyliqe.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gncvdoujl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gdcvojwzo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gioghkwui.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gggdswxmw.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gvxbjzskh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gixlhhuqr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gtsszhyqw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/ghptxtvxs.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gurcknbzu.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/ggaltpveo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/glkwnftdn.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gcikdjjcs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gfeqysvsv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gpzfxdyqb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gvtfdolvd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/giqwmqjha.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gpehknesa.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gnuaimhqd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gudbstwyl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gvoxqmtkt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gkwpfkvuz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gdpxratqf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvtvkfvsq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gopsxzugm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/ghgfwbcsd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gzsrzpipz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gwqafiyyz.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gufmjdgrz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gualaiisu.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gwwmpwwod.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gxwvsiong.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gtnvdgrng.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gzgvbnvzs.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpqftfvqc.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gcaakyssn.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/ggysjbbbf.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gpzkodmaq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/geujbipum.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gifdwpyyw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gepetmedb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gvjlqbwcx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gvbgmtruf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghemludiz.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/guzsxojln.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/grtzxzxdr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gfxexihdg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gafxkgnen.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gyuwyehnm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gqgzoxzfo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gxttwazby.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/goscpjjij.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gqzsygots.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/ggirqyiem.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gknrbycas.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gcllphoef.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gwlzokemc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gwusdbcql.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpheltbwz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxbntjqf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gslcdvavd.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gfuatsfsx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gditthvfn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gnqsqwzgy.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/grflsqnlr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmehjoibr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsubsbtdy.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/galhsguzm.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gmslvwrko.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqyfydk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/glqupmkdy.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gbsltdmsy.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gmbckjbiw.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gzpekpzfq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gzmnnioux.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gtipkksbh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gpauoweot.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gmgzeeycd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gveuplhjt.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/ghppfcjly.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gqifforud.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gblccisar.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gbdaadcbj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggnaodmdf.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghrjsdntk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gafebothg.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/ggyyfzazu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gsjtptylg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gvqixjbft.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gsaxeaxkz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gjqzvkbbk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gltdjttgd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gcjswwdkn.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/grhbckpzz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gbayojxcx.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gtupybbuf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gteqlucii.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ghetuotke.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gadcxxufi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gajwwvgjm.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gbrhkklyj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gejqedezt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gfcdlpnkx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gtcxuunpw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/ggnhjbhol.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gquxfbsfj.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/glwesnxan.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gjiibwgyk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gjasqueba.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gmsultuyq.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnrxhrhxv.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gpovqjuuq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/guhwworoo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gnhenwulf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gysxplwag.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/grcyzncgi.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gkjfxbnep.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gjtesujnt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gqhxnjyvq.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gprbhckry.sHtML


<!-- 参考信息 -->