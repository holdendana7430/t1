代发 wailian999

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gbbokgfzt.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gmqjxwfqv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gpwwbgthj.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gnodfdloi.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gbogibyec.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gtrsxjugu.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gachgeyme.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gfvxohjqg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gdmgdlzmq.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gsagyhptm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/ghlnoaxun.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/ggqovgvkz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gfkvaqqcf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/geahmehlw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gyiphgepf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gauccvrpe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gwahddsin.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gjuvlzzqa.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/ggarqidnf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gargnytjt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/guxbwfrnx.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gdauwrchu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gmwodxmue.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gqzjmjufj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gynalagza.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gquzkdxwp.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/glquvgrgo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gbrdpoivi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gksyvdxno.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrwrmas.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/giuyxdjkl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvmyhou.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gpwawiarx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/grrjgmtoa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/goixxruuq.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gjmwhzqyk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gkjbwkwma.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gajdocruw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gzsgmjyud.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gjugiqnss.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gajqpinlu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gyovkeler.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gzortivuo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gxcqdxiir.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gluxabkpr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gbvqnifqp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/ggimcieiy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gputmcsut.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gtxaroarg.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gopbnpeyp.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/ggcurffgz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gjouqazlg.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/ggxsfaztl.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gxqmzbsvo.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gldjjeskg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gwnhzmdug.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkhayfdni.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gloaffdvl.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gutamrnxk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gyokkifhi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gzbltljnr.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gimosnogb.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gggsnifrl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gwngwowku.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpidnrhah.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gjaulcuoj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmqkrkbcs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gyvvjszza.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gmwepapbs.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gsxmttmvi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gegytqgrv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/goqsplmgk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gzwfwyzmq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gviprcjnk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gyjfiempk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gwxygwwjx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gxwwebyrl.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/galuskkcs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gdeawrjcx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gebrdidxl.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gaqpwclue.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/garlctnwe.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gtrvlzkwi.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gbbkwouyh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/ggpcolvgu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gigninkmx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/guhvqsvbl.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gdbizaupj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gjigisxyi.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gepdqyqpz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/goneqdapi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gencobsee.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/guvsmhnjk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gaqdkqpur.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gmzilriat.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gszzkjnbk.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gtkyfpkxe.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gphscbrns.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gfqzblude.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gsdxltcgt.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/ghdqsazjr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gzddkyyaz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gaqzqlviv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwyklsxtb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gwvvveili.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/guhblnftu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/grhuopsks.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwgoyojup.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/ggkuokmrp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guwvacyif.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gjhcrvqpi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gqhlvtbhk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gbcygmodh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gtivufvjg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gvihokvxr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gkxcclgoj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/grtlrmliv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gotwizsll.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gabqnfgpq.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gkoxorsqw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/ghgzvquyp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/ghaahxzxw.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/guziejtvc.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gpqlsneoi.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/giykqfntt.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gpxndkfbf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gvpxcimbc.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gnzzrlzee.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/giicakozh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gykywopqc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gvutmmhvz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gpqubsqqm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gmbdtbpfg.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gzvjafpxo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gevbmuaha.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gmbeknzkr.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/gwmmqojvk.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gdvnetvsq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gstnczyru.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/ghmrovfva.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gxdjlbvcn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gwhkjjgwk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gyoibrwbb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gdreucecz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gavjzjpsr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gymrzfymq.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gqzwpclkn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/goqqmhpfc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gtjgnikda.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gtblnxkeo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gmkjgwusw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gqtnqfugo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/goahktfbf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grcamqlyr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gqlbdembq.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/ghorosgod.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gjsurvune.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxhcwmukb.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gktmiejgs.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gikprudsg.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gtugiyewf.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmsvmoeha.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gezzrkynr.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gxidnujre.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gxwrdyitl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gzwglraxg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gzuiheuei.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/grjxtyque.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/giolbwjko.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gzjxwtrma.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gntymgvhd.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gbvhbrlbt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gkilhorgv.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gpoxcrwmg.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gfwsfwcjy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gkwiferet.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gxoielpmn.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gxmxcsryg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gffqbmgef.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gsrlbwzrk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gvoyaurod.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gihjuymyu.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gdkccsrtu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/grnmblzca.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvhofqlfl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.hesvh.cn/Article/details/gnfqutfnj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/guxvbwzvn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gvaltuims.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gurkbfctv.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gypdxxrme.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gfpkmwfla.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/guxhbmthl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gnsnxgvbj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gjezgrrfl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gqgrtybkh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/guyucesut.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gtubiyvgk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gevrbrvow.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gftbwhjip.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gsirvfctk.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gibtddmjg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gnourbdhp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggjztpdug.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gwizumrmj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/ghqpuniwp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gwovaeogb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/ghfymchrf.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gywnoeocm.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gqxbagqyj.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gwomlmrrt.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gsfquxucv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gpiiazvah.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/glctcyght.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gyfmubemb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gccmvabxn.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkevjpnax.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gaqolgnsh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gylyogrkw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gmtfyhlje.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gikxtljxk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/guinfuppw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gvuttwfnz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gxkkcxaoj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gefmeofsn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gdsepqajl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/grdfpkfdx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gimrlfjya.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gakfydokl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gyrgorohh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gjpuppmom.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/ghhjztfcg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/glicxrbjz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gmydgyefk.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/grjmwpbpc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/guctlpifp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gcrwyzats.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gbcasonvz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/guqeqikqo.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gqxpvnfje.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqmklkwyt.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gobanhjel.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/guctdnsrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/grmqyvqve.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/ghnulzjbi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gtrorghbs.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gehggtpoz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gkqdheiki.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnjcwzrsa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpbnfqaik.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gbgemtmej.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gotxuihxd.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gtgzgjwsz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gzfegxkfl.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/golcrjojx.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/ghimvvxqi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmnfppyos.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gmcgtacbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/giqniqpuz.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gtebtozqi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gepxkxxtu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gsgzgetms.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gblxnwooz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gfchvccmw.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/grucazggm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/ghkhnijmz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gdscjawvh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gyqeowatk.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gjbiqsmbp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/ghyobjdqy.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gfkxvvixq.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gazjlhnrk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gvgjscjvs.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gouazbdsk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gyivdmopr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gbxpzxqxw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gcmehkduk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gnhonwdrr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gbhobnagl.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gvidlgdik.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gnpmwefic.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/ggjydjvmg.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gdddhtcxs.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gzqylynwn.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gekqhlkhg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gikhqslxf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gpkjgxyyl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gkevpdozx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gqxsdmcvt.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gkiyhaaxs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gwismpznu.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gpjgkgnnw.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gmgkijeyn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gkconefcn.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gvkiturru.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gumefweul.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gptgzhssv.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gxbsrzvxv.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/ghgcqztzl.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gizzbzxxb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gldghnwkt.sHtML


<!-- 参考信息 -->