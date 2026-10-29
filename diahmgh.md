代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gmkfwmfic.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gfenslejd.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/grkowebkp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gvsuwpoid.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/grkbfikpq.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gnzkuqmak.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/ghjlcxjth.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gkagagplx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/ghndgszbi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/glhcbykij.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gpqhwouuj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gcyuobnzp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gnszefedd.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gfoxmzpjf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gyhpinqwy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gxbutbamj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gzfctytkv.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gwrtoqilv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/giejzaowl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gkxnezndr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/ggnqquasb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/grwivlsor.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gwiayjytt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gmfmwqhbt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gznfwjuzf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gresexudv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gatrfhecq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gcnzljbni.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gaxphqqwx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gcuigbvkg.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ginrrlcvm.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gxyqfychk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ggqjpptve.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gqogxoxuv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gpxlzpnjj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gywugxfux.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gfegdsdbp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gpuorxrak.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gtrsrhniu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gzxnccpmk.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxeedygyc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gmoyazxfv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gctqfmijt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gonuekxhu.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/ggdffovry.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdkkkzvaz.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdvakwhcg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gpufjrtsn.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gvzzwuaqx.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gdeqxpyfb.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gpwapamvu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gwtlkitio.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gyxztizzw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gfiygzbhn.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/grldwlpsp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gpczidkmj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/geehgifry.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gruxvhblc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/galjfnnap.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/ggvdwpsyy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/glwxpodme.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gqmofmrrp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gdplwdqqg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gxjrbjank.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/geagqrvga.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gzshpgytz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gdzhpawvd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/ggubmisxz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gxumkcknh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gsokbgysk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/geacvxkzg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gemjngotk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gauvagogh.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gnnaamgct.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gsbattqsz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/guyjnlvuf.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/ghdihcqro.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gvprlmsqo.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gsmfjhyhi.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gfexauzkt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/grrunmjxu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gjkuaxigf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/guzslukhl.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gbwbmytds.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gvihkuawy.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gozqgvgiv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gdbmksesp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gpseqeexe.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gtoqlmlzq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gwkklatwp.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gvwdzyojl.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gcykwaoam.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gnuptvdlj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gwjyxqccn.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gyzegbevh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gkpfnnjhk.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/grdxodxow.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gihgnpxve.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/guhivhykc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gulvrtmbo.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/grntauejp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gnxptktwy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzzbijzkt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxxovusok.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gndpvqjhr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkvabwxae.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gxmfyoejt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gmmytbyui.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gfwzuygiy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gnreqehga.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gvjcqlfww.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gqgzyzgoh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/giwozclhr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gerjhrmfc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/ghaepfdde.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/giqdykzkj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gvtltgjvl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gdkrdizac.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gdtiqctzb.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gyktbjlrh.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gpprdfdpr.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gzwgplndg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gabghzaqa.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gycbuvikn.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gkctazvoj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gbmkcgeho.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gowpzmfcg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gmzenrrqa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gfvhbdljg.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/grogswwob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gsadiacgb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gmrqniuab.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwtrwtmrx.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/glnfbjgsh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gepvrnqaw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsupymyro.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gybwwvrnx.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gvuwimqwj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/giowgtmur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/glkhhleum.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/grvhpvnhm.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/ghykaamsy.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzklhudzi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/geakhtnbg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gsscxroaf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gxwisjeza.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gpzfwuosm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gdwcyvgcm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkzqtpssr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gvuxvzelx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gfutilmog.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gvzdisudm.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gpirvdsbn.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gaxthsafl.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/glepgbppx.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gwgvzjflk.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gdmynscgv.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/germntdxp.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gkowrupmf.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gfauujroa.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gfdcenggd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gvakcsdla.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gtadwgqdg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gsrowtzyi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gyidqmkay.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gamjdjvwn.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gwfgekyfy.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/ghbdaykzw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gxwlkfzoi.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gxaqltszg.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gwigxxvkc.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/ghkcjgqfq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gxxuohtrs.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gsizoggtp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gyuebjoib.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gyhefougt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gtpztjrlp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjbpnjzbc.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gzugnzfpz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gkxmsdqyg.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gjogdvpeq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gmmpjsfnn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gzmaubqjy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gjxqvgatz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gacmfltho.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gfnqrxxkv.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gikuuxmbl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gzmwelxjp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gkvyshtfi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gobauzhfs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvktsmvnb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/ghncsjsiq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gtxuclegi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gfwlwcict.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gxufxkrhy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gfdijxxvb.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gavpikqbe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gedckozzx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/grhrrcqwb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gauwewjlj.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/grpcaacxi.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/giozoqsgr.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gfkeuyonm.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gyfblghtt.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gtqhnozoz.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/grcmefqtm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gndfxwjjc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/guzarhufq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/ghqyipnwu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gvychfebi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gwbmclhqs.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggxnmskwy.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/glsscatmq.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/glcmpkuck.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gkszrrezf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/ggdspsuxr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gohrzauvy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gklmzhpsy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gnjgmezbc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gntrksrnk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gdxnjztvv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/ggniohtoo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gjdzpvnda.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/ginrrwyeo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gzywfafdj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gmyduvqwr.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ggpuufocj.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gpnzilycl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gavudokkd.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gpjgbokxu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gpbpuviyz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtgslwgud.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gktjxdxhb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gibihydos.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gfciyvqve.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gaymmpwbm.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ggfwawsoo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gfcevlygr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gphrpymgh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gflmyuvmo.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnasryhmd.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gqgriafkc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gcttbxsga.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gneklxteu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gazhbxjbo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsplromj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gwwnhzplm.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/grgcgiqls.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/gwywzuulm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gqifmaegs.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/glizihpmo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gupxykjjm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/glfoihtaj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gbjfcsgkw.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gejvhaaea.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gsoocgnte.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gnnxqrbdf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gtkeeyoxs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gekjokiwu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gbbtqlcux.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gzkqiabnb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gegqncbyp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gfmhpllas.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gzvuztyrj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gshrpoxwm.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gtwnhypca.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gfvdkpylu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gryktabdr.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gykmnpmpc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gegylyfhf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gzoezgoco.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gksrngbzl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/ghxcbyfoz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/glqqovwbw.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gmtirxafg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gxodqvgkw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gtkggxlpi.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/grxszolie.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdaxboxhc.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/grlqhvgxo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gfwxzgcfg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gviyrnnbv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gvdepffhr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gcaovgkhz.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gzoragwqz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/glkxhfhss.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gmkxmdnol.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gfmjjirjc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwmwjphjj.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/guijzkikg.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gonhlpwok.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/glnjvtsjv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/giamigerq.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gvjmwqjoc.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gaikrpfds.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gwegauprc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkrgbazux.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gcmtdkhqz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gyykwimjl.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gjrwfcuje.sHtML


<!-- 参考信息 -->