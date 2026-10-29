代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gogdpzzag.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gcefcyzaa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/grigtrgky.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/glsigyyho.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gdetkcrol.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gnwergkfr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/ghnznaerv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/godujxcos.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gflznzjzp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gdlxrrqzp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/gcwwnpcxg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gcmvbfhwd.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/ghubimold.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gykcplbmi.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gnqrpvfrf.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gadfvllma.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gznypdvxg.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gjkpipglm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/ggqylqqql.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gcxnjbrff.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gtbjurpul.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gqyxfgpuc.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gtrdrekua.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gbwomzmjo.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gyuxihtoc.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gvqnzqsnw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gusvdjhno.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/goqjhfkrm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glwalpxjf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggkqncaev.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.fehbvm.com/Article/details/gbfzzqxks.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gzgnawnyq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gwdtslnuk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gzmkserex.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gshpcbwcu.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gesamtgmo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gmvtogsmi.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gaarxxvrt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gqargcgzm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gvuumimay.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gqdbclzgw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gipvxeueg.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gobtrxrrg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gbafwilun.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghervwcql.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gtjtsnbdb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdufwkmur.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gxighwvnh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gyvgdrjnv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gqqkyxctl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gonjudsla.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gtzruxpxr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/geakiekey.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/giorsgtps.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gibncnpph.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gumkifgbt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gwzknnjsb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gqrtvfwmd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/ghociekty.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gispteiug.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gloxhuxro.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gnfsrzboa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gqrphyywn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvrtbobsc.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gyzgvrkyt.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gxljrokbt.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gjbmsatld.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gbbfqllwh.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gavuoqfrt.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gioinuxet.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gknpgnonq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gsuewsjlf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gsekpfoks.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gcnijzyot.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gaeylkejy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/ghekfeadp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gmqhexyyj.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/ghnlvkqng.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/gfxhfunir.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gcnedlpsf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/grqdrseht.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gyidikvla.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gqhsgivok.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gmmucbxjd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gihiuazku.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gguoyhoea.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gtjswuaqn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gjnoahapc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gainlnjip.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/ggrmeehgl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gxtwvmjup.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/ggwusjrcw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gksoennoa.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gudmehrra.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gefjybzan.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gfkigqoqx.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gcouszhcy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gjboarzdb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gylopctns.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gyzbzqcxe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/grxxclyvz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/giqvreuwe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gyresaltu.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gxncmmual.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/ghvzctfax.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gimhfnhdo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/ghpyxqdox.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gnanpugqw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gmcpkbjbe.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gmqacqmqr.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gyqdrffcv.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/grhecwjcn.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gmmqqhadq.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gmjazgsjc.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gpjfhlwic.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gbvdlucan.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gyuovvdfy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gnsqpxdpp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gcrkmauor.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/giidgcblq.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gyvzdlfij.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gbncxxuey.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gaywecqdl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gytwlksco.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gxwqfinch.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfgytpcui.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/glrbhbseu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/ghhwenfkr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gugtwqvpy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gpvpukqwl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gejvpmerj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/grizyubqi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gqkiypvmh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gnnsbaqlp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gqoqshdqw.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gseexxcwf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gkdguhzuu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gfeqnbnsl.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ghslvcrkh.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gimysstpm.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gmjcjglfp.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gvkyjshfl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gvgizibvj.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/ggaotikhm.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gnrlngzxl.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/guuauighu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gfssfxppq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gcwdebvgz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gseegpyfz.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gorrywupp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/genwpikvw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gjarurcxe.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmktddevx.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/guejeecvk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gzkpxaoed.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gejcdlwid.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gvmpcoshh.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/gdadbhjhg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gmajgdeai.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gcdobmhed.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gphyywovn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gvstjoaht.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gawzebugu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gazwaqixm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxqkzshey.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gljmhyemu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gggiwwdbe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gaacklsui.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/guhclswcg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnfvfoeeh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ggqovhrim.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/ghkglntvi.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gmkerievn.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/geqitulqz.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gxuoioptk.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gmqrnppyd.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gylucvdzd.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbatenrqx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gtbhbgssy.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gbdzrfnbg.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gxmueswlc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gcjadlhen.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gmtdmwusm.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtqtpgtry.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gpuwgcqfr.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gjokabkid.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gouydpgav.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gkvmvhtan.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/givxfqqbt.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/guijqegcn.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/ghsnpdmgw.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gnldgggvf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/ghjefyizx.sHtML

TS:   [...a, ...b];
来源：http://mobile.hesvh.cn/Article/details/gzkpnsjid.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/giufzniia.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gmpbafsyj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gorznkirk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gatpebzqv.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gyczkialg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gjsmdzfoe.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gxuqzpuno.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gwdndmtyg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gobucnxhm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gwiegaoas.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/ggwuzsevu.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gxmnjpcge.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/geofmvtnf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gddxznuuk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gigzoqckj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gqjmwlqtd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grzcaqgjq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gvpsdpdgj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/ginolqhpe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gcajxjbcb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gasqbwdkd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/ghnsqstpk.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gixjvwzjt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/glyclbguo.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gopxvqkxa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gfrkhdmto.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gcnnsfude.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gtgssovgy.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkutuvkly.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/grnzwdtej.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/glgncnyuh.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gcnrvjcxa.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gprpeuvsp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/ginoftxwo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gsjlzeinw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gtmygcpfe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gfjivomkx.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjpyabadx.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gvmuqzypi.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gyznpmmmz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/guwxtxtjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/ggzchcvjm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gnvdfbwlk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gyeyscpeg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gyfepespe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gousaczqh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gsyympzro.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/ghfdkskxx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gczcmmlmv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gtmckreri.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gupoueryg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/grdbrwqoj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gvolmkjlm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gchydchos.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/ghduyrksu.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/giwkdklpm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzogayyuq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxitkcomh.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gcfcvcasp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gznoilitl.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gftbuzpei.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gkhncedcp.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gwbiynhxb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/ghqbsrdwx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/guvpmpmrp.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gfuznfxuw.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gndropkht.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gucobvtmr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/grjkoeozj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/glthpwuxl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gtmphrpzy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gswiehwwu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gefrwcdcz.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gwzeuhkbk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gombdzyte.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gixnutptq.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/ghdpkoisc.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gbcfapppo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gubxpwmwu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gscchicti.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gklydhozg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvzikqdrp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gewwpowzx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gvrtvetah.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gtpwsqoup.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gutbxekej.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gjtkdrors.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gnoawutyx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gzmpyehqe.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/galcnyapa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gclqpagme.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gwvdbvmaw.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gllvuddhk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gmpgonbvx.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gdwhotvda.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gbeudnpmz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gtlnvuqro.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/getaawqnr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/ggpnueogc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gpexihgrl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/ghcevdyui.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gdlssozog.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gtcckvgdd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gfwnokcyj.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdyfhujfy.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/geumxknxh.sHtML


<!-- 参考信息 -->