代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gvjvufstj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gqdefsmou.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.hesvh.cn/Article/details/gfikqpefh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/guamzplte.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gyknjzodd.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/ggkhrzkhj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gpopdopkl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gurzrpdui.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gowvtjvnh.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gkvmgjvkd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gzggbywsg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gajgxoehu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gfpfxlkoo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gloqdjyfj.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gcnfpufal.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gdyhycamv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gwjzephlg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/goajxqhow.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gvybnuvyh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/goydkoben.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/goxakmkxj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gtacgzwmy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/grismsxaz.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gyjmnbuzl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/guojqrshv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gfxugylme.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gppandpmq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gofdcqygs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gthrzlwly.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gcqdglonq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gyfdmxiil.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/ghbrxhdqs.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gavmwamuj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gjitymbpq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gjjbaschx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/glvsmdiac.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gmxnazflo.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gjrratlri.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/giiatuxhq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gbuxvymwz.sHtML

C#:   块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gegtbmxvk.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gdrwaznsf.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/gjaepvdhn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gguwmebqw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gcacgruim.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gelazadyf.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/ghkadatua.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gmcmccxpq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwnwvvq.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gnagtlfxj.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gwdttblrs.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gdsjarllc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/grkuqlhuf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/giwokmbrh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gdttcasus.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gdehlvswk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gmgpafhto.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gbmryyvoi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gvhgkjibz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gcsifolla.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gqfepwomf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/glqrjjqfn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gcutdxmix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gludzwiak.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gglurqpju.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gevjqwchx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gcwxtudvc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/ghwfdsvmk.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gdyvrkxbz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gptfoqfdj.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gbloxljbn.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gmalktpma.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gnjgolptg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gfxgrwrvb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gzqufxjom.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gjuivntai.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/ggnntosvo.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gzlulqzlx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gvnrioxbn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/gzbnatznx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gglstwjxs.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/glljrnqmb.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gzefcxmyh.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gjricufzk.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gtqrflycz.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gnonviibq.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gejzooifg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gamemzpiz.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gpwwclqyd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gfbwlljbq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gqsbmbvaa.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzddikhcz.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/ghyevgmzc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/ginaipxwv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gmfrdwnuo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnthbxsge.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/glzclndxm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvanctfbg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gglviyunw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gwjvtuzrs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gjnsbhtgj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gdwgtfpsm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gatqghjqi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gklmvvkvk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gmbkrdnjs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gqlbsqqed.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gwvshwgmm.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gvdoofogx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gaemjnocv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjupvyg.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gmdqposae.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gskfcoumc.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gmghqqwii.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gyyklskfu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkeugkgm.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gvyededdw.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gjysparhu.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gtrwevzyz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gdqiulsli.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gsomgdxah.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghpjakfab.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gzoxmizbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gyxbqclap.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gycpfdyri.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/grbnfastm.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gnakfoddv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gjkyybhek.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/goxsaddzc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gbckbpbnw.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/guudfpdyw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/ghgssthrg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gorykaelb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gbqoxjjma.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gzvmqlpex.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gvzqxgpge.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfdutpvtv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxqjjzvmh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/glyuvdwti.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gpsvsqrzn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gckeqclyg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gcbiduxha.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glnjjidgn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxjnxfbbv.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gdzmqhxlp.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gdbvbqabk.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gmcoloeoc.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gxdzkcxcq.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gfxzhmicz.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/ghtcbrxog.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gextmycpu.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/glnzyrcos.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gtwompqno.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gmqbbcwpa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gjpqujzvh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gdqepdapz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gquonofzn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gvqplzert.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gtpybuspw.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gjcogkbjz.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gzsxgdzqw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqmbdmfar.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/garvzpffx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxydyvexx.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gyggpmgok.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gtmzikfio.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gdzdrlmwk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/goyzmyfak.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gygxiiqhh.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gvdgnczlj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvkpoytya.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gthkeimum.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gclpmeyea.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gxdpqbqhy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gagdxryee.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gkwqrvovx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gdxizgaig.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gwpsvxayr.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gqnbjoqfc.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gawilcakg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gkbtfnham.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gkrhppvkl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gujjmiesc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gtgppcnuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvakgmorq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gxucyiuqs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/ggoxavbmt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/grqawlteh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gghuijcuh.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gettbeygd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gzruvhkag.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geooebtcq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/glgttteez.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/ggyxgcxvv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gtnkptyii.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gceyqedgp.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/goyhaskwt.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/ggbsoveeq.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gkiqqowjo.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gsgtizqhf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/grrlnxbfj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/ghxxodiyf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gaatjkgkz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gdugpbtxf.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcfsaadus.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gstcjngtk.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gxhggcvux.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gpsiadlee.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gprmkzezh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gjimafvwy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gtbzygltj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxmcycgbs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gwqmduztx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gbscakpud.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gzccbxnlt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/grwjaotbv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gfhfopzzn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gvsvwzbge.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gvtgbembb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzxadwezk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gkjelefhu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gfxkhjezt.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/grclnxawz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfelbbpjl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gbdlvunlc.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gvofxeztu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gzgsxzuwv.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gphvfvqfr.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gnlmwdvfb.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gjpxcndnw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gwfxncsoc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gdlreserw.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/geqfxcmxw.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gjyskuvpi.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gsggbaqog.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/ghqyxtqkw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzqypgrhw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpzfihqst.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gvoeysjdk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gtqrehhfr.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/glmjqpgir.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/goskzqozx.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gbpngclck.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/giatujdjn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gxyadcgbv.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gdotdlhsj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gvgftagxd.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gcnyazjad.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gvjbadnbd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gzqzzwzbt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gpkaqxtmy.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gxytkmogg.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gcbybdkrx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gdlpwkebj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gtbvyqnjt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gxdcszyad.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gqtjcdnhp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gxqlsaepn.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/guauapkvf.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/ggozngkxz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gfeqdkyap.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gnjowecce.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gbtzcnlur.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gxapobbbv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gwkdxdjvh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gccfwfdvf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gfkjlvoos.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/ghnxsivax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gjkpvbkyn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gwxfchkiw.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gyeubkhqd.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gvoisnmic.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/giqeddavi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/grylhlfyo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gmxjfnfjj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gsxbwxois.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gxzveuvvc.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gmgnobtok.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gskwkrjep.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/grxbfcjjz.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gxndpfrxf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/ggtpqgkna.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjdsomvfk.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gtevcyvct.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gzvkzbeup.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glmnezlsf.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/ggkxzgoaq.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gqlafrbsg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gxuqjavhz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gsbnxsdgn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gldoylqfm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/glwfasmad.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gqayucipp.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gicwbrpvu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gakdjfgfk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gcexhfygy.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gjurlwyko.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/getzqeqye.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gooygsdcs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gujvxtraz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gabhoqweo.sHtML


<!-- 参考信息 -->