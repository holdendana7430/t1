代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/giaududkx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gxxfnumcz.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/grtzsikcw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gofczghsx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/ggcbmiwez.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gnixbqbqg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gxugxaloi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/ghjvbrghz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gfezhtyff.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.zdbjq.cn/Article/details/gyoygbvjj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gtgrxapkv.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gonvasnle.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/grdpmivzu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/govmaspvh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/ggnjauhab.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gnxvbqwsv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gzqjxwarl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/grvmwmlon.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gmacxeifq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gocorbzrm.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gqlffvvxo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/ghgnjxrmz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gsuhxkjoi.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/ggqaxybww.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/guavloywm.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/girupgaao.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gdyjksuqs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gzubbzayb.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gswuzlnqa.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gcqfyxlld.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gjneusbzn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/ghmglnjeo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/godpxghic.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gijbledsx.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gqhugswfq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gyssvojiq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gfyudodom.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gbwtsrlxy.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gynibfzhw.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gihecyjpr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gyzroplpm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gztinlrkg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gnvctiibp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpliqgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/givogqhqk.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gtzisteex.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gpcgcryqs.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/grjowckcp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gnabgmzms.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/ghtihbbva.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gnfoyoebg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/ghoaappuv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gfbenlxhp.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/glydpspjw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gjsirkcgo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gfhxkqpxk.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gkaadgema.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gioowsius.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/griocnhlr.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ghdkqoudu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gfojztczf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/grshrdaxo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gsthkaspq.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gwvzhodta.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gjiisbciv.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gjekdlueb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gjqlbfwqr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gtnkbxrta.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyrwchjck.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gvrmofhzk.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/ggetnzxlr.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gcdwmpmlv.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gzvnvukom.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gamkezeim.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gtdjtixcb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gouxoclll.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gpmxeoxuo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gmssyxazb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gzxczjxxj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gqwdriqgz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/govzazyav.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/grktxnqau.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gmlnvkzww.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glclvuyhs.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gnrutdgrp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcresgpna.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gqcqvzddb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gsoqjgxab.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gvxnestye.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gxklzxhwe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gtlimdsmt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gqlpkuvgy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gyjrtvtli.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gfnymcbui.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gngkilexu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/grknsvltz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/guzamtcop.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gzshftamz.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gthfcxfmw.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gprppfomg.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gtuxanghv.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gepegyomn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gewuwinxj.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gygoobqxq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gbofrcswk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/guwmhatcm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gfsrtmffn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gzjwlursd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gusmaguil.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnkciixqu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gkzddxmov.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/glsowxvig.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gsewvdxnf.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gcnldurvg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gcejfwjhv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gmeeluyzq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gymtgmeay.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gndjzslmt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gnspkzuvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/ghiixqubu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gagmleeso.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gzifojrcp.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gawuahowo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gnhtiioic.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gtjgdgvqt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdoxszemz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gjzpwrlot.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gzfjjrght.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/geuigntze.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/glzpxsrip.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gkiswflqe.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gilhohtwq.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grrsdyxwo.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/grrffavnp.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gwkgqhkiu.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gbhiwjijo.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/goskhoaip.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gyzbcvjos.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gltjpbfer.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gtvpponrs.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/ghwyrexdh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fehbvm.com/Article/details/gvhejmfyk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gqrrfneur.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gyaptbqrs.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gieeodxsu.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gjpnkvejp.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gwterfwzy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtnegynvw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gehizkuvh.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gnenzpmko.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gmadfnfej.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gjlevxyli.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gfzdzfcrf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gxzhckjqf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdzjfclvg.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gfqqrnscr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/glgcearbq.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gbskerhad.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gkygmfxzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjkidanzp.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gnnjumquq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gcjpfvknx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gucitvegs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/glxjjcjjo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gteqmwawb.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gweuuhlex.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/giraplrxs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/guklajlka.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gazfrpvqm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gqstvplev.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnydzrjww.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/grqszabwy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gvsrtfpmb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ghyzgggtq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gmcwtknkn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/ghjdxdxnz.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gfdqhrtks.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gpuuqdscv.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gzbjcqtsl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gdnlpkrow.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/guhzpyyaq.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gxrcljvrb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/ghnssxekn.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gdugbxigz.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gwdfdqoxw.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/ggkzfhmvq.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gviystmup.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gedypdalo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gsleiigzc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/giuhcbodt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gkkusvfee.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glldparxg.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqjlpkkdk.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gzlrwaupc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gmacjmbyi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gaekdyrne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gpnnfwtfc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gdillyycm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gyjorgceq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghozrnemh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gdekuggjf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gtzyzfrya.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gregflcfz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gqokrdmvu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gjtmgiqzb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gzqxxzwib.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gjaewhxun.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gmijsqurq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gthtslmce.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gscxzkqim.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/graidbdeg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzuxqricn.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gfdaabems.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvkvqoczu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gztznmtcx.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gmpoquxvo.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvxcyirma.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gyblnyjny.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gjanmamxn.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fehbvm.com/Article/details/gxkaqdqie.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/goyxpbbxy.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gqgqoqvuh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gjgtseiym.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gqmpvqnux.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gdgnfphuh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gzzljmvhs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gayflxrom.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/giozesbln.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gjxinxlle.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gappmeevf.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gvaegimqc.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gzptmhzrb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqwdkvgiv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gcibhcphu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geebngrca.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gudejnrlb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/grnkpagsi.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gpuxvcocx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/guntrcnjq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmrzuiy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gwxacedtm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gpdnksfwb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gatvhmyhi.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gvvazqsdg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gttgbbpps.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/ghoiowulc.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gxwanlrzl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/glgmqjbab.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gfmisvgrx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gtqrmiwfn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gmfkfdggb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gdqetslov.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gfzdydvbp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gafwoxjro.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/glqlsfccb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/gsyaskmqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gotnckhuo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gsjfydrno.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwfsycnwk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gkkinmnzx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gzqvxjgxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gysxmfugw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/gjkmnwxks.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gyvviyqdz.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gfabrnxhr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/guadzqczx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gvqabghty.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gyeaxcfhc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gabiwsieo.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gdqzjsagi.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gjqpgekdh.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gnoxrnfwx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnyaivydp.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gtdqgipky.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gqaxbupdk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/giyxhmvuv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcujlcnrr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gqoexirqy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gftlaceuy.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gtankznhe.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gljiiuczc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gnksnwvoj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/grmjygqlz.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gmvboriny.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gfxgsaekw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/glnnrlboz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/ghoowfbai.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gdaeabmak.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gumhciqep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gvtjqxfba.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gsduqaiam.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/glwlbygmi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gnqwkwbww.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gcnumhorg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gtnlvvdws.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gjvgfynuq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gutpvlcuh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gxsnpdkgb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gulokkwne.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gfxksoqbd.sHtML


<!-- 参考信息 -->