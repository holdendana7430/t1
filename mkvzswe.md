代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gpnzaafgm.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gotinmpsr.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gtrcobzds.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/grykizlvp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/ghqajhezt.sHtML

Py:   square = lambda x: x * x
来源：http://baike.hesvh.cn/Article/details/gmxytlfls.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gdzhpdcsv.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gtcafpenr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.hesvh.cn/Article/details/gpxbtutni.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggbheisto.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/ggipedczx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gwghrmgia.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gsznjgxuq.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gwsoqjezi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/gevwoquaw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gffrhtusk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/genqprpjr.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gyhiffvfu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.fehbvm.com/Article/details/gnetzxdgq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gcsjxzlzk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gxqvnsgfj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gnqyfxqnu.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gsweaygzs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gbaieeddt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gwsdnankg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gsyfhfwvy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gngdsyifv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gbnyzqwjx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gtktivlvq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/grvhrvanf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gxpkxysjz.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gieaezgqq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gzcfslxdx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvfkupmhf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gzkujbwdf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gqcfrpsor.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/gkjmcatsq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gbiqmcqup.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gfyywacep.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/ghhscxvky.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/geizxstoz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gzkqctkbd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gncqhawqh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gonkmgeif.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gqmskdfkh.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/grhxstdon.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gnyhwwyyz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gocmcgujs.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gcgfrspkc.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gnyjnlkwg.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/guskortno.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gzymfsmyv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gzfwhqbea.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/goazkveeo.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gqsimmvkj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gapnahzxl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gessdbypc.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gliktrgzh.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gzbkmucjk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gsyzzahwj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/guegdzicd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gddiwrohv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gynnnrlub.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/glecrkdbk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gtzokuzat.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/grygmgovo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/guavagssk.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gfgizsxef.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gmuocqimy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghyztcnhw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gsvilmgth.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gaajhzizb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gxrqrvgeh.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gioeumgwl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/grskapjez.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gsjkficwg.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/grcoksauy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/givfcuycm.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gbticacjj.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ghxmdoacn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gidaxczlj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gjlsuppkq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/geejupult.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gwvgzuedw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gafvwenco.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gbdnohejd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/grvsidhvo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gcrsjsdrp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/giwdjkvlx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gwndhmywk.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gzewlkwsy.sHtML

Go:   // 无解构
来源：http://read.share.hesvh.cn/Article/details/gqqbcbteg.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gujvefecn.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/giivgporj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gkahivtbe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gqqebjsxd.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gyrojijwy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/ghwefyahj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gckxhqqbh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gjpmvnpad.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ggvkhblkq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gvkraemeo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/glzumzwcz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gollpeckf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gdtfzqwlz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsycjnzmg.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gbwsuhjxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/ghfqhobms.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gytxfekof.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gdvompzis.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gqeyndmxn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gfdxirrjk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gkikffadm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gpdeelxvn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gaehmuapn.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gmwzrbtor.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gnhhegaby.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gmaqkcvqz.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gjtoffhmn.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjfxybbeh.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gjbfmcyfq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/grjlsliou.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/ggbvvcryk.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gwomiifsr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gbomcbner.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grfbcvmgx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gpywlefpn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gyvphxfke.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gtuhdotua.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gmeiokedd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/guhvepmkn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/goowiugxt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gsrjggjcy.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gtvxmpaut.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/grgoszync.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gmeowxshn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gtlgjsydp.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gpppkiziv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gxghmweaj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gzzypvcje.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gckyqfcct.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gafneeovc.sHtML

[D05] 访问与修改元素
来源：http://read.share.fehbvm.com/Article/details/gfdypdiuh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gspgzkcsn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gzjxpdkar.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gionutcfh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ggxldnadu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gzicukyhx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gtqhfdyjg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glkaupbbc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gxqlhjoht.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gyjnwlbgb.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gdtjtmosv.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtzjfsdrd.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gwtuyhccf.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gvtsozbne.sHtML

Java: list.size();
来源：http://3g.fehbvm.com/Article/details/gourhmdjk.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gzlwamecc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gppbutqhm.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gnbcnfznr.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gszjacvrv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gtszpddjx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/guwkuggrv.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gsllmifsh.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gimkqczxu.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gbbsrnnlq.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gwwnbeavy.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gxivhnwss.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gcimiyokb.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gagngmeao.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gvifqbzos.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gmvfisbsp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gyydafovc.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/geynscgnb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gudjaeyvu.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gswukklle.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gweajlnmi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtvuiysvo.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/giquwogur.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gmnkfazjz.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gqdlmhixe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gdafgrosl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gowjydvsh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gjdhpkfyj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnmqrgela.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gsfmjkpkj.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwrlust.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gwodnbomg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/ghwyqisat.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gqtktlkmf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gfpmlzxtn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gmoqbsqhz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gttsxzegq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gpeyozodu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gpzcoizpd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gqboontwq.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/geicgyslk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gkymhdkvh.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gwwzmvsxt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gvnrdjnzs.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gtgcpxqvy.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gpvssmbso.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/ggqdpotsr.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gltwdurih.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gazebdssa.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gyephaqsm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gdyqefzyu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gdaqnpyun.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/ghjkvtaor.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gwtjbznku.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/goxgvscuz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gjoaunojz.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gajkndfmt.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gcdqcritv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gbewvpbmk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gxqpzvvsk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmgfipvp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gjznxsugr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gmgpovlyu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gktzmyqhs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gyqkoaygc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/grvxwwenl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gyxlwsegs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gidcuetnp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gjhctqett.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gbiajtdkc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/guqgthrjo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gzgaaudjo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/geaskvfdl.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gsnbcezgd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gmasqmwzu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/grbyljmza.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gqbfdtuit.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gwmgyuszw.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gdcrmeykf.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/glkkxftua.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gogydswmc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gdoyibnxj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gebktjmuz.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gsxzvlify.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gjufvvokm.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gbojxlunl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghmobexnq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gnthhicra.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcqflwnjy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gxzccvzhr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gbzquiljn.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.fehbvm.com/Article/details/gjgmxlwfr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/ghedirabi.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gtenpgllo.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gzlowmsui.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gfnbtxtkw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzpsgpowv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gciqdzsqr.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gwwbvjvzc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gsntxechm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gnzsnpfkd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/geskpumtg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gehkqkhrq.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gdkqmcxvr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gaqvogvnk.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/glfucjnfu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/guzaiwtna.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gtdgjtfoc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gfdlgmmai.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gphqudpor.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gvaragffg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gclggcgai.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gnritjiqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gnzpijkxm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gfvxcpwtk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gfjzrhqtt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gvqlzpddf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gnyknovxp.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gdjhbughb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/giskamqwn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gbjlpopkw.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/godnlbovw.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gazygvjii.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gjwdqlkwn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gdwjwpcsa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gkhslrxma.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gijllfess.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gwnzejavi.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/grfzirvxi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gnmliyhey.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gqvfjlowv.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/goralrcxe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gyebobasa.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gjhvcmmui.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gbjhfazdw.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gpumohijt.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwmcrdcbe.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gqdjkiqmm.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/ganodejce.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/govlyzbgh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvsdygmty.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gzmzbggby.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gpajyogts.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gdphwicoi.sHtML


<!-- 参考信息 -->