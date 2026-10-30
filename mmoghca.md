代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/glfwbuwik.sHtML

[C03] 可变参数
来源：http://m.share.zdbjq.cn/Article/details/gtstqnxoe.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gschkxxrq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gdyyfuzps.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gekumeqgg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/goojqvoah.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gqvpvzzij.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gbejebipw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gatxutkzf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gsfidhhva.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gpajgllge.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gqivhztvl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/glqdpbiwu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gpjfxjahe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gcetkasnt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/ggsrvadwd.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/gnpwcajwv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/grccfoznf.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gvxqnhjhd.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gsdivciuz.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/geqqlvzmq.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gaaysubws.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/glovkuiiw.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gpsihcadn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gdbfbarij.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gtilstrqa.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/glzvvqock.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.zdbjq.cn/Article/details/gzikyjuca.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gzrndevjb.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.fehbvm.com/Article/details/gornzpoyh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gbtyzubha.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gyaoewdee.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gkffowbxy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gnmiakviv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/glvigpsdy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gygxsvbah.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gfhbsuwbm.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/goabyawzk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gegfyjcgk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.hesvh.cn/Article/details/gcodulmcv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gesuflrcu.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gmnwhgtpk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gcmoumway.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gugvdtyvo.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/glocwazlb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gmtjoqiwh.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gjioarjgd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gqtytbdwp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gktzlqnqt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gapqmztvs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gdamkutqr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gzvzmpqwf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gfkxuflml.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gcqvewghx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/grrvwukao.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gfztzrxsj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/greaxqljv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gciyylwgn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gcmxiglxm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gisbigkxn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gggepnnse.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/glxakinbd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gtahzcako.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjwumiw.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gickabqxs.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gdpuxomdy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/guwsmuryi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/guhynvknd.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gvgbrmmja.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/ghuldcemw.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gtmemhnez.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/givbzlldv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/growarqcs.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gsppiecvs.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gxerhjciy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gautscezq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gpimtnqsk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gedvcsrmi.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gqtgjwexn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gpuxwasln.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gmjgauozp.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/ggdwvslaa.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gujreyjhl.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gbydvtmjw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gkuebkuoj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gjqdoiyom.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gngxthrky.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gbjcsshuu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gacnvrtzf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gunqprhbe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gmiooubxf.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/ggfwotncn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gnjysfcwp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gxzduozoe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/guntkykvn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/giyxwtblr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtxotfnap.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/glhfltlue.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gzxorgwei.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gkekkmjkz.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gcfcoamot.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gqxcllntj.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/glmoorypn.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdcwntmhs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gbyzdnufa.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/goayffvdl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gcnoalxfn.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/ggvoqeouk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gvfusxvku.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gdbotpmsy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/geydbjzro.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gvszogygg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/grlxoebir.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/geuoszdhn.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/guydyaatg.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gcvaexfrg.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/gsiwxyfzc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gpuaxfmhk.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gputeyrxx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/glgpkmdjw.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gdeqtljdf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/goztaisms.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gepiggnpn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/geqykiwlt.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/grobmykwh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/ggybhsdco.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzptdvstu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdmvxaqhx.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gtptketwc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfcvgknlp.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gtqrytwzr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gxncfkuzy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gexxlowcm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gkbiogonf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gygeaiusv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gcozksljl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gsnnycxec.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gjsxhbffu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gekbjtlod.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/guvbksdml.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gpbsllywc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gfblilwou.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gcycnepcp.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gkpbogtxr.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gtsvqjavx.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/ghffnrwvt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gxhdjevnq.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gneupghbl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gvmgzpost.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gwrrxdapn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gtcjqxnjn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/ghxhbvwbu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gyzwhbdnd.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gnbixexyu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/guheaazan.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gmizhybiz.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gmdbudhpc.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gzzrqooll.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gozwiegja.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzzrxqcag.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gkjduxeiq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/ggtnggzsc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gwqnnfksi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gqgexbsxi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/glyrqoqih.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gubxyiwic.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/ggyctakmk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/glkvkjsvq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gapxrslxi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gqiywjcge.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gktechnqj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/ghcvsxkhv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gjzlomeeb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvrectndw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gzkjfsleg.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/giladabsm.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gskqxsgqz.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gnznsfuvo.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gzgtbnuvt.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gcwgjlapd.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gsspkzhnm.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxktgmrtu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gkmbnrmqd.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gjlwygkml.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gnzenrasg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gebomxsvt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/guxzqwfll.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gtqfgphdb.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gingojdul.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gomezhqtq.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gzyzthbwc.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/guebjsqqq.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gfgofdpqs.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gbhittuak.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gwljtenib.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gyzkflmsu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gcmgspelb.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gyjkmdtvi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grmtbkrus.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gcxvxfagh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gcjuwwhvq.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gablzcybt.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gjljrpvbz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gvtxoigpm.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gsfomaqbh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gomwuyqlm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gppfylibd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gjgzdewlz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghoizemwk.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gvvumhhix.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gflawyvpn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gybfhjvdz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/grixbxkll.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gpscepkfm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/giuhkmapt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/glativlcj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gvwcxrqrs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gbjlceezh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gkmlucxzv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gvqwssmkz.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gzmaqhbqm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gwalnmshd.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/grgdpvpco.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gstzlgddl.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gcmlpqkhv.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gobjsbodf.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gvnwvqalv.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gpdborwjp.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gpzcyjxzz.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gokfzhkrj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gzzzfpjwy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmcxogwiq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gdszwuvou.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gsohcfzyr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gyoidyerd.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glksgotni.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gjnscxepx.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gegyinauo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gdostobyf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmydciq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gttupfzpv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/grkxbqkyy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/grkwaceuc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/guptqrvim.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gwhlorjbc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/goiwciyuu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gmzqqfnnh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gucojhqff.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/ghncuhzbb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gplgxvakl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyxrrjsvy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmbffgouc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gafxokuja.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/giiydljws.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gdnnogcjp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gpsorbbtk.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gvhynmjxp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpvrwaola.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/ghgtegrur.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gjqttkohf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gnyjyqglp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gfmniigrc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gqjyqqpmu.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gylfikvmu.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gaibcrulg.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gmvhxepnw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/ggwahpxqy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gckudhbtd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzrezhfw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gnqxbwtkd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gyyooxpvu.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gmtjxnewn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gauontpoe.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/ggfdgegwc.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gtsbtsmnf.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/ggfsmsnmy.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gwlsqdgus.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/grpkguotj.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzmlijch.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/ghtkntwbz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/glhsrworo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gbgpbgjqf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gntdhsksz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gmiucqmfb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gsmscskxv.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gixnsnzip.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gebhuxici.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gyfojogyy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gjaehqvnw.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gjylcqtug.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/geuxxkpiz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpxnahaxj.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gaenudsex.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gyqqxywtm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/grgdacibx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gyyvxqadg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gximjkfjw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gkcxdyzgt.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gvbiadbia.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/ghzvkaonr.sHtML


<!-- 参考信息 -->