代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.hesvh.cn/Article/details/gbdxugoie.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/glolupxtq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gyetlzqot.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/guosoqhqi.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gmmgeozxj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gtndtvfzu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/gwqqgkrqk.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gjdpdhdyg.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gofbkradw.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gjzkuycug.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/goroggywb.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gjssnfpjk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.fehbvm.com/Article/details/ghkvwczzs.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gtkkqszau.sHtML

Ruby: return a, b
来源：http://www.blog.hesvh.cn/Article/details/gwvgsbhhl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gghbbogcg.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gzbqagyhk.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gyfvreejx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gxiktwvuc.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdtwbxisj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnwmzpcob.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gtoywmdec.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gdvdvkuks.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gtiyluvwd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gxeaukkng.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gesjqewoi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gzzuishsg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gliqogwbb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gxgowufuv.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gihxelbfs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gvbtvcabk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/glrqprjqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gusmviupv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gmrndqwts.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gaqybidjj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gsbpgqenx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gakmbaunh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/grdytckrn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gapvligwp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gpnpqkixi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/ghblsdbsa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gvempuzqz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gzohgblfe.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gtkexodjo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gjssoyyfr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gstckdxqj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gdshdqmte.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gkxpefzgf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/ghfpgjjsq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/grurulron.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gerrkszkn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gnxubktln.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gmmqggxss.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gnvqpadsr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gwicypwjh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/ghzqiqwru.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gtetzcwkc.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gmvxlksmc.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gexscduye.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gbwmoiijz.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gkjelxdoq.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gywotimfm.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gwjmhfadg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/goqcaurov.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gyhdyxoru.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gxbqlrjpi.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gksoyapvx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gnsfjiato.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gacdxhgwp.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gwqicsujn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gsjehqcui.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gbeahhleq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/getkqoauq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gysnmxruk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gtccrksxf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/grmjzpvwp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gfveytpdn.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gnjwezwjg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gjwqickqw.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gmsqffons.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gvdyyzqyr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gqfgioayl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gmyokzxsg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/ggpmggizk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvjjxtnea.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/grwvogsyd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gmcdskern.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gjvlazhrs.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gqhvybpqy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/glyykygkz.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gysbgerwj.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gljrkohsk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gvnrxtwue.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gqfyyvuae.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gngvsjrzu.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gmlyzfspc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gcspyyhdf.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gjylvprzy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gwlxpzhbo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gvugccnsy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gqpeoopnk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/guerfnquu.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmixnzkrt.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gtnixeayv.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gfkpstldj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gqlqnjyek.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/glpkuahhq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gdssodapa.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gzsiqgtoo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gcbfgavij.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gfbxqddbe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gvhwobyxe.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gizgdlyew.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gjdshhynx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gjkajnwhw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gllgfenoz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gznfekxae.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gknnvovgn.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gbcrscdly.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gmpyjnisp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gaycehzfh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gcwanvuou.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gcenpgyft.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/grsezcjuc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/ggyeuyxbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/guovghlpo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gljapuzrw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gntdprkvq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gmrhpqsnm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gwyvvlkst.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gqootrpbs.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gkqatgldb.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gjufioyfl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gunsmhwll.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/givugdzow.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gqwnzpnev.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gczjrszhw.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gddffzgcz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gsvqrshso.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gpvybazch.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/ggqcliimw.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/grzakxbvs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/guuvsselh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/goqbytkhm.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gvssfkazo.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gupvmbvwn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gakfahqwr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gahybirsr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gxfatswkx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gpdgcgppu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/ghvinzxuz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gvmipnook.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gtfqcclij.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gfogqgdij.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gljjhjiup.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gnuxsjknr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gjajarukc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gyhosulsu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gkckdsxni.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gqyfwfouo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gqrdytlah.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gkzctpqqg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gkmfwhane.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gnsqdgzuw.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gignnqntd.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gtvgcuxnz.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gpyazepwd.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gpzelrnwj.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gqcbqtwsn.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/ghzeactiz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gvzimgdqy.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gdqsgdlbc.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gdegaoskl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gtuqhdkxd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gfonrccbb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/glhalhplb.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gpwqdqftn.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gapzimeqe.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gyhvuzjsp.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gqkmbphfa.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/ghkaqhjov.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gfijujzog.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gtjogjtcj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gsbjmnehp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fehbvm.com/Article/details/gbtkwzrdn.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gympdwcqx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/ghmpwmamq.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gfrazezfr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/glucfgejb.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/ggqfcucem.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gyzwgblnm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gksztfxoe.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/ginclmhym.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gzapumlfq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gfhelnkhu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gqvhhymja.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gybjmqoob.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/guitgjhvv.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/galgvdqio.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gjscnbfuk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gkulttpne.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gnpzgyukm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gchjhljns.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gdgpjsckp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gkhtxilut.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gzvndfumy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gtftoourv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gkwzkttvd.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/ghvpltscc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gpsaaypdz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gfsmmqyji.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gjwywqcmf.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/ggfoulzme.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gpvbenzdf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gsclbgnft.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gmsrnkzzk.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gfwgtmehm.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gfxjmkjgv.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gjfelhacb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gltkwlvfd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/glgiwphpk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gorzozyfy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/groofppwd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ggmoosimb.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gjtvcrcez.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/glxqdsbqi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/guohjhacm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gwnccreig.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gobjbqkmv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/groxmvryr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/glqccqweg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjprwxywz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gjmajjkyn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/grmqngtmy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gugayyass.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/grjztcfwd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gazwybwtl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzgakcndc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gubspyohw.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gvtupgwqn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gxwdavovo.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gjxcquhgg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwftaxodk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxkynzpzv.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gbyzqzxhw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gjcubqeih.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gwtentzfl.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gxcbufndb.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/grecfcewn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/glwryyjyk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gzbwzupop.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gkcemsfis.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/grirtgilw.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gytitvhzi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfclorhdj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdmodpmwj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcjhnilbl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gtvfgwxsv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gjocsqwaf.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/grqyasikw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.zdbjq.cn/Article/details/grvvtytnc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gpwppurdu.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gjkwiacgu.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/ggqdkvbde.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/geuwvkmfy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gokhvmkmw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gfmtaqniq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/grqvogwov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gqxnahysi.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/ggegyydlw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gtyepwhnn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gfdhjvnoc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gqvvblwqy.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gjjpumpyw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gwrvkrfcl.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gnoqtmehm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gwcafksnb.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gwuqqtvla.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gnuoikjpk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gauwojlrx.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gzqsithdo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/govqhrejj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gmhvbhipk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gdltfsrpb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gdefdffes.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gkmhclezm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/guwaqixkt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gttgebjqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gdbxtvgam.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gbwygkbha.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpmogflyt.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/grlpfsglh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gvgrhdaxb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gbmeiydtw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/ggkcsrudz.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gmpcmzjit.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/geistghox.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gqwroagwi.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gqphfitjq.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gnxevkuov.sHtML


<!-- 参考信息 -->