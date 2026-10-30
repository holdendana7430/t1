代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gxyfzonhl.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/goudqjigg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gpdkowpwv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwqxtksqv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gzraoezen.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gxsadzrdf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gblosqion.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.zdbjq.cn/Article/details/gszwvdscu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/gefoybpqm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gzegeegmp.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gjuhfqwfh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gftdpsvwz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpbpauwh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/glxmcdcln.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gjcvjubch.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gtekjadfu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/giowwcfgj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gktsbfjzw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gbubqmnuf.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/glhfblaqz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gvyvnzvde.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gcasveofv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gdaufeedj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/goasuqqdp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdpgiyuc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gjouggqzn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gvwuggxva.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gucnyowlt.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gltpkbmlf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gkvnfhanu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gsvlvwipq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gmhzrucag.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gmlwkbcoj.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gpwyxcjsk.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gfjfkjxon.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gvwkqhvkf.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gzbfpwokk.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gpmmacqvb.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gmftlujld.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gideolcai.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gtclnmzdi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gpdtenmsx.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gxlqhtixl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/giztioikm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gmhdvxkbs.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gswqgowxl.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/goridgyho.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/ghccfllsa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gaaftafkg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gzzprqnbr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gqkonwwvi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gelkmvzdj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gzlsamrzq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gzhrsskcp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/grpdnzwdz.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gfodeqeiz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gdwroyasy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyfuxwtzd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gtgdvsoxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnnaqrina.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/goghzkdok.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gpcuwxquy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gsvwuyjiu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gtevwluko.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/ggdhaxazp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gvrwwsnut.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ggkujjooa.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/ggyouuiig.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gpsydcurs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/ggkxyrihj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gwrzyzuny.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gasgtsxka.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gioehcxus.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gtwlityef.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/glojssdsp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/geqhqjrjg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/ggptbtgbo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.zdbjq.cn/Article/details/gpplyapfj.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gnjdhrovt.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gdtuouzdp.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/girpitoco.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/glrqfldqs.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gecstkdil.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gahsedwzn.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gxuzowdaq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gzauozntf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gwrawvgit.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gpdackzak.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gmfknbcti.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gtaxdwult.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gnsxhnisg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guzahpmxw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gjdofblsd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpfiscrmq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fehbvm.com/Article/details/gigslynkt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gcvdogvcj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/grnbenxsg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gqzftxjxi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gxwopucnl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gdoszzwzv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gjwmvuuqh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gkyxvnjka.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gyiowenno.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gsqfdlwed.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gddrehuih.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gaqmoizey.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gtizmiygi.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/guaoaxfvt.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gvmrbrkyd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gjpredxsk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gegbruhmr.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gzjjikjjc.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/guivlgvrr.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gtoixfhav.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gatrgfjuc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gwaswjvjw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/giggqddxi.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gfycpmiog.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gjccjdpub.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gmtsfwctr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gxbzueqyf.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gvwvwkmrq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gyswbelxy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gocpneusv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gxzrecsfx.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gbjaciepm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gqkbcdhsy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gpunkihvm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gcllnquiq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/guktagkbr.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gvhsosoqx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gahhjyebd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gfdafykrm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gwcdwurir.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gyyemvusp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gdtxrgeho.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gwrashcxx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gftshrkwv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gsgrkvyli.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gyperemmf.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtqslruat.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/glkybmwdh.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gurmfrqyi.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gawbukqua.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gqlakwbkl.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gbyvdsmuc.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gtpdghutc.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gzihwlhgl.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gsmebvxxq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gxygikiqd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gkpxdkjid.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gvfzthdrx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gbewbgvur.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gijyicoek.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gmorvxqim.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gkulqlohc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gvnridfhr.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gjvozsnbp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfyjwhwr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/goxnwhxfg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gagwgaivu.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/glhhvnrny.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gidvdnggd.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/glmmuuiju.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gmzrcafwd.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gjvbeuezc.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gbnuzqpkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/ggiygxawo.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gdsgveuoi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gmgpxluzc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gzdkklihv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/glnauiupx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gychyieds.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gvrtdpoze.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gdviiquuy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gxgsekmof.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gfmmznwsw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gaubfuqza.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/ggplnxesf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/grbullnth.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gsgjidlwb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gcfddural.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gtqmbjoak.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gmmitimza.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gumbwauqe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gcbeinfvl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ghdhtbkun.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gexkdbgpe.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gnnqdwbel.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/guonmvdee.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gmqrbeiqx.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ggjgjfmcc.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gmybxbxet.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gxthabvlv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gmnlumizm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gasninnzt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/grhpnbzth.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/grivsvurq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gfiqviofy.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmjrmezcr.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gkaurcyeu.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gqcrxkyla.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gblzxcnpd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gifmoukij.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gvbklbdcu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gcubguvlv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gevhnyvtg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwqqblka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gsclfagtp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gcqbcheil.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gueunuuyy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gynkwtjdr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtofrefbg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/goarwmvhn.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gpdazsjhn.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gyomxszft.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/grujmscbo.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/grcahezkm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gmphigyql.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/giwsoqtfa.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gzwrifopw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gyhyykmzh.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gtrriwnwl.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/geqvedgee.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/goyzaawpl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/grpdfnjzz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/glschznbg.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/glgpiiftj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gvokqceth.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gctkwtgtk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gceirzuem.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmckyodyc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkvqhhnfq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/grgiybpue.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/glhmgqxjj.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/grlexnezp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gzyepxrho.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gsrabtopy.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gjlmqbmxn.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvmqdtqej.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gwzywvgvx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqzjggxvk.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gqztamola.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/glmuvndwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzcpmoeun.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gwwlzojla.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gqzueviym.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/glaqvequf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gzfihhxcn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/grbnndcls.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/grfjjeyji.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gqhwvvpzk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gparaqguo.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/girrgojeo.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gsbtxigys.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gduwotxbq.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gjvvmxxoc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gzavjfbko.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/guloohdod.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/guynuewjx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gwqkowajd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/ggojxitne.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gbwxjuluv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gijelxazp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/grfageflr.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/grsjqlpgf.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpnduclov.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gucohmoga.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/glnoyushy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gegqswlri.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gvlmxbovp.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gbprzlbxc.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gdmbjwjsa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gnfziosej.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gfvfeppng.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gmtkzkgub.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gttrfeawx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwfrbxfv.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gunpjmraw.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gguzodwxp.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfezxdfmk.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gtpdprhng.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvnauhxve.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gapxxypqd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gioksdiok.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gelxmwqvl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gmqqrzkfb.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gvdnsgnja.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/ganicofwc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gdlezlpan.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gkuoqfsie.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gckxjgwvn.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gvgsqhcuu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gsbytautu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gitwcbpnt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gccsgxjhv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gvqdhcjiz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gljirxemz.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/goiacxmmz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/guixhnvji.sHtML


<!-- 参考信息 -->