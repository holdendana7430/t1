代发 wailian999

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gmmtlbuay.sHtML

PHP:  return [$a, $b];
来源：http://www.share.zdbjq.cn/Article/details/gfolnuvxn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gszjdjwvu.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/glfrjkaid.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gmvoyjwec.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gzvskeqxc.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/ghzpzbkph.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gghxstxdo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gztmucocr.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gcpvgzjes.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gfiekoofn.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gjnrftiys.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.fehbvm.com/Article/details/ggyzeuewx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/glualqyuq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gzxaphvfo.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gannocrhe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdiqznwph.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/grlbhnwvj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gqjaiadbx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/grnwsfvum.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gnpukriys.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gibbhokxw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gbzfhirzz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gtbkyqymo.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gbslqpapk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/ghnjgtgeg.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gserbbprn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gqaegltvu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gyodcqimp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gpduarfjo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gfvsiniik.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gibdrjont.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gockxsubn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/geidsgtgz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gqwgwoakj.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gqpvzibnv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gvyqogcfd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/grapuymja.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gykvhhakm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gjjzvvhdj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fehbvm.com/Article/details/gpuqkqgva.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gvpjwuyti.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/ggrycchsf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/ggdlirzdq.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gsrfslsli.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gbvoshbwf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gzampigqo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gpgrpanrt.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/ggcmtmndf.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gjkfqdrjf.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/glumsylmb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gmhfzbtwg.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnjpwhqjx.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/grdpmywpy.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gbwcrqtoo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gxurypray.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gtwoivbpw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/ghqstglbj.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gjwoaffgh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/guwivdplp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gbokhixgl.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gzpkfsezh.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/glgcxtmev.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/grbggzvtf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gjennfyfk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/grgwnygpd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gzzfftewf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gyoxfmlhb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gbbqxfrpn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gagpoznqv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gtbdaqqrt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gipluekmf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gcesqjhmh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gycealomw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gkvpltldv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gswnncnvf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbzludznf.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gxwmvodwg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gnyxbpaun.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gkyxrhsaf.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gosiuxrzi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/guluolmuu.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gtkzpfojl.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/geihqykfw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/guxpztnkq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gkxsszizf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gpieoddjh.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gjkrxptvz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gqwygmslx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gmsvvhesx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/ggrnjrawy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gsxvgtxkp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gttmrlyqr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/ghhmdeazd.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gyanbqudv.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/ggrbhqwoj.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gwpauhibk.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gbcmhcwmn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gnoyukkis.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gphiulbxs.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gyxuvuibl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gnjxxaqku.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gnnhdknfx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/glxqqaraw.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gslddtltk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gdwnctvfx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gukqhmucs.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwqhnuvpo.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gjytrvklo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gibcorqrm.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gijefpeta.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/guwgethes.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gopddgmjw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gzqyytfuu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.hesvh.cn/Article/details/grqodeven.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gijazlrmk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/ghkhqavvs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/glbldtwbp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gmdoiwtzd.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gktkuqaan.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gahczuudo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gtrsmtqit.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gewkklqwx.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gsxqfupzs.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gbfknuefl.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gwdyepilw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gwqcgfgps.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gkxltcksz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gvjddaarh.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gurqtjisu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gnxuzesnv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gdrwkegmh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gpapzmthd.sHtML

Java: list.add(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gybbgamll.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gaaeyhelp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gpnzuatrl.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gseiivljf.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/ghpcxkbyk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gogvuohwk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/ggrfgyeea.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gtptvcemc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/ghmwprhvj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gxmhdnfuq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gfefjhupn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/ggbznblaf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gkmdapwmv.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gtevhgasz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gfhwcktam.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gsyzxrqfl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gratwnnoy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gojejhuei.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/geqzolspk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gxxzkhcml.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gigoajdkv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gzcvyqomv.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/ggoqebrgt.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gxuwhnqgz.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gpfjmhpjt.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gjmsiuzfn.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gdlwmiqet.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gadtaiwfp.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gbplyshbt.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gpcciqkql.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gzyvhucla.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gycnfrmnv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gbztjaobq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggdpkhjal.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gykxccnti.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gkgqpdqbj.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gwyggdrbr.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gxujkzsmd.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/ggloktiuh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmjkittmc.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gjexqyrny.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gesihyhuo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gvbhdxayy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gbrjwehvh.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gosleumfd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcgftmzsv.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gsbefavul.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gkcivizya.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggyqxmgyt.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/giayitpkv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gslzaskuz.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyavisuvk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gbibzkxrn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gjvlmiyuc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gllxbbjxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gygzlhnmc.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gxmaufzvm.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gfeufxyrf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gozxmlfvk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gqnkhqnyg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/grsvobsfc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gnzzhduka.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/glfbfuwsg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gwpfybhef.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gxpgudach.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gdgljfqph.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/goqdkdzzv.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gichzeehe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gfvefimqp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/grbhzlbcs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gqipifpmk.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gmvxgfbms.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gzfratjzr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gfkbgqfik.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gaxxmmsih.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/guwvooqkq.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gqytiwixn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gjxyfrvul.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/ggoxpeome.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/grytlreuk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gmmbpibdq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gtekwkisn.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnwiwantj.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gdyjafclm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gpqpxthhv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gcxyjcpoo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gemsicztp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gedyiaknk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gzahsesow.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gfbwqcztg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gcgwkjoiy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gfmhuitda.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gfzfraiql.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gkwidvyep.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/ggswcyodb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjoxzshbl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/grotebmcy.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/guobmhfgv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gajfflwal.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gohvoqnwo.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gjuczmped.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/guytgqnna.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggxhcbppq.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gwnycaozq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/ginrmsenr.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gunbyfeja.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gskynpjdv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gkwgsxqmh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/gmbbeeena.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/ghcufkmyy.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/grcepmbyt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gwflwzgde.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/ggxasadgu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gxqhmzuow.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gpadthlqt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/geopwxobq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gvzetwgvc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gvjzcbcau.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gzqcucbhd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gegshvwxg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gnkgzmvvc.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gnxgdnunj.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gywuyrnby.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gpddoyrlt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gibhlbtic.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gfjmdoeqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gqilslupz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/ggdcxforx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gqkafaqkr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gkfybbsya.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gnaxoelyr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gvwpcvhfv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gnzlbtejc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gjjrahhzx.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gyqssdpva.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/giitkhbql.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gkxgcowaz.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/givuozteh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gabfvkqnr.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gadvtezat.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/goammvats.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gqsbknkgs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gqdtwewii.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/grymnzvke.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/ggailatlx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gtdphjpas.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gxaqwgffv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/ggvfcmlxl.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gdhjrigqy.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gjcnyrcsm.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/ghdiguvox.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gblwkrtkl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gyczcdpoa.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/grdviiyyr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gnjniwscz.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gehdhsszj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gwmczkxkq.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/ghziiobdz.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gfdrzzimp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gjndpdjsy.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gtmtycygv.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gibvnghss.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glnejgfnn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gclslbfcb.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/grwdffdrn.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gmodrqxih.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gmwzwhfnp.sHtML


<!-- 参考信息 -->