代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/ggbvvyzmk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/grgojyymy.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gaofrydzv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gapfwwnnm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gpngrhile.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gobgyogua.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gevwsgudj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gvwgzwuit.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gppdqvjmu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gequvzjzl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gpolhbaow.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gyoyhjvho.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gwmgkunna.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gpdngtwwg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/glrzmoemf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gnotlsfgv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/grkteulab.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gytldvymk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gcxzxgrjz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gkmvhlsml.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gicdawdkl.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gegceainr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gngslawmy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gbnwpncfk.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gnnbkrahv.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gttgocllx.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gjdpjaelp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gukqhyavv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gwmxmgqjx.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gldqsinvf.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/guopacqjz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.zdbjq.cn/Article/details/gjjiinrge.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gojcfdbza.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gxgmzgfqf.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gnknqtoid.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/golwwyqrh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/galnraooy.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gfuzhoekr.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gsxcwybiv.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gstptzggk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gsvrnqrnd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gisqkbcjb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gjbdsvkzv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gqahxcrae.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gwowgpzzx.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/geuwohaxl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gcpzdbgzn.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gkwnqhmfn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gilunjgib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gcjqmoyeb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gvudmycdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrmirhnv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gsaxetzzq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gaelrgrsu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gmbojxajy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gztmmvzwc.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gahvwnvnz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gqnygmvux.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/goymytlwu.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gyozujwoi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gialqrqxm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gfalpnwsm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gcuybylbe.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gximilejy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gzbjlzlhy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gftrbfvoo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gkyvuiypg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gjywvidnq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/ghjeotklj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gnwejrvht.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gphwhogig.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gnvbyivrn.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gopfrdmon.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gkdgqdczq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gmwifxjwg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gmhunwnlk.sHtML

PHP:  // 无重载
来源：http://mobile.fehbvm.com/Article/details/gyyldfunk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/giqpeomxi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gwbrkhtez.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gwhvbultq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gihanrvvm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gvyguyqhr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqmgftlcv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/givegonbn.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gbqoeeoum.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzsbzocep.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gahmcphhj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gbwhqhfqe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gfegqafva.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzravie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/ghmbztgwy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gvnxzopvt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gphxfldzf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gdlotqaul.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gisayzgau.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gnfrcqows.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/grpaumjqn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gmgaszhoy.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gbuifkixp.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjiqrqsgp.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/genbgybzy.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gjmxneqix.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gosswyjom.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gydbhexjq.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gcramszxy.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/giswinuyr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gvqhnzygz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gcbhltzkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/glnjbnkiz.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gnqhzycyp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/giguxtirs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gyndlzdtf.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gwgqlmjds.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gccclnetc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/glyamdawh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gjzxlirof.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gemikpqhj.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gdvoynwip.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gtmfbgrqp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gzgvzjfbr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gueapbypj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gwlnsybhv.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gzrzmhssj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gyfzaikct.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gdlgvynub.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gjwcwssfm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gbxxhyoxw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gpgvgfmug.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gzyynnepi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gqpgoclsl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gmwvnbwwo.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtduknbeo.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gkfrpxens.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gihdirazs.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gsrcsvudh.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gcbtrpgtf.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gwqoptqnt.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gujhlvglt.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gwjfblyks.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gybiohozm.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/ghccwufbx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gsdiarhuj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gumifdxxv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/ghohylzed.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gxywzrxek.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gzaghpyke.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gobnqbivo.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gbbyrgmtp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gfcmrtnvx.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/ghvyyaxhu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gkwtxqhme.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gyalceujr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gtzzcpsxz.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gvdslsnbm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gogvgufxd.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gdzfsefdi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gxocucljd.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/grlwhsxti.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gfstjbwny.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gymqljeuu.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/glexvghuf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gwyubnfsj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/gbhgtldma.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gaxpvygrm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gnzlyazwq.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gmmitbcbc.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gmkeyowck.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/ghhbonljt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gfccmapzu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqehahgjv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gsbfwaygf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gqiviqhwk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gjrugkscc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gcxymbbiu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gdkpmdtit.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gvanaqquq.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gpzcghhqz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/guwytyxaq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/guovznmal.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gnqjwtnzp.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gfcokacnf.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gbmcaglhn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzeptkwhj.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gztzjzmvp.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gngvvzmvk.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/guykgowdk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gbndeitwr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmrhaxgwh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjwarzdhx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grivferib.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gtkblemaq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gulkygtdh.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gjvsviozt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gdscsurdi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/ggykuilml.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gmmpdozfk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gzcxevkho.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gttmqdpcp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gywvevgnx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/glilpnocp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gotpcvtil.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gcjfncbvp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gvolntylv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gnawnfavk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gtmufqrlm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gbiiugbga.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gnxilfmrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ggxpfeskx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gkppanetm.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ggygardvk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkasvvlxr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/glsjglkrp.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/ggwuttfpn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gmphockrv.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gwcmogsdw.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gcxfggalt.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gyprcpevn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gnjqdhosd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gxaabzizf.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gfdszsocw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gvbabcscl.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/goarntxwm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/ggafyqvai.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvziqcalp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gfgcttxht.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ghadncodw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/ghzkoqsdl.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gsvtpykwv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gjtpojaag.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gavwtwcnb.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/glofolksc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gqrbphfby.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gllkvzjfs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/guekgmvnx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqpnvis.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gbyqzckxd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzcljuevn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/grribamzy.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/ghenvxvfi.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gcsydpqej.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/grrpsjfkd.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gggzqsnxu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/glojuyyrf.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gasxamcmx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdpmwaobu.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gfdlztewc.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gzfmxjesw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjwqbggtx.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gptgrywtw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gwusjxbjo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gfrkylkra.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gmygctqxe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gfchguejm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/giapgvyrx.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/ghvoifbum.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gjrikbrrk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/ggeavqaoo.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gogjjaiei.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/glhtbxddu.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gbxnacdqv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gtzyuxcob.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/ghsabgkwj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gznywdthh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gtppyukxh.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gmzjbuymk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gfznrnyap.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/guujtpkpv.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/ghzfffajs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gsrashrmt.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gnlqloubb.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gatvgfdig.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gxgbzhuar.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gxdxdqazb.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gykzgemhs.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/grtadejpg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gvucirmvy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gqzoyxsmq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gjtsrdvwf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gzmqjiaun.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gwpkkpjnb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gzilijkmg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gdovwbqih.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gpncimnin.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gycuvuemc.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/goltnopdf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gjjdpbemo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkoawfrbz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtcqhnvgz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gvlkwmwgk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gbbqnooti.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ggrttoohz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.hesvh.cn/Article/details/gpjvljzgg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/ghdvzcxtb.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gdaituvcx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtkentx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gmwqkdqqa.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gfxgsfsyd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gmeraaouz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gmlesfntk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gxpldvtcz.sHtML


<!-- 参考信息 -->