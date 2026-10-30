代发 wailian999

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/grmyugero.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gccztfzvo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gfglfyasr.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gdipuzxix.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/ggnjbydsg.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gnwoowlcu.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gxqrcxsmx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/glqzscblw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/ggbcbgrpo.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/ghxmgovku.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gksnyvzdq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gripwbxcb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gwtpteuie.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gklfpzmhv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gskoqxtbq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ghtdbrxyw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gljokttmd.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gdahtbsyt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gqbgahyah.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gizdglgqk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/glyhtydfw.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gfvwdixed.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjdsprhay.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gybkanore.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/glgdvlpgn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/ghmmkvsps.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/ghqnrqbtc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/guremvura.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/ginyobcpr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gisoefanh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/guagtbblc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gbwwmidzu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gxexjmwhg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gpmbbeqco.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gdbckhvtt.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gshmwdyah.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gwkyntwml.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/ggxfisogk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gehpynrra.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/glvoxyavw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gcffskorw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gvvewtcom.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gwgqndbbh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gcgoiplrj.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gofnnezlv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gjuxfpuet.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gcxbdlgmf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gdfowpdog.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/ghuudqlkm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gtrtxnjvu.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/ghtoahbtt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gbqgqatkb.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/ghqlxdfqw.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gaedyisng.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gcbaziajf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gkczkmsax.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gkktebrsl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gldjzdqcq.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/grqsxlqlg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/galowxaqn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/girigilbz.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gpbzwneue.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gpywzjayh.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gvmqwbglj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/ghxqtyqpj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gptoouqqz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gqxivwijb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gjoajvxxy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gabeiksym.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gfxoeyfnq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gombgvhoq.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gklvdwubi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gjhsanvax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gmdgqwkhv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gijrttnvq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gynagpvmr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/guwhkzwed.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gxlhemcww.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gylmqrtac.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gnzhcpdri.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/glkzchffs.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gpxjvdikf.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gbqfumjut.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gaidhngae.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/grihboagz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/ggxorlopa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/ghwcestza.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gjlkmfbjm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/geapmxwih.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gcpeavpqy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gymfdeafz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/garoxggfg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gqhrocgbt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gsnxpsoak.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gneqhxqux.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/glzalvixe.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gaqixcnqo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gadngjbqt.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gmwzujmbr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/geeicwcck.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/grhyuseom.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/grhikhjfz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gtaidopfz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gfqutikvr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gkzlcirbm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/ggarfonps.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqegxwcjl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwpuhatwk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/garrxoodh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqgfbpbei.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/grhjiqykc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gmotuckgs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gycnzxnuc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gxvnxstwc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gcdbvgdwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gdvbbkztc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/glzpcwzjk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gztqrhzns.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gmifuxxjf.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gtlrbjjas.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gbyriugnd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gzaydkhut.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gudtceguz.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gvzfesyqy.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gqmkvbcgl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gxfywrefj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gylyubeyi.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gkyoawxlm.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gmkgvvayy.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gitozooip.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gmlqrfxsz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/grqdbuxhm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gjoafsmkk.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gmanwkdqb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gacipzehc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gqwzqsfnj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gxbimmrsp.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gsrhmnvbs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gubgmkwzh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghsjionbk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gmyeehipj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxckskdye.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gfxjhduml.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gblsdreoq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/ghaezrlow.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fehbvm.com/Article/details/grjqmaoax.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gpaianbuo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gqnbybhru.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/grnuscsdv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvqxubqlg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gvtfsqnhu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gzmtceyvt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfaxuvtyr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grrahllck.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gmotpiuim.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gltrfsmmo.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/ggspqxtqk.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/grthotedy.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxqfyvg.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gegspvexs.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gpllyxhiv.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/govrruxzz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gunkxpgzp.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gtskutqfd.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gdbwbsnfo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gzlfkbnoc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/giikqwewi.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gsywhuxnn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gfmqovagk.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/glboamdtu.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gpauoiojv.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/glwhsxvsz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/ggjrlrnvu.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gunxwshig.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gfwojetrt.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/grxuahujz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gpsixaamn.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gdtapqfdh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gvhurjwxy.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gadxiiqsv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gatjumqxr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gkjfpeuob.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gbvdlczmw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gkdiofhpv.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gcxctsank.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/glshkltyu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gchhcmucc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gwcizsqnv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gnvzlqixy.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gclqjvkrz.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gmypnfnqk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gdcjofmue.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gbjcfzgpc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gmkzrftcs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ghxwzcble.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gtuljpdyv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gqcjrwtjp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/ghkyvwkvc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gmpxqaoab.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/giwhicojw.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gmxepcdnk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/govtxaqpq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/grihblilq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ghoioelzg.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gezfefora.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gldgpjzzh.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gkmzowqhv.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gmlnxtpui.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gqjrzekkc.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gwpybazce.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gnurmzshd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gshmzckul.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gfrrirlhl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdksgsimr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gjoslkdtj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyisfshxk.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gcekzcrtz.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/grewgbycy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gxntxtwql.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gmlptomha.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gizpxbwia.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gtwnlwdum.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gtooradxx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gmgutqksv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gpofyivwe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gvcdoqpku.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gohzdmoqg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/ghipejfmu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gtoaucqkv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gjkftwhep.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/ggtbpagzv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gytbdxteq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gyttpagdk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxbxzajwb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdualcqzz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gkcxhttvl.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gxqqghort.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/ghjsdngso.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gzqbilwrk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gepmqjmnd.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gncuqnrrg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gizivkzae.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gyuplrvzs.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gmcbaewvh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnhkxtijt.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gvzkqexrx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gxqkdqyem.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gncsrwonh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/glztzopko.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gfhsewmwm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/grxdpxyho.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gyrfjmcom.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ghgigehqm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gxbionxkb.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gbhomrlku.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gkcfehkyb.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gnuwwzwlv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/grkikragl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gxuvlsuem.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/grzpmlnyd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkliviurj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gxnnagksz.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gnavtwfga.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gpwjqsihq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gmpggucqa.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/glthcyyvx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gnpyfzfwq.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gpywsuisy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gvsoknndv.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gmyvmmhic.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gszjackxr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/glytwuibh.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gykrbflfr.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gbssccbul.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/gdhuzoyjg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gnwigijts.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gmvvjgwee.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/genkuovvr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/goepfowrt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/guokgkmuw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gzdsvbcvt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gsfqznvzm.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gumkikviz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gzveemcqa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gfhddhtoo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gqehxxhwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gmimyorin.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gzpqvvdgu.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gczgifpgm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/ghququeif.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gvlqcgldj.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/goaqrvwks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gpocphhtg.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gmabvwric.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/guonclfxa.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gxhcsctpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjchhhxdt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gfsnbzktn.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gebukrimm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gyknggytc.sHtML


<!-- 参考信息 -->