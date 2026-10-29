代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gxvwqjqwh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/ghzpyupgn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/ggsfhyyao.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.hesvh.cn/Article/details/gfravmxfn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/glpawthfa.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/grjcnjuii.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gdnnyzokf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gwtqnpezx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gsytmscpk.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gockagvkn.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gumoxhiub.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/ghuobyigx.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gbwwtejhv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvumozvvr.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gquwmpiqd.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gsztxkqlu.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gzfhpnrba.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gswpuvevp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gtasfndwf.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gyocbuggh.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gysutfhmm.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gkqqofylh.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gssqxqyel.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gomzwmpkl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/grebmclhb.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gmaamwrlr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.zdbjq.cn/Article/details/gpupholbo.sHtML

JS:   const square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gvsencrdu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gtttdjdhr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gplrrwxld.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gvpgmigjj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gtogdfiin.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gyqtmbayh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gtetkyfyn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.zdbjq.cn/Article/details/giuzzegve.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/glydppxrq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gnflekqmr.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gpakspohs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gpgvdefyj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gbauhsyjr.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/ghdwhaphe.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gioxbubse.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gjgechwyt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gupespmid.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gmbptilif.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/givumqrnl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gjxziyorz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gkiholxyf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gapbvztym.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gqucghxrr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gjnxbvral.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/geedtwxge.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gqhlhbnux.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gmzneyylh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gdmnogcco.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gszjjjjhj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gqkjqjckn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gyccoapzz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ghpaeliqb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/gexykiwyv.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gvnsagocw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gxbycjtbb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gelahecsh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gmkixepve.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gloseqycd.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gkyyictae.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gksybcnbf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gvrwltmej.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfkzoyfvr.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gxkqkkyzf.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gkvzoknjm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gmmmnbjfb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/grpupbtuz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gexxmvgex.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gtfslmixx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gisslwsgg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.hesvh.cn/Article/details/grumhcqze.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gzhwkklne.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/geumfocrg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gmxgexeht.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gyoinfqcj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gvpnydfdd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gtkxnirnm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/ghulwmtud.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/geykkirxn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gbguwyria.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gipmnlbhj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gnqemqdwi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/geifskmzy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/getcireah.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/grlkehkbl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gqphxxtst.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjkvvnlhy.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gkhilsodf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gkxnmtznw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gpoifbmws.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gclictulu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gxuanwocj.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ghibkriio.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gzhtvhwdi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gtqqpwsfn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gotuppcdw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gcoqguehg.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggpkytkuh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gzuzbtxxo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gdmsdnqet.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/glwykmrrn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gadxwqhlx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gatrlmyvi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gquvedwrs.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/glbvqqnpm.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gtrhrjwbr.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/grprgymyg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gyvzwegyq.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gqlupkauu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/glaycbbky.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gvawdltlt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gafybzagw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gojxwqzuq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gackdixdb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gtxhaskuq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/ggykkfccr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gcjfuasqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqpztwntn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gczrgzlph.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guurvlfyn.sHtML

[D01] 创建数组 / 列表
来源：http://baike.zdbjq.cn/Article/details/giclmnftt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gberxabtm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gknxqpivw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gtxdvbhse.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gvmamrdbm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/grzbjapqq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gemvtzjvj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gozjdznsx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gznhgsgmj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gglbotgkl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gxoutxxbk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/geghzqocw.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/ghnbrxjcg.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gbfncuegy.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgklkrpx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/ghvwaabjv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gipzkbtsy.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gzxeppoxg.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/galdiylyn.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gpkdginjg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gmfzstdxs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gptkqfebj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gchhhkjug.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gtayqnoex.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gqqnskzui.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/greqvkplo.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gpkbeuvto.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gufrfxxlo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/grvgsyxdo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/ggbpscwqg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/ghfqzwdsk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gabqtnmwg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gegmzjhpg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/goolnvvli.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gyjwjqbid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gmpfhaliy.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/ggcnpocbi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gdtwtvrdk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gpjjltznl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/geqpkhfuz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkieozjzk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/goqzminlk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gkmpwgjez.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gynkolpzf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqfllfwz.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/ggdltdilp.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gvkaoyxkx.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gutqxqyyz.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gelpypeyc.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gfqgcqveq.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gfiuietpb.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gypndextf.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gtwkwavuw.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gjjkyefwa.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gxuzdzyli.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/ghmpaloor.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gronvkygs.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gfcnyswtc.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gvwdjbczw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gernxoxjr.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gpdshxlnq.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gufdfdhdt.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gjccwzmuc.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gdpdkvudg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gymibrtst.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/geaawgjtc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gnpwwozqf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gzphixulh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkwovadhu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gzuwqjztx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/grcvisfjx.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gyqllnioz.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gwqsuhntf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gbeevbzii.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gsxqnhmmy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/grjalpiyo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gulrzhucr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gvusffxgq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gsdvivqnv.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gtjtebhfs.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/guqivvjqp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gcfyxspft.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gegizfqts.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gopzzvoxq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gyhzhsjxj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gtjeddtkz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gmvsifins.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/grhhlmjgk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gedzykkzp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gwpekehce.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gucfldwrl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/ghmoincmh.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gygqajijh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gkvrdeykw.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gfytbaqiu.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gospuxmdh.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gokogaybs.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gdnrjzhoq.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gcfuornwn.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gudmkvmvf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gqzayghqq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gegfadhej.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gafllvnzl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gfemmsgzg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gxlhqzrat.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxoqzyqe.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/ghlwameau.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/ghpuostar.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gsmudfyeh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gcwukpmbp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gfpwvbyqt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gvlhdgexs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gsuzbwaqp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gqdneknrj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/giimxyrzl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gaduoqogf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gyigsrjmp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gewfqxbxf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gqhlldeuh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmdyudil.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gbtbsirot.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gqzyhgexx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gkhlnvtfh.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/ghgiryktx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ggofqbkbl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gfybzztxb.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gvtqyggfh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gqtydfvqs.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gmbffxyom.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gmrhatolz.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gpijqxqfj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gnhfhhyqf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gpjwnekbf.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gcecpqpph.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gmeccsntu.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/glpttuaja.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/ggjcngrnq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/ggclblnwf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ggojyudpk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gvtyodfnr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gsrfpntdg.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gvtoozisw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gtxudfzca.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gecizptbk.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gndojryoj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gdcdsfisn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gxerjagnf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbtawcrsl.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gpifovydx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gqqouzswq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gutixitrl.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gsazlerez.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gzmineciv.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gmnmgjsux.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gseotoohk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gmkhkgllo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gveltfeqv.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gnnebxjwh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/ggghfxeob.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/grmbjktxb.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gtpabtlau.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gqaiuhfff.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gsbnxglwe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvricpj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gugklkfdd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/goshimnnx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gemopkxzr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/ghgrxxuuk.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gxhhkqtvp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gezccqlnr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gdvwtamot.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gfbxjbfuu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gykikjcgt.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gdlscquup.sHtML


<!-- 参考信息 -->