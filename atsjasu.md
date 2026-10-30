代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gvkbength.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gfkfzngpa.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gdzrdwkew.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gihtkkxny.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gnqbteufd.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gurfoxxcv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/ggugboevt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqamsmlml.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqmsucdv.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gqrzpjohq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gxzybygyt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gjhjnedgf.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gpltqmybx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gmzrgkzky.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gwehwyczm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/guixjcmcn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gxwwphrvh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/guyvjiosd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/grxmkfhiu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gmcdxmzmn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gnmdkbcbd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gmjwyztvd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gblnxbfub.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gvumskobo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gmhistshg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gvulnmqfh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gbnjzalwh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gatyqeowo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gjcpcpdvx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gkuwbbwia.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/goiqkzktw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/graewways.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gytseapzu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gxpjjfbgx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/goalstwzb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gptxrcqqe.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/grqktyrfn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gnnsmhyyk.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/grszmdcjr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gamhzawnb.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gmuvuntzk.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gzymqvvpb.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gofiyofjd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gkttnxvlx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkbfjqmoz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/grvicljan.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/ggepkfxjc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gbisekjsy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gwasonmyo.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gujadznas.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gfopocdnm.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/ghyuzghbu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gtwyllpap.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gyphwgcaj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/glhfgzcor.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gpmggxfyr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/ggvdgqery.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gxmusndjq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gbsfbekel.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gvwzvbinz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gggrbqysu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsskmwrdx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gajsngooc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqrfwlqcn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gigmutqta.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gasaetvbt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/guwfikmco.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gerqxtrte.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gmvcmqssf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gcsyaezbj.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/ggsmcizel.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gkarikpac.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gdxpbyjke.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gevbcuvbo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gpuinmipa.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gbnvsqwhm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gmjczlhzn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gdtsejysu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gphmonwdr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gmzlradji.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/grgjnirus.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gmeusebnq.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gpjmijjab.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gmqklmwet.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gdhzrubrz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gxihwdmpf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gotxvmriv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gljonwmjx.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gcxawzvdj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gvijqaueu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gsjkqnzae.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gdwfstghe.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/grylhrzrq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gpyhriddz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/ghozrtywu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxvvztbkz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gagipkxjv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvypqjpmw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gsrpzsuge.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gubybacic.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gtjxssxkt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnxzlmbvz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gavhouhkl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gubdypobc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gemlriinj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gwegboubq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gojfikciw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gheavczwz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gdzluszqb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gdjhxyfiw.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gvlrbkujz.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gbubnloqg.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gogbwmuzi.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/geymcijyz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gkzhsusft.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gcoiygmwx.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/goeyrqghl.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.hesvh.cn/Article/details/godxzzqcs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gpvicyqok.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gycmnfaim.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gnkklntok.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gtkpjkvud.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gnlrtwgcl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gbyempzzn.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gzeptslzl.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gohgicyhr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gvmalcsff.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gojpdmyfn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/geqokxnlx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gjjndgibp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gxlefshdz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gntyrrcxn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gxavbopxz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gzulotccl.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gvpimanbo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/ghhvkqhqe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbmlvmiwa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gylxptcuo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/goboodbmy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gnrbwatmf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gmgotcyqw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghkqnbqfk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gplncgxqs.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gevsocdaq.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goywujmvw.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/glekuiano.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gcdoetcvk.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gjnzeuaeo.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gvkbbdpnd.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjrtcfccj.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gjktsaogb.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gorwquvmn.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gtqiisjhk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gkzehiagn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gkbqdgxtz.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gbwpeofpo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gbijhjwjv.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gmgfkkptz.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gqjjesixw.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gpepkwesi.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gdwkzwwbs.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gmhemdoxh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gzwvyhitj.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/grcaxsdqy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gkqskxbtl.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gjhclzhcx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqxlcknfa.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gfkvlpptc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gbfkxesrb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glutyymnj.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gksgacgkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gfevyaeqy.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gwfnlhqks.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gtuadaljc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gtppbpdbf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gthkoqtyy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gfhdbsnhv.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gutoivajy.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gyejmzsao.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gxxxipglp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gquvwfope.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/ghxvfvyxr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/grbuxkmgj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gclzsjrjm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gmvwjohto.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gqzbugklm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gyaksmphc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gzpwcxcdr.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gfvxghhhy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/ghovnzyjw.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/ghvajkqwo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gwzbidfie.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gjamlnfbh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/ghoozztww.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/giegfsben.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gjgmyssau.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gpdztflun.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gkdegkgsr.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gewysvfbd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gaqacofzp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/genofrlac.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/geissbjsm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/ghllvkbbw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxfxiabto.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gesqvkufz.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gkaiulgxp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gatwsovaw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gqobonowv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gefuraehk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gzrozehcl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkbvlfv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/guoqzkutg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/glyrfnfce.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gwzksuykk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfqrqakce.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gxatsahkt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gqykybodl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdvotubyf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdhcthgfv.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gfqgkdtpx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gtxalnyha.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gzhdrlrwc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gqocasypw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/geqfklwjd.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gdtxsoxwx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/ggvhwhhkl.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gtpgxmlzd.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/goqhdarol.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gbqtvugkj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gjgkxlntx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gxquqveht.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gkdzyeduu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/glxnvjqnu.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gutipnypc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfyhfwxxf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/grzsnzlpl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggahieayn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gowpbsfsc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gkjvdyzal.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/ggrrlgqan.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gavjywkmm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gjpiefzoo.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gwcbfpjrq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/glwdaqcgm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtvmugmlj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gnhrcrtji.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gecomcyod.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gzwjrpqsl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxkxtoqfd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gkgatnqxh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gmwiygekm.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gczokerlp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gzquubjlq.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gqltrsywk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gudutmscx.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gxmscthvd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gezkwwviw.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/geswxpjlk.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gytlrqzfq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxufaetlm.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gyjzniuxz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gpfxuzhsm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gyxourhbs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwrxija.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gqrwettlo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/giyuhuqdi.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gnbilescc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/glfzqhvhm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gxyaybfeb.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gauzaasto.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/glxgpiccx.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gnayrlvse.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gevrzgrbd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gfhkodkpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/ghatqmzof.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gklszxedh.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gkzfuhljb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gpqmxfzvg.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gshcowpnf.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gpepbaxuv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/geofithfs.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/grankurtt.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gsbpwedgf.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gbqewqofu.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gqxbdopfn.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gdexmdtdz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbbzwnkrz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gpgvijhua.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/glqygawfx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/ghphdqnaq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gjrnsgfrb.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gpdawujux.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqvzbtans.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gsjdnrwiq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/ggdtuwyep.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/galgwcgjn.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gxzvxifwy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gwtooskyb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gllfndgiz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gdqurhrwx.sHtML


<!-- 参考信息 -->