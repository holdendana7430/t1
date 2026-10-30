代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnylrjkl.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/gepqjzlck.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyjyopjx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fanxiaobao.xyz/Article/details/gecrnyuvv.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fanxiaobao.xyz/Article/details/grnmniiob.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fanxiaobao.xyz/Article/details/gqfgwttwa.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gehlmgaaq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcplnvscq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gziksvwas.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.fanxiaobao.xyz/Article/details/gqqgfufuz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/godokcydb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gkkpeqdsk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrxspvkk.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuiluvhn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fanxiaobao.xyz/Article/details/guclogaoq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeevsdmi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gslzrqyto.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkufnior.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvokrgan.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gougzdeyd.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvwrwjjk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyfmymsa.sHtML

[C08] 闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwyxoxmu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fanxiaobao.xyz/Article/details/ghvminwoj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gydffqaaz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvmgwbmr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqprpnzsl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifquclww.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbwguqyn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgsnpfss.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbdgyakmm.sHtML

[C09] 递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrursryd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhjthkbl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdcnopjq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gfguqoeas.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/grmfqdjsb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfcmrzly.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fanxiaobao.xyz/Article/details/gjtbsiitg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gszbeqzwd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjvbubmv.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gjhgvlcaa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gowzurumm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/gycclmlwi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gugadonbf.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gfigepcsl.sHtML

Java: 方法内为块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gptcglfwa.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/grqjzxawp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fanxiaobao.xyz/Article/details/ggwbznjiu.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gmdnljgms.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/gwzxeyacd.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gcsrwioyh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqnzhxbl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gaqoristz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/ggohwqmho.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gtqayqtkr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/guryenjrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gjtjxmkrn.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgcolbvv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/ghjtreffx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gjccowgzf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/geffygxvg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfcgvfex.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhvzjigk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjhqkqns.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkgpyloc.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnospuvk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqmibkav.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gzfefcrys.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gpbwntdar.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gomhulorq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gfvpplkec.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjusurwzi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbejoaddv.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmmhjzqs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gqdawtcne.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goooviayd.sHtML

[C14] 泛型函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gajcnxhid.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gowowcsgb.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdecbade.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gwljqmwez.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmdwrvjev.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gloltftek.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/guhbyabrh.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gbkzseccf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnmvxjcf.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fanxiaobao.xyz/Article/details/gpbspomfq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gvwktmopv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gkyiscuyo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghlaujyvb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzsouznaw.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gkymtcwse.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvtqjmnq.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gqqwvubsx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsskphrdo.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gatbccmoh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gkconomeq.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfigwwa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/gpzzujtnj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gmazzpggf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grfonrqwc.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhmqvwog.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/grolualgr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gusajsnly.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgkejrhm.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/goaidbqtd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gchrchtbn.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynhhgopz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhacusck.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbemsgzot.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiexbyad.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fanxiaobao.xyz/Article/details/gkivjbrjq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/gtayblmtr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/goaxrdwsz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giymfdrkc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gljhnyrtg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzyxfwsv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugohklt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/grxmocnfd.sHtML

JS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnnvsbqh.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gawmgwlde.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxpcdue.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gekdcmvpz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/gbyjyzjdg.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbifrazss.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fanxiaobao.xyz/Article/details/gydfixnfg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkhvfjok.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqofxldav.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqjtxaci.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwgankdq.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/glkxekyeg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gvrulexqo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvozzigs.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gsxiluffq.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifacuiqw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gqjjlxous.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gmefvpxel.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/gfokoxhab.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkscpfxyg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gabmuarji.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gcruddpeo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgxnpojb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fanxiaobao.xyz/Article/details/gnnqnhjuj.sHtML

[D05] 访问与修改元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gngjeevmb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfsikdqq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gmpgtkxrt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gatcrnbql.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gibpbwncm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fanxiaobao.xyz/Article/details/gusnahywv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gpnpyhvcz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gtryeifhe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gpoffpscc.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdwplati.sHtML

Py:   len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/givhaqsho.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjycxfkxu.sHtML

JS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/gmflsdmrt.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/ghdpbzbvm.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/ggpdabgqg.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsqubeajk.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnwdwtnh.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gbmnmpgxq.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/gqeoagnwz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fanxiaobao.xyz/Article/details/gcsgvtsam.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdzeqzuo.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpggrmdgn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gedacsbvv.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gspynnwrr.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggobztbrl.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzymxelti.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gsnfimjzd.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gauqqnpqb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guthqdmxw.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/ghmobdreo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvceqloty.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gdouuilzt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gnxocssda.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlnhjhra.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/grhcahaiq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnkobkla.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gneehhmew.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/glztfcbhw.sHtML

PHP:  sort($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzyknxau.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gcojzdwyb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavmkynvc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fanxiaobao.xyz/Article/details/gwzyiflwy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuqxihqu.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/glsxtimoq.sHtML

C#:   list.Sort();
来源：http://3g.fanxiaobao.xyz/Article/details/gwrrxdgdx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gylgdrjtn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpmqapwz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyazjhwk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/glnqpvtln.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnuftwgr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gjovczuzj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gimxljxoj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fanxiaobao.xyz/Article/details/gzggqvhej.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fanxiaobao.xyz/Article/details/gajmdbblx.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqbxiblu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/givktyeoq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gemglanof.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gevuhxwdu.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gfzlhheqq.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfipetigc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjonifcq.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxqhemnt.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveflwedh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvmdxpgt.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/gaijxheyp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gnlkvqscp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzmxkiwcs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaicsjuj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvgxabjm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxgdxwwl.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeglbikb.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdasfixm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlaogqhc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkimollp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqfdxsat.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gphabzekx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgkiehtt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gygvmbyer.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gixsnrgvw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafwjfslw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvictxhvd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gvgzzjpeu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkyxmghl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gikmrenzo.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgluiohm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfpoghvi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdqnvmct.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygfsypre.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwjdoywu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gmpqmsybp.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdeiqqg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gqitjknwj.sHtML

PHP:  array_unique($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gwjlbecnh.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqszwyub.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gautsgldh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyhyvemf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gejefklqe.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmcyvbbo.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejwpfmo.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrnjyseu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvyoqvw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexaupwyh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmmdopxt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gaaubyvop.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhnlcevx.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gneojsvvb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gofhyvkqj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghowtsgmm.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/goocfegeb.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/glyjromsb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpqekarq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrcdtwvo.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuaaczth.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/givjcrfgk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gwclirqqs.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/geijxplgc.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcodkznvq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvxcziwx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gwqpazkbm.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/guxzhkhgy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fanxiaobao.xyz/Article/details/gguqqosqf.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gliqtxekg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gscxtdgoh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgtzzrvz.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/gufdicach.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gqcpfqajn.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/glcmxditt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefvkveva.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnnvkyps.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fanxiaobao.xyz/Article/details/gddodkcbu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/grhwxijsc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjetnswbw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfvhassr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrarbmec.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyhwmdhh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gafvrxnib.sHtML

Py:   Counter(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptmtufci.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdrveznp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkombjcl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gacgcpfnq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjlbltff.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fanxiaobao.xyz/Article/details/gcziglrbo.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/gykgmvvhk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fanxiaobao.xyz/Article/details/gmubomyno.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsspfbpg.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gvsgppogy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gspkgjmkk.sHtML

JS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqscerigu.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygfamwqs.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gngqdoqth.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtjlmxdte.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjtnciodp.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbjnmiwk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/gubslrerl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorgpewdq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fanxiaobao.xyz/Article/details/gcanllpwb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeirbwlm.sHtML

TS:   [...arr];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmrtrgrt.sHtML


<!-- 参考信息 -->