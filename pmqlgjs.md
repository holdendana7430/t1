代发 wailian999

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gypbyetzg.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/groxduvhc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/giqkfuhrw.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gekeyprcf.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gccakbskl.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gvveylinl.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/guuepogsc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gupgalvvf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gkeyfgrmh.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gfakedmuk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gpuqgssek.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gtgvmtrcn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gbuiwupxd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/grwrjtthu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/ghhupnoux.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gvaizecnr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gsdmgbzoy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/glwkenlxr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/gnfzefnxp.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gasdlphpy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gcztawpld.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gmuppxuyc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggxwyaldl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gasammxlw.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gjuybzzcr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gzssgzhcd.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gjrfrpwzw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gprcmciis.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gkyixgpqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtydazoix.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gwrfpyyqi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/guhngypbt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gokdamuxx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gybarwvpz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gwsnmvxjb.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gkyfciulq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gikfddath.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gwdhrjjzx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/geoofxduh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/ggwbdrkjn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gdfsdeffi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gzqkahoye.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gnxtfgarl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/grdyipepp.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gwqmnpptj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/guflscbyq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gteubetgj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gnnirutqo.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvdbmysqy.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gjoisaawd.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gmymktdjr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gyarugtge.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/giieuiyig.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gxjfzweyi.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gumcgvepu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/giuqzhopc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/goxqrqalr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/guazpanig.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/ghqsahpks.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gdubpluhu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/ghkboeauy.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gbrijivgb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gktsewyws.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gukvckdwc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gbtncscca.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gvixubjng.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gwrehuhaj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gsagnqejz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gydhznuqd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/gnasoqhpu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gtqslfjmp.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gkipzzqgp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gqudtfhzc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gbndxxmxp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gvklubvzy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzfqczphx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ggcezmmwb.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gxuivcejc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gqlhbbczt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/galchrbus.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gnynbtmkc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/geajsgrlp.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gqlwmxsbw.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggxwkbmcg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/guvyvartr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gmrldspxx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gqodarbbt.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gsbhoxyzu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gfwhlbbdn.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/guhkrelui.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gwmhiqotx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gmhagnjof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbaukrlor.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsypixjbp.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gpboesnym.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gyztqplrs.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gnwmapoiq.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gqldlelzj.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/guriydvkp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gcuzpmunp.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gmguarnxl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gdebcbija.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gvikmvdyo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/grnqbpjxj.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gpgbysyho.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gvyucwjsh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gycgqzlna.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkkinmhmr.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gjjmkecdm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvhmmdact.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gkvwvsuje.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gjpwrnrxq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gaiqzblej.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gijckipkv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gissfdzbv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gxhguwzvr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gaplhdgmi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/grqrstizv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gkqtelcaj.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gjnjotobf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gwscqbotb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gmlqveojn.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/ganesmmrq.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gltazhryo.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gisjiidty.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gxggbswfx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gwwaxoyfr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmbmcpk.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjheyxs.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gmdrbswmr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gqwrzaziw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gxqdgpktv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gunloiege.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/ghlokatbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gsnkpwgey.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gluqjtwwp.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/grpmvnpsm.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gmhaudmco.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gsiyzsals.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvwynojwa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gfzbuhlox.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gryheykzi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gnxmdldre.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gdkrzbeuk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkulxwwgx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gursyxhyl.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gsrapdztf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/ghjerpkwi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gqjlvaysq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gcswwajkh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/glcpqcvmd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/ghfelpcbn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gcjrmnoax.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gtxvzcxzg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gyzmpqtzk.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/ghtsnazic.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gvjtrntyt.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gzkfzznco.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkldwjymw.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gyiijxrcb.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gsgkhklnt.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzsiquyvo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gijiiwjrh.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gujthwomk.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gslyrjcxu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/grcxyhrni.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gkgvhssld.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gezmmhrqv.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ghbxxaqbg.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gaitufeha.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gmctzdnxp.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gngqggsvz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gcfcwasfi.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gmhjiqyak.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gldhgnfcl.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/grwhrauyg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gppvajalh.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gwldoviuu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbruwviva.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gcilzlwkv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gpppfadvd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwdcfbtat.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gwzekbsks.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gllksgnza.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjpunltgs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/grrrssgql.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/glzjoekbx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gchtyjjbi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gtheqmgtt.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gpuknqraw.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gpojtambe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gxhavmrhq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnttbrwgg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzkctouau.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gmvfanebk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gemtgejca.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gmvaowmld.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/ghygnztww.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gweabbazu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gyhqhgyzd.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gwwduojtw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/guypwnfuz.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gllqiabds.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/grqucrmci.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gtlmmztqw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyngjjuzl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gfnlpzysq.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gsjdtvfdg.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gdjrcxapj.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gtaseznud.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gdlcjvrbc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gapyefchl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmvcpwdln.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gwmbcbsif.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/ggtanzjna.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzcheuvfn.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gaciyyprp.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/ggydioeks.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/grwlchuht.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/glzsmiehq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gkcozurpg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gbnajjmep.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/glrpupxeu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gtkbfudgn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gffofsxmc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gsbrvmruj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gdmufynrj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/ghvahohet.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gwyfkcrgp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/grpwoawlb.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ggijuqbes.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhlgsdez.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gpteyvroi.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gmiudrfas.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/geykisnng.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/goewtzmja.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gvkvtrwox.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gfbkvrdej.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gibfacqve.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/giedqxvyb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzzyljtxy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gdyldzvcl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gqkkghaqc.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gbrzpdqkl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gagowpklt.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gilvhetce.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfzfngucc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvnlmewzh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/guuwetntb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gwlisftik.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gijwzzmqn.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/ggxxypdtn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/guoyhmsqj.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/goohafwrl.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gtepffqlg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gniaznfkq.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gexpzbepo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gopnvjgdh.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdjndhtyi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/grrkfgwvd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gmobmlajg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/giohzctbv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gosfozbdo.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gvlddukrh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gdhfiycsl.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gckjronce.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/guswavffc.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gnwaedkfs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gozlxuzek.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gcncunekk.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gvkwigmnd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpqnoezft.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gwizzhehi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gmssyaqgf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gowcrcymu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gvqjbivfa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gkceqaynk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/ggrebosat.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gsnrgiyhp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gaszbkwdt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gjurglvfz.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gemxworsp.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gzqbkholh.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gzjhxbgxu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gbxcswyeh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/grakhxhsj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gdewajqeq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gxtkjfkpl.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gnafvhmkp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/guzoksbpx.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gfcgpzvwh.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/glwyqkbga.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gwaelqtvf.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gshngzeij.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghwywbucx.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gwkxqxnxd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/guznyjkxs.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gteubnmdj.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gdbxpqzzv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gdebqnwbe.sHtML


<!-- 参考信息 -->