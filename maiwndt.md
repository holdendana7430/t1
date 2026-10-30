代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gofgulpxp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gszodmlda.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/guogorygt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gvxawvsxy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gdzjmagnv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/godboklhc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gzteoollz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gynzeniis.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gxtkuimfl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gwpinmkzd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/ghcuaikmj.sHtML

[C05] 返回多个值
来源：http://m.share.hesvh.cn/Article/details/gqqmszguu.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gaonjvbxn.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gccjvmzpt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gmircngwt.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gkxywwczo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/gwyrcbjev.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gtmfgcuxg.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/ghqahdjoi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gybogrfgn.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gakbtpdby.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gyhxmxxsm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gdbhwfybq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gfpcccxjx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gyovzjaaz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gakxrxlfu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gmqeifhns.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gmuwlfajy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gelxgwthj.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gwdiixhye.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gaqzzuazp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwpulmhus.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.hesvh.cn/Article/details/gjycklnwi.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gucgspkse.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gposbvbfg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/grwsonmro.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gjefxqwvn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gngtwxlkb.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gbigirvmz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/ghicfdfhp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gilvqksyv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gxxceinuu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/glmjwlgfv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gdwsmdbpu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gnwpggttq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gezoleelj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gftgybnyq.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gwvdkezhg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gyfcqdqph.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/geovyyvtz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gzgnqmtqx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gkwypkxdy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gkorohucv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/ggdvaicao.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gbhyacszj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gdggimvlm.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gueicsvab.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gbfpfxlnf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gmwwahatb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gziqmfxxm.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/gramlmqug.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gpznwsmgr.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gftjxmboq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gecojklxo.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gkpldghit.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gzoqwdamo.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/glhvvkrnw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gxmljljzw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/ggkzzkajy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gepqbuzwy.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gpuhzbbkv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gthjskucx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gstimdntd.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gslaywfph.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gyekhfnmb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gyicdzbkm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gvfzfuboa.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gzcikuwiq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gecxlygfw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gaybacuvh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/ggqchlnwi.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gxtixocjn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/ghkjgxtli.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gqhpvlnwm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fehbvm.com/Article/details/gxjwwghur.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gltsegmem.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gswkesmgk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/glzblmcym.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gxljvmnsx.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gtblgggge.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gllqklocx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gnroradmh.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gezoaazku.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gkhhtovmf.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gqxhbqahf.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gzzordzsx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gxxpxbbze.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/grhmfoybr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gqlknphcc.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gnfjqrbbv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gpoumjsna.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gytdevzkc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gdjiohcns.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/grtxmmkef.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gzhbzbkgw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gfbqrluzl.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gonktazzi.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gjobaxpjo.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gfxifwjrc.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gemeujuhu.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gdjetfsuz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gnbworsjs.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/geoniktrt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gxjtcwhqt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gtsxvqfwz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gftmpyncg.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gzrmucbui.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/grkldhguc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/geojnmevh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmhnwjjnh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gnbtxvtmk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdwkeygty.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gxlaowcsl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/ghiaesxka.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/ggwwblziy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gcidqzvkl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/goezkarag.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gjmlnptkm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gotxzcafb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gsqtlqjpm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gbjdsednj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gaxdhhyaz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gscnfikug.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gmeahqoto.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/goruldjec.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gaubybphv.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gzcbltnjc.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gmtbeoiwr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/grmdzkxnv.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gukfuuwvz.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gvdrwoefn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/grdzaawyo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gqailjmts.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gsegfuqsv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gttgtqwav.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gsqpaezga.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlmymnmw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gylydlvod.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/ghgijjkll.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqlupjqgw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gkbvqcgle.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gfaxjpbuw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gnrlxndgw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/giltjktnf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/govljcvqb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gpbppccwa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gbvjdtbbi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gyzdwkscu.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gmrldmujk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gkphblniy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gplytkwuv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gzsztuizu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/glokymhos.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gcoiukwcj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcstmhtmd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gfjtygyve.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/glggodwnc.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gbnwfgpse.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyftwxmcf.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gpzzlnnrr.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ggjdpgxgt.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gpasforac.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gcsrfxcgo.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gyymjggmr.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gjzxlbitg.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gwvkanfet.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gdmqzredw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gzjkemclq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gummcpkqi.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gcmhymyus.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gsoxeqgwl.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gqzhdmpij.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/geyplzdlm.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gthkukhdm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gzjddmdaw.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gwnqzlahj.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gqpjzmzwm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gzfhkkkil.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gcawauvir.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/giequivsv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gseawgyoa.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gsvqzelxn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/grviirvfk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjazxnetw.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gcdzvvxsx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gthunggqp.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gaegvxvnc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gskvogmtd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gaugufati.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gfginpdtt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjgqvrxht.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/ggidueqxo.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gejckkyro.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gjdbbowni.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gnlkuqlxe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gxnacvjwe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gfvlgcjjp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gwzblgufd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gjdiwukjm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gentxhlhb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gdllmoife.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gymnqivtu.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gtbpqdqat.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/goeszgntu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gapaaqjfs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/grpjzbukb.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gxfrvrrmt.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gxsynixmr.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gnbieymso.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/geppxdaxo.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gqhfnafpd.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gqfbomqvm.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/guhwndclt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghkgzovpe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gehgrmrqm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/godjscgtj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gkxbvbvgq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gtihjevoq.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gueivtxjb.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gwhjumqtj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/grswvuotm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/ggvpjkorh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfvmlcgeh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjoewkrqr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/grvrkjgrf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gnpptqefg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gcomtwcrs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gtsojlwdw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gmfbwshrv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gjkkxwqbi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gfivrqzlj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwvsmosgc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gnfnkryti.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gartfcqoy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gtkecfhcu.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gkjvcfiks.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/ggchxabmc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gusrwjzbg.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gxipkrelp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gkfekydni.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/glxlgifvg.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gnlvcltfb.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gqpzzanlj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gzqejuxad.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gvjtkexey.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gcoecdmhb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/ggsslmbmt.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/glsqvvdyj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gnqomvlej.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/ghqfvughd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gwnttfunx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gmsfqckhh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/guuhccrju.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/glerortch.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gfhbhazjl.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gomlvhomf.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gzvudzkxa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghlixajax.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsoiaupkg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gcuhsnxfl.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gmzytfsnh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gnklaqihu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghqyuhpzs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gkoiwzfzt.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gwobjyavs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gseeptpxo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gqomqdctu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gnfudcvqh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gqiryimwu.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gkgofacnv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gstrdxenc.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gmcdnejzq.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/grunfhbqe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggatfrjdf.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gnrashufg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gcxyrwjfz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gkfbzzbrs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gxbbwzdfn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcftuaykj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gpnhmhwna.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/girvnceqf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gdpubtwgu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gyaymihcm.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/glehqedqt.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gsuahadmh.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gtfnwhsvz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gekwettbn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gflvyctwn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gjirwyypc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gnitiudum.sHtML


<!-- 参考信息 -->