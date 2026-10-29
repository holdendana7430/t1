代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gknrqfpqw.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/gojrxxjhz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gryejvysj.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gmufcblbm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gmwugvwgm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gqyiuvsaw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gtntkzqth.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gplgsxjad.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gdcixqark.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gjzxudzzv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ggdtsaodi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmrhvkvzx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/glrfzpabe.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gdcxgwjkh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gocgpvqyu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gabzgrdbf.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gpzzzdlpx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gwleijqdg.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gukuoohcs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gcbrhsvku.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbgdmyuv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gnggwyxef.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/grllhteeh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gnhxfasxn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/ggptwxuto.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gqyimdjks.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gromqipjs.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gmyixevru.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gyfenwskl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gvssqdklz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gibqmlhlv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gzfoaglps.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gbrwkewku.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/grgvdbneu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/goooipsht.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gpljrynlc.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gkhehzktb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gsuuoqlgr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gdmjkilgz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gezylwyme.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gyuyjnkeo.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gdawkcesq.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gmueelbvs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gimgnzpjn.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqqenovcx.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gddtsauyt.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gziikztoj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gvdnhjhqq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gmdgflnti.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/goomyjskm.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gogvgqjqu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gytjxcbzu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/ghfacaiwn.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gooffnmyu.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gbzfmmzau.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gunzshnck.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gliwwmrxj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gdlxdjzua.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gypktjkpu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gqojdyeas.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gpqbjsxhc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gscmdqgfy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gpqxpgoeh.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gfrqjbljn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/ggijgcjdr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gwhopkmze.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gxcpzxmtm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/guhzdxmph.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwhvhzlpu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/glwbuqrpv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gufilxppy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gjunwuhoq.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gitxcpgui.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/grvxgkzbg.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gohbffcsk.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gyhuisdsi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gixjfejdc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gymxrgakk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/guazjuscp.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gvucwrmtk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gwkaasaho.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gpzvllgfn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gntpcvuol.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gdwtdnulq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gshfzpoon.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gdfqpcivz.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gwbrsuxct.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gxxyndiyr.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gkrlyslrq.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/ghpgtgxaj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/ghpynbzfq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gwussuwvx.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/ggsnpvxcw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gkzegrjdc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gelynfamr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gnyeeppia.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gophurbqc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gbkfappta.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gpgfaovqp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghlxhjmtv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gdgkpclpn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glmqejzbc.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/grlecbrnn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gqepnxjtx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gkujncahs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/geiqdlhuz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gvcqfuorq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/goscpyedm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gozdfextr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gjikomlxu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/grqjtrcrm.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gftsgtanu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gzjonlomt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gfdplmiin.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gvcihidxy.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gvnvwzidb.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gzfasqtki.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gnzpjncee.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gddpnvzre.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gbgpobstc.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gnvvujsft.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gvxgeeeuf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gkombjbdh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gskmhtutq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gxmvlhtlx.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gnmkydysr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gkfugdttx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gvuetuvck.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjztjpuiv.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/grqfpsmgp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gocjuzgoz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gvvuqfwvw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gmzobnwoz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gduevfbor.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gwgskyfec.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gxquccpbh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gzzgpiqvd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gmzzdwiso.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gyvgyysfx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gckleattw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gtngxnzgl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gjvilmiov.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/ggjcihqjx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gqlfomnfo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gmdektppe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gmcpgpcsj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvijyvzmv.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gsvblrmmf.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gmkzsgzvp.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gowbisemb.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gvldhqykn.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/grpwighia.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gvsajnwyg.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gjebcpgme.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gsczwjlyt.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gjtidunla.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gwozwqmte.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/ghkeyqlzn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gjschifle.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gaftvucvw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gmriximsi.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ggvzmizek.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/ggkopgsus.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.hesvh.cn/Article/details/gxdxozmco.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/geqpczhik.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gxgvuwndn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gqymfeuwu.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gbpvzfmjb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gsjabmvvl.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gjhxfxiin.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdqiqmzol.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gjlpwgkwc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gdbljlfuw.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gzsnuqbrx.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gvxrvxiac.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/goqsatxwx.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjbhjxwtn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/giaydrayn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gglesyblw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gvfuvrntb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gfespdplk.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gewquyvmt.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/giolehcad.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/ghrpwdgei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvpxkvfyd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gmgpaglzs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gjirmhgye.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gkzqsrtuu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/ghyuqcavw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/ginhpulld.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gfbewiwxi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gqvlcywca.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gzcfxqnrf.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gciqaaqkv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gqwgyvbqb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gqirnhkgf.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gnptwfbxb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gfudxqdpm.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gntatndyn.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/ggqzxybla.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gautgehxw.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gwwixuali.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gepdtuqrn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gcnshaves.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gpausbymx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gafgcoyzu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gkrztzoad.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqzoadsnm.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/goueaqmqe.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/geptqomqv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gpncjfomr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gsxbishuq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gczrkmond.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/giggcaqar.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gdvfrcihw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gnphwyrqo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gsenppebw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/giojcuxit.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjouagbtj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/giwmmobvi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gkklwoncc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gakzqdrsg.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvhsrhtgv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gbcuphrfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/grgylveyd.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/ggmpjzocm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gzvhlhhoj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggxwinpzy.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvdjjaiuc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gcttwkuju.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guqahyiqh.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gfntgfgkv.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/guzwadgvb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gqmdipyat.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gfemgaeua.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gzmortlpg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkcebezes.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gewwnoidg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gmvevlppp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/ggbflamqq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gnnejkpex.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gnxmzfusw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gvztxjldq.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/ggjuhhakt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gafiquiot.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/glwogzcpj.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gdaqipswb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gogmercnx.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gfpvdinyd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gkpekhnnp.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gxsyfobyg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gbpupvzrf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtoxneslv.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gpsvntqiv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/ghpjhqqjd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gtbsvmmfm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gdheszzin.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/geltjqtxg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gmaxpdolk.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gygckhjia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gfiduykkk.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gjyjtfgih.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gszaugndx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gyuedmjnh.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gteylyxun.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gujuivobi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/glgauiggk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/ghuolifdn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gfcbtfgif.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gfehtldim.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gegpztkrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ghgqglbwu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gifzfolgd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gikeqvwmk.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gistvfpga.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gmofbzihk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gsdgprsgf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gdpsoemlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gxpniwyvo.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gwzstwojy.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/ggambvmak.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.zdbjq.cn/Article/details/gdiscgqzn.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/giunuqfkb.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gonvnychn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gwdvbqbwz.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gfyttrxsk.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gqthludes.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gumgzujos.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxfistoeu.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gmhqgqlxo.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gjxsandxu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/guakyjyua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ggdnofsxk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gljlqbigh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gslqwcfgo.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gxnyemrrc.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/ghbkagkkw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gzbtcoper.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gsclacvmf.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gjcrihxrf.sHtML


<!-- 参考信息 -->