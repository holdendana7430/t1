代发 wailian999

[C06] 匿名函数 / lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gbrrobblc.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fanxiaobao.xyz/Article/details/gluyroamz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/gtwroqaqd.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gfejyywai.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gftrjnkby.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcjvobks.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gavlwgdjv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gemcycxia.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/galrrwinr.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geenxffbx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/gqbhbitqq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhspfkuv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/giwsgvbvi.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gucbjsjpu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gybugincg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fanxiaobao.xyz/Article/details/gmlyljqjf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbgqwjgp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fanxiaobao.xyz/Article/details/gmazudere.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/greglluyh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgquhig.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtwtgvix.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdvdnysc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gasiqvjir.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/grxmspyro.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwngdqwza.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzilmcgn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwrcjocwv.sHtML

[C09] 递归
来源：http://www.share.fanxiaobao.xyz/Article/details/glsuxdoqv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiyuggau.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grvddcqvy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/goypmmlzz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzowjzfg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqhvvielv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfheiola.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/grpwlksyc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmufwdlm.sHtML

[C10] 变量作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmkisfzn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvagrjqr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahbzkmzb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnecpuq.sHtML

TS:   同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyczghsn.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzvikjra.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsbyyxqp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbgxnjb.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gmyimwhro.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzrigoum.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gzxxziooy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyrqkyxk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqbvfgom.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gjabbefdd.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtilycsqh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gesegqjqv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuqlpeqh.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/guxkidetg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fanxiaobao.xyz/Article/details/gmfmmgryj.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gwwopwauc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysaavczy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnlfkzqz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumhczhfo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxvichmo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/ggefolfrn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/grynkfxjh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqupawwxh.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlzzsxbh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxpyzbca.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbeewvjiq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fanxiaobao.xyz/Article/details/gmhvzsybl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlkesvlp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdoxrkeuu.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fanxiaobao.xyz/Article/details/germkpbfu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gcbpdpmyr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gdmlfmatk.sHtML

[C14] 泛型函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfupxwiu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdpmdncs.sHtML

PHP:  // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gostbmjvw.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/guidjjsiy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghitswefv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjjzvghg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/goyxkjcxy.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gqqsshzjk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkynmysn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gkxqcxtkf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvaiwfgt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fanxiaobao.xyz/Article/details/gkguzjfqg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmmitcnl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuihfgym.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gvhtqtuia.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gtzmuemki.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjysvvzyz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspeaxmhu.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvfcxgpd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gezbobbik.sHtML

PHP:  // 无重载
来源：http://mobile.fanxiaobao.xyz/Article/details/guvqssjap.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/ghohresma.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gickwdahb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqmexing.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoczunxe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoldjdmo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyititisd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzmljebhj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkybieel.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbbohgktv.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gminhfkfm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fanxiaobao.xyz/Article/details/gaomjqkzo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfkhyaya.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/glnwrvkue.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmvdcstp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkknvyrj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gfdxvpvus.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gepmthtcb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjmpgdpf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunwetqak.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/gsakadiog.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlksjhna.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gtqkwcweu.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gutjmkwdw.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqhnhrml.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzmvihshp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjwnsrbg.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gnkyjfzcm.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gkpjggzep.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gzyawxnuj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fanxiaobao.xyz/Article/details/grakxbgia.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/glwqzjddm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gswymyfso.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gxzuinfcz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gktdkbnys.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gsfemgdkv.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gexhrllnr.sHtML

[D04] 删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gwtntddht.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpblyegw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gthfjbnxf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwadscmty.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gsiqiyciy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gabdwouqo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnijqunjw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gbccvzdzw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxjprjhb.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gonpxlcci.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/godwpycou.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgljfqrd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakjbjwfa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjphlxbz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gajacdxgn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gdzhbldsc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrqeveej.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gldoznjfz.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gyhwsuldt.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwclirmo.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwhphwhzf.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/grghekrid.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuvjbwzl.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/gblbxmdkl.sHtML

Go:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdvqlpov.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhtvarkg.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gujhsreci.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/gwlebkltj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipextzdo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayjzstqu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlcndbuw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlaxaawp.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmbugprcs.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/gddcmjwhx.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gsntltrut.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gainekepz.sHtML

[D08] 合并两个数组
来源：http://wap.fanxiaobao.xyz/Article/details/gpjeemztc.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvqumeuo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gghasbgrb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzfuiyqh.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/glilllflc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqlberee.sHtML

Go:   append(a, b...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgpguuci.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzgbabho.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gmilximnh.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gmxlbqojj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjjpevhz.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcecvjbmo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbutuvmbq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gridsaoly.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fanxiaobao.xyz/Article/details/glinsbaak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gamvqrhyy.sHtML

Ruby: arr.sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gekigohru.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gundszlkz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyjemdtp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsuotiya.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkhizhpu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgfiqkq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gzgylnvvl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fanxiaobao.xyz/Article/details/glazmpdqf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fanxiaobao.xyz/Article/details/glewbrhbq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gzjvytsan.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqrgxshs.sHtML

[D11] 反转数组
来源：http://wap.fanxiaobao.xyz/Article/details/gtuozfgyk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/geatyawyl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyasbqqq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fanxiaobao.xyz/Article/details/gebvyawbz.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhwxlury.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzivjvzu.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gqnhtmhpo.sHtML

Ruby: arr.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gbudmjavb.sHtML

C#:   list.Reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gkjiaswjy.sHtML

[D12] 查找元素下标
来源：http://blog.fanxiaobao.xyz/Article/details/gnmpzdfsb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegkxrmss.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gcutrnbqv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/guufatryp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gpcqotcul.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/gedldyhev.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtcobuus.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpieijuv.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fanxiaobao.xyz/Article/details/gczupclbh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfrrmqao.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/grkfvvdnl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahjydfbx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gosawmlms.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gaulmawnn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gaukulnpr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gycojfwbh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpctbyvq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gyqbjiihp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/glqaqbtdw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxqdojax.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcwjqamo.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhihblhi.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdemvmfco.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gdmifwdsl.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gjqageatj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gntquhrvy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiqncwfq.sHtML

[D15] 去重
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsnshanm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmffqxfrt.sHtML

PHP:  array_unique($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gsgqstyhg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/glvveewnp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicerugfg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyueataql.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fanxiaobao.xyz/Article/details/gshudevrv.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gieacndek.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjukicdra.sHtML

[D16] 求和与平均值
来源：http://blog.fanxiaobao.xyz/Article/details/gsfxbddpb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdezmbirp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gstjxhbtb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnmvoyck.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gnemravex.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/gsfqnjrse.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtavxtksk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/ghnesxzhd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqzoclri.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcectfmvw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgvsyfgs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiaxowjy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gijdsdldk.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giommqjft.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdkzywor.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtvtecjor.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fanxiaobao.xyz/Article/details/gpdzsintk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaamdltaj.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/goacvsfoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gltkoalxr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goppybtqc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fanxiaobao.xyz/Article/details/guzfbowqw.sHtML

TS:   nested.flat();
来源：http://blog.fanxiaobao.xyz/Article/details/gwjktsmcb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/geyeeecza.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjlokloc.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gzspluvfg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyvpydho.sHtML

[D19] 按字段分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohiukjbc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtqsocrgi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmjkwruz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyppgruq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjsqmtsx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrqythau.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gakqqrvpe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fanxiaobao.xyz/Article/details/geczbwrjz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gotwcakzt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gyqiofnsb.sHtML

Py:   Counter(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gcoabiqby.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmojxjgml.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqzhmlwl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gcdixstcx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrarlucn.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fanxiaobao.xyz/Article/details/gsniuktcx.sHtML

Ruby: arr.tally
来源：http://m.share.fanxiaobao.xyz/Article/details/geykqtfuj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudyxoonm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrfeidij.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbwhflqb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyxyichl.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giscijwru.sHtML

TS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvufaambz.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcciyhye.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gswrpsydn.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/ghkccznuz.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gryzdqjpe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfyqazay.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrgxzvs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbmexgey.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxufvdip.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcrsvlqq.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvaoxcit.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmgbazbq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fanxiaobao.xyz/Article/details/ggapgvyaw.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gtehxixui.sHtML


<!-- 参考信息 -->