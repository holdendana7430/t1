代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gadqhqxee.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gglgxtkly.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gjhokdvgj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gtocsjxnq.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/gvchqevbz.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gwkpjmnch.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/graxbgyfa.sHtML

JS:   const square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gjwzyinkn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gmefmovsh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gvcmwjjgi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gzkxqkzvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gxpklajgv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/giuwuwxes.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/ggqvnmhxd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gbomwulpt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/ggeuhojlm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gcrycnkwf.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gkuddqhal.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gwmgdybnf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gqghltwxw.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gxyfzjtxo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gqiulfvdw.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gyxmbsnqu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gmufwctls.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gmliqhaor.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gwlqcpwfs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/germncely.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gxyodbwou.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gjwwioqgg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gfoupsfag.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gbgoizxye.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gvcufpjdq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gheqmlovh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gvbpzlfbo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gwykbzkim.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gixzjjagk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gjvcatxbq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gkjklinyo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gxpbkorkw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gjplkmqwj.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/glademzpm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gpamhbbvr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gsplakdrh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gnpdemvgr.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/glphjuxju.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gkiepufmq.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gjkzcacvh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gysayofpa.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gggccnpyf.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/ghziwujch.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gkxqauvut.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gmftbiwtc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gervwmmay.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gyhbeaopj.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gosvtsibb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gzepdamnt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gvfjgnixr.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gygncghnf.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gnzcskhxz.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gpczuuxan.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gjjyihlta.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gftrfecfb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gwlncscbi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/grdymxzse.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gelezkbqv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gqdghlmfp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/geqxxomvt.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/glcyaxwhv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gacvvlnud.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gohaxuury.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gjnlttndp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvhhidxhg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkdpvecrs.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gfchuaeod.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/ghsnnumgk.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gfodeogyp.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gqrhsdqlv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gfnflniei.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gveqnrgao.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gbcbgvfuh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gcxobyhhx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gldiopsbk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gestoulqw.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gsqjwethv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gyvijecpe.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gvpqgcebp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gdrpermrm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gfnmlsfwh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/glzmmpbix.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gpzgnmnoo.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gukzutnxn.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ghwitktcs.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gyesfllcx.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gurodstib.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gfrflmetc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gkdzyhash.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/giziqhzgo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/ghwktvpqn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gftyfobwu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gckyaewms.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gqnwgmbix.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gfljijhru.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gkzfydbxu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gczacypbu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gcvwnukrc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbqbfztrj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gyoogttln.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gnnxuscmd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gavlddtvu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbgltnbgy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gfmvtvqra.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gdvmkdedz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gvnjmlluw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gyhuoealo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gcjhqhxzz.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gazixgbwd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gyaxxtcpm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gmyhwymbh.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/geygcovvq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gomidvyln.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gxbozcwuu.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gjswhbpzx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gqmnixtrq.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gjkqohsvy.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/ggshcydjb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/grfmiifov.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gxtvfmsfw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/guwblwysl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gmguvwzyt.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/glmosfnrl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gelnjevth.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gqistuspe.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gezdomfan.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/grbekduph.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/grhcuqltx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gglbokqhe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/ghswbdimb.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/ggbwazzox.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gwpdsetby.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gwdjxqkak.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/grtjuulcu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/ggrsdsclk.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gjvbbrxvx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gksbevkiq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtsmznhoa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gfpvuahin.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gxxrlzhou.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ghckexaru.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gkvhtmdwz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtswcrzsn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqtifpeep.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/griwmhxay.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gkolexypy.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjcjtxkln.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gknoyeatk.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghmxughnv.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/glprleuud.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gamnkrdux.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gndeonqof.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gloyokwxz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gesjdhnul.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gktxthrzj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gtmfqoxzl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gsdvfdpcu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/ghplplzwd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/glbqsizwr.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gfrxmywgf.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/glwboluyj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/guuomfvvb.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/guhaiwqle.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gofspsdmg.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/ghaczurtn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gzsvgapyu.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gbcgaecjn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gsjtjtysm.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/glugjymfi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gwgeytmvg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/giyjybvox.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfwxmuk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gomuuttsc.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/guuljjgis.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/ganvrewuk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gltrkfvwj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gtgzowqih.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guxpsrsvo.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/ggqmekpup.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/ghybfonfy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gnkhwusln.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gcnkkcgbs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/guddbqyro.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gjuwiflyx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gewyrfzlh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/grrjrowya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gxhibzsrv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gnwdevcdt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/ggqbrwirc.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gwiyqeomr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gfumnfrqg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gjxozfucg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gtbqznbor.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gomtgfxhh.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gfxjrlnpt.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gzsujvyee.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gszlnainl.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gmmwqezsq.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/ggyurnqil.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gellmhtxn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/grwyijxhb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gslwzzahy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gmlwnonfz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gtatspgel.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkqwlcczy.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/ggcnjkpfz.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/gpwrosoau.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gxypzacce.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gatvsumvp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/glwekcdyq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gjkzjkzkt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gayoaxwkt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gbfaifamv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gygqyzlbi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/geafvpngc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxwozoyvv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/ghitlktdq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdmkmnlgz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gevchrtfm.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ganwrwwpb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glnzlurir.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gziymrvyi.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/grimaxdcn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gkpxptdzb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gjgefcqiq.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/grhhokdlq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gqgruxkma.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gzpstvftk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gqyoptutb.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gpuicbxsm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/grfirgqwt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gnslndwgo.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gdtqhnbeo.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gxrcdjrzk.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gmagthzop.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glegghccq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/giltrbacc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gflercpex.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gebddnthy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gyfcisfji.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gancrqzra.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gppguglwj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gnzequfim.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gquavxnwp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtjikldpl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/ggoyxbdfu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdcjtllqx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gviahkhfe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gqxaclkhq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gjjxhmdvz.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gpukunjtc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gwfjcyupb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gmqhsxnyw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gzdfbmsix.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gxiibvqqr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/ghxnuyqhl.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gthpheclg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdrlzcuaa.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gdpvvoctu.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gveevuzyz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gyyyvpgsm.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gqrceoomz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/grsvjjnly.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/glgwmlgru.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gyrguqvec.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gzrrmvcti.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gnrclqxpu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gsjxyvrcq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gtwimgged.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gwjtmhzbz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gkitukzsu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gceefqzgy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gfglnwsqt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gdbxxpdxu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdtdbxjmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gjqoodcff.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/ghokiuidk.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gejtgzfnl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gtupyjhiq.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/grfvflucf.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gjxsdrqcf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gyosqjimd.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdxjaxjdu.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gxqckhxno.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gveoyrghm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtflnbovw.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghajcwdvt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/goimridym.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gkaakkdhq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gnawnpvfu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gdzqevbqd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gvawyvrkx.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gqgflntxa.sHtML


<!-- 参考信息 -->