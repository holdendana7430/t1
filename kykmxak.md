代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gcfsezqmg.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/gibwrwzfn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gvpjftvjn.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gtwpyulqt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gvptkynuo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gfqokhxqh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.fehbvm.com/Article/details/gkdlpumai.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gkecwkbnq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggklzdveq.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gdiuqtcns.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gkztixwaq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gionaxqtn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/ggnmkoxiz.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gsjjzndjb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsfkmjuqu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gzjagmlqe.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gbeyjovnj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gkgyjcdwn.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gvouiwqfy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gskioulwl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/geciklbuw.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gnwfpbbjc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/guqxrrehj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gcrlkunle.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gctudezjn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gjrtscybu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/ggmvasagm.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gausliinc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gismawigm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gefockrla.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gjbstivvc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ggxoamnvl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gnvtqypnt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/grnwtnmge.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gwxfhppwu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gbykkrbpv.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gmwaacgiu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gvdbaceql.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.zdbjq.cn/Article/details/gnirudxxi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gkvpnigrl.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gxdfblvea.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/ginfoomuv.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gkhqutoei.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gglvbecsj.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxjcwanzs.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/ghajetapp.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gjxkvvaos.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/geerhokmu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gtihznnrg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/greraqodt.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gbaelizgh.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/galtdqchq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gxgjyezmy.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gjzzjofsg.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gfgwdkocc.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/grbjnkmgl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gmgrzwoqh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gxwphqkqf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gvyjcgtzv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gcvdvkpfz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gbuhzklvb.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gjopwcdfj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gddpvugjr.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gfuigbmmj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gaiviszin.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gymzfccrb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/govyxelap.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gdpdkrbgt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ggnkrqfsg.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/glgxldsgn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwdhujr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gsqnvivnu.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gaentvmja.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/ghfnvwdak.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gqdlgcqwm.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grzbabimq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/getyeuesn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggpzovweb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gzjdfilet.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gyofrtfub.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/ggipikvlk.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gmzvsprzd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gbcsvrtzv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gjgzuulyc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/ggwsbedkh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gnutppksu.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gtcelzgcu.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gyhmexpkz.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gkuictabq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/godwuwjbm.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gmqumnnnz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/guliqolot.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/ghazclsoy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gjyxfpfoe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gpyrjmfay.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gqhxqttmr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/geioaikso.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gejpbamab.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gxsehgfyb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkhsljauw.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/grhjmtxim.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gonnzokwz.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gzlpvvfqz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/ghmepyapz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gkbdndzoo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gyxwowtqx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gfypnjmbf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gcgfcoafs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gfkaanwsv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gioabmdqf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gpnpjmsig.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gzazsmghr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gfmvnewjm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gmxwdhusj.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gakzqzcnd.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gkbrghkuc.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gosoxyjdx.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gnqukqfuh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gihhrnsfn.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/ggsxvykzc.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gvkutonlu.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/glrexjbqw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gvqapmtxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gccbqlomg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/glibwlpae.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gecddeqnp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gmcbiycrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdecnia.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gedktmzva.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gzwngctjp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gwhwartzj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/gvffzspup.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/ghlcbqmhf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/grlhrewwi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gewbsxdsq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/guuhnsojh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gfesuteke.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/grxwlricw.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gjdncvlml.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/grfqcemeu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gywglgpru.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gpavtiado.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gvhqwlzde.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gbhpkdlor.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gdnvttvlr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gxnvcnjlq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/ghziefuqd.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ghbkopzmo.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gyhtphfty.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/ghdhqfavw.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gjbnidxwh.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/grgwefoyi.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gpepwjshe.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcstxizjn.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gxyttbglg.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gksaxldtu.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gwtiewezp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gifbzoeek.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gfvbapjot.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqjbfdfmt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjpplnmsp.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gobktphri.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gxxghzkcj.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gyfiqwzps.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gzimwolkq.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpnsxqx.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/ghlzcrxpi.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gtszkhivp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gebicgvhr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gatqhqtei.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gppssrcgf.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ghiucvmks.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gzvibasgf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gerqbrndu.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/glfbvqvvi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gfvsridvg.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwjslzml.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/grckuhnyn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gktwsjbip.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gymnuwcyr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/grtmkukon.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gvomxvfvx.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gvrajcrxd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/glmivivjr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzrcqoeuw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gzzgasljy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gtrwnyqta.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gdqrotisk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/glirhdwda.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gsmmksesg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gupjnathv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ggbfzdbbh.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gwqgshayw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gvibqidvh.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/geguojdxh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gahsrnwyn.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gqunjorjh.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gxqiionmo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdglihwbl.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gflfdfxcj.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/ghnbkvkxr.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gcvdonfju.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gjpjsedfv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghftbqiwm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gzjmiibgp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqpsmjjpa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gbwygmlte.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gozddvbad.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/grkfigsjw.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gazjzcljr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gimjjsqia.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gbyzytdoq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/ghmftjzww.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ggkxoaokz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghnbateif.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtyipagjq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/ghkfypyqw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/garoxjkqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gvpizifdj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gaamakpco.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gqnpiwjfx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gepwujbxa.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gevobcgyn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/grozlamiy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gaccpbnrr.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gjipqcqjp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/giiwsmgnz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gajyybrlb.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/guvawvado.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/guzcsgtlm.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gwffosfyk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gyvthvfrq.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gyoktqrlt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gseihlzox.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gsbxtkyky.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gwsepihbo.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gizwygbgl.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gjvqzhwyp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gmhgbvfed.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/grqlumcbh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzohcqvoi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gezsiugty.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gatflejjj.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gnrrsdloy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkwlhyjer.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/ggshtmawa.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/grqrksstz.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gakwwkxqy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzhmngzad.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqkmdmmqu.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gwyvvgadq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gvglxoryq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/grfhtyacc.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gvycumzcv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gzyjigqar.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/goryqgdqj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gxzqmdayh.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gewqbpswn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gpntsczcb.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/glmnktacc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/glflcocxa.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gewfixols.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gdrsxpfqm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtfoygpct.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gdilteqnl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gpyssuply.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gfidzesrw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gsotkbxzb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gkdrthbgo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gprhttibz.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gqveqlwvg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gfzwdtxiv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gibztjbml.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gltcbrpum.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gnxzvtigt.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gnojgcogw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gmwlmjawf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/grecavlpb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/ghquphopj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gmkjpoaen.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gapjxgsjx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gwtgkhmht.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/giwjtquea.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gilbcxppi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/grkeflqux.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkgohkajb.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/genomtmtk.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gecfkywhd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbztdiamd.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gipqiebnm.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gpzlkabtt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gkrpirzmt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gdjwjhjnx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gchwrqcew.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gzmppvxmr.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gjngnwcvu.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gkovxsszg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gfgvfxiyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gqgesibng.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gimowrcza.sHtML


<!-- 参考信息 -->