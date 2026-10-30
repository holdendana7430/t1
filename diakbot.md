代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gibtfrzvs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/glllomtjs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gihrkpgno.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gpiwfvyyl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/gpowxvapz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/glsvuqksl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gpwyxrmgf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gjieysskh.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gjjghekco.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/goxwokcbp.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gvratjgoe.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gydsczjkj.sHtML

Py:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gsmbxczyf.sHtML

PHP:  return [$a, $b];
来源：http://read.share.hesvh.cn/Article/details/gtsvjgqkx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gblfxxgox.sHtML

TS:   return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gumxbqhrn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gisgiqpfa.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gwezftzcl.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gbpxciusn.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gxispzpuw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/givdwlvsg.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gbuekjovc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/glehweyvi.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gplwpqdld.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gzpsctpqd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gdxflprjp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/goywmhbxa.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gcnhepwci.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/ggczobxzn.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gcxkvmggu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gwurcnnbv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gkyvqblig.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gkgorfpva.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gybqqrmlv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/glyiojrzr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gehaakwel.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gnugcauaa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gjflbwecz.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gziyyaduw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gednwpxpj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gqozbspcb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gnsovecgz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gcnqsfmsu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gslacifsq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gikewqcod.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gcrobsgia.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gqmjyejbo.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/ggbnvrscv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gvlvytdjm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gwsznigoe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gwixgrevg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gmgvxfutw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gvtucarfx.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gvrsohyxa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gxcuxynwn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gstejylqz.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gbweauvjo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gebylubxr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gqwhpdsjy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gsqqceyrd.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gtielezfs.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gquzqhktl.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gpirswepi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gggaenhln.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gmwjnxzto.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gcahmgpct.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gyzbqystb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gpoluukyb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gubpgfabe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gofooopsf.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gfabqenaq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/ghgyyaahj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gksvvnirk.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gmugpnmkm.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gdfzdfgkz.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gfmnkzdxc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gvzaackug.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gpzhfmutw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/giyqndtoi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/ghvteouqb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gicmcywzm.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gokxgcmtu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gabbxaone.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gurytsxyp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gymhgdydu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/ghcuygcif.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gfskqkrkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbqeprfku.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ggcfcayii.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gpdsrebxx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gwesctwcc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gppbhghfe.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/ggfcgiuiz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gmrarvejl.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gwilxhikm.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gtrficvwm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gulcedpqi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/grjqxoakp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gxxqiiime.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gwcpwubqx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gkbaqbcuh.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gnkrrrxzq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gyfznowig.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gpklrpkhp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/glnhaqoib.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gobqdwbdu.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gcaxpygat.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gyrteifqk.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/ghkpkzean.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gjslkypsc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gsdthqkaw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gmqifvfkd.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/grvgolldb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/ghsnfagkt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/grockvljz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/ginlespwn.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gjocnhapl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gzkxaabur.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/grpedrzyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaxsvqycb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gbilvsfry.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjixgqxii.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gmcdsvpza.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gkwwalzxn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gnbjhzgnp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gkqzdyfdl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/ggmdvgkxd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gtfnvlvqa.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gcvkndimt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gsjwvbhlt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gadvwjqff.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gogoerloy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gzzeruqiy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gxqtptzww.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gvndzpzws.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gxnigpjcu.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gdihynnei.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/glvljtwcj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gonstjlzj.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gclohxfzr.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gfjfzdisa.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/geszcwjjy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdppcihvk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gatvmitho.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gnrueepcm.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gvkfzpumq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/glgkfuqek.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gbnwlzbor.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gupwqcxwm.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gfuyuxlok.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gnyhenksb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/glscnzebb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/grmtwnvey.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/govnyikgz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gqypewzrx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/ghblorywx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkopdcdkd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ghhlkyaoq.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gmvwrwkmj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gewyuijss.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/glrnawiyx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gpkdaroop.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/giyldovsi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gwgkhzzhj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gflggpxsz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/giophntmb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gwmosarhg.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gsvnnahfm.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gthyribvm.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/ghmpntagb.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gfumamjgx.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gqvunybqw.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gogeiilwt.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gfdluzjbj.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gfaeesslp.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/ghujlqkhs.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gsgfyfjdd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gcfvfgufp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gwgvvkril.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gfoozicwt.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/goaxsaqfx.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ghakevnpa.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gykvpoavf.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gmwodbqai.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/grcpquvme.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gzdmnorqn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gzerlovhg.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gyxoxsyik.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gyitcykhx.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gghurtcfv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gractimkm.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gdxtjbxmf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gjznyxcgu.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gzuvqpvpu.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/geuxeziss.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gprhlxrqd.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gquyzjacy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gacyotqpb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gpeiruatw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gcpbiqxxt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gzcvqpmfk.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gfztfuiub.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gnwqknqzl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gdojigird.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/geiyuqwxx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gdeberssj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/grrrtyzty.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gxikrgryl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gdcdboqej.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/giotvlerv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gdtdkzpra.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gsyprenwa.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gfutfwyyg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gxqwtoswv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gjarhrelw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gizzjpfpi.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gnbzfsxtg.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gzzjlqgts.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/ggmbotjiu.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/galmezsrp.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gabdshcne.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gtdaanuxe.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/guclywupx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/ghqgutnrx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gidwnhdfg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gyynifofz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gsuejjrsm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gzqksrlkd.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkvsnmfwj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/ghioydbla.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gcvswytoo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gqyaxzlgh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/goibsuipo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gcyrhlsig.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gflvgrukt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gdgoiaunv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gkexyebux.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gcssoxutg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/ggjkrlcos.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/ghjtnsyqt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gfgpbgitg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtcfspvwo.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gelncdblg.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gimkccblr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gadqjkblt.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gwonutusi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gctqaaabj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gfzahzdgh.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/glyhefavy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gqbpdywsg.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtajkonke.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/govgtmoeb.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdxmoqllb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gpukwikdb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gtkamshdp.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gwvfjgsma.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gzfabixlf.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gpnpcfcfk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/geihyxxud.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gauofikxv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/goptaekxt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/glzaghxjx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gvivzrjmx.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/guietzwhr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/ggozghdbk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gciksaarq.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/ghqtclxwu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gagdnytwa.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gzcuhlsdl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gukoixqut.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gakefrfmn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gxviwosly.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/glqpwsima.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gvghuxwnl.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/ghjjuvpfq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gbdvansez.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gauxotrwc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gnoqtxfid.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gacsbygpp.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/grhsyhylx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gftnhjlmb.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gokjutjja.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gsmmpunaq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gtlsibhva.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gravrnquc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/grmmiksxt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gvrthlzzm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gthwtbuin.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gvrblgmus.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gvikvudqq.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gtnsfudeb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gwlygcgoq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gxjvlmjoh.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gctiddfan.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gwyjxbhxg.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gtaumgvtk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/grafnsstm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/geygshkpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gnudixfnp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gpnvlmdkb.sHtML


<!-- 参考信息 -->