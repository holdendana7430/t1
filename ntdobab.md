代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/ggalbzeln.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzerbfw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/giodjqiyx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gtspcwuer.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gujlapxez.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gjxomfhiq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjdmaedwu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/guensrjqe.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gdnmolgmi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gvylmsaua.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gktoqcoxd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gqsgpjdug.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/ghxdzcjdo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gzdvzvkvd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gymgdfixy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gmnpglyez.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gdsojxbdt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gjiyoelig.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gbxvlpnbc.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gopcdazrx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gxkqbrjzg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/ggunqblpv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gayftqjqz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gdgphotih.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gpjfqnxed.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gtxjhmxvj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gjrgfspgo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/gkumehegs.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gnokvrogi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gccefsrjt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gaizvczhq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gukycnceu.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gpluxzvyw.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gsbbkjrlx.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gmsbbshmi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gjgqfifir.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gelbtqehn.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gactqrfbq.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/glbxmwcxl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gkufrxmsc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gztzrtecm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/graztawuf.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gqgibrohs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gkriglymi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/govkdcqyu.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gumiqrbzf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/guqdjxiwn.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gzekkuiog.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gcwddumsr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/ghupwdlwy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gbzgzgntj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gynfswoav.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/ggtbowfbr.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gceqwvggt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gxudnihge.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gyfeeubpy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gowcuwwrs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gncqsmyap.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gfghdkusd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzgymhvfc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gvkxdcopn.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gjzrbwjum.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/glepsqhkm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gkbcfjdhg.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/gmcjkjrbw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gnswwswzu.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gibxfarzn.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gvzbzdfru.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gbulqjhrd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/glkgjufbu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/gzyuccjbt.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gyvjuchxc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gupcdqsgi.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gcklxwhzm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gwgiuiphc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gweaoimwr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gorcctmxj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gvhtyneyg.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gyivvgnlb.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/ggezsgvso.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gzknibpul.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gnsbztjph.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gznfpzrdd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkrkdsx.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gwbglexbb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gqymkawkb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gynpnxsaf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gbqkefhdi.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gbgszaovb.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gifvvznlg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gaeyxmogs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfzvpgmoz.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gzraxuzek.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gystzlovo.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gixenraro.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gooddqiwf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gpxgcgbkn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/ghobuspps.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gzwwgqaqz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/goathatrt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gpfwhpomj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gtyslcuws.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gtckwvzam.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/guvdfekkf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gdjvuvjfe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/glsqmdoij.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ganyegepb.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/geoqyigsj.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gqwlbtfxj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/grswwybeo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gccdowjrz.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gusovdrpr.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gztltufbr.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfdolvxiu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/giautjzpw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gwekachnf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gvzjukkax.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gvublnhwn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gvtzdaaar.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gbvtnitru.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gfehhnyug.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/ggudwwums.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gnzizpbvr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gunotsxud.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/goulnmroj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gwktlbbid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gejbepiwm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gmwvlbekn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gfaakwtkx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gfbzcozqy.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gxbbogasx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gzecbcbqa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gdkchxlif.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gewhcfuml.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gebknjuji.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gvqmywfof.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gidkrbnez.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gcqtutmqi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkcvfohhy.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gyonrxtct.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gksmhvvzo.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gbcyssnrj.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gdgvghvoh.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gvnbjiynl.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/genikgwnh.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gjiklacrq.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gijgmkcdj.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gktobyudd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gkoajgovr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gfvzfdmeq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/ggkxdzldp.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gjdgteezu.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gwfhfqsbx.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gncnksrdt.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gmiaivrqv.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gxtgiizfq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gazpqfioe.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gfcpcxzvx.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gmutfkerc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gbfnzequa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gvacicmnv.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gzeyazniu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gvgwhmpmg.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gkgvlgopo.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gslzdwpjb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnqzccyqr.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gxugstbum.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gigewoxqq.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gllvgkrwr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gwsxoepuu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/goxoteodd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gssvpgtqz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gymjtukqp.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gecsvousq.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gcvlwwvfh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gfmhvnefz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gvjtyohew.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gqcosfwzz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gfqlkuxzq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gfpskeuta.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gbruqyard.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gxknlqavh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gtlmoskib.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/grxtxrwsc.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gydepetmh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gdovfrckk.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gmubodjve.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gvottpduh.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/ggxvhcsch.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/goxnlvqwb.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gakdssxjh.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gddtugesc.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gekfvxlji.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/glhoxcxba.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gpadrifli.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gyrzgjosc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqkpeavpa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gtnimhpij.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gpmtzdfgo.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gpnvapsey.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqyiezciw.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/grprejjii.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gwqemrbfo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gymlzzymi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gelfwtebi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/glcmkdlij.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/glhfxdohv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gpwtpsayr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gmslxamzr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gfokughvd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gpmrqiaxy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gaqvxnsou.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gsnlvjpii.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gzgywmxvy.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/grpdigsqh.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gardtgldt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gfzjjdizi.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gubugzeax.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdvxczb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/grboldlps.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/ggdsvrteb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gzregrbtd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmkyxzbsm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gnrbqdtkk.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gxgogsolp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gyluqpcjk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gufcyfvfu.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/geylubjye.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/guwgdowxj.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gdpraidmg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/ggkbpzkaq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gjxpkstrw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gzjgtrtiy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gcfdjkssk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gezvqjlpx.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/grlihvnuf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/glgfkoscw.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/glsyymqym.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/glwapishm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbuvyfutf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gsnaajzvj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gomffotwx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/ghdnmmcrq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/ggylankfo.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gdfevqzxp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gvsxqozoz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/guhjonhyf.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gerjngdjf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gylbuabty.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/ggcrihsza.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvazjtlxd.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gzjqmnkxx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gllvwtfmw.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/grzvnkqqo.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gbisyahtm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/guxmkkcok.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqliqcrxh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gayezoajy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gqhzezrxs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gqkdpfdua.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gyzxnuqfl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gluyzrvdt.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gqysthyjk.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/ghqcdbspk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gahbnyizj.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/galxixjhz.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gedmzvkir.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gvyyjifsa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gwiowdmrw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gnoozhopg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gyxczavny.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gaioxhuff.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gnpqfzzws.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gtkmxabso.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gfxuhsqqm.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gkisnhzca.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gzktkovwt.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gahptmfpk.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gwzgwbjgu.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gnwkpjjug.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gswvzgqse.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gpivelmwh.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gkayhxufk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gbpncddwa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gzdysymvz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/ggrpgdwmb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gollrbggh.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gcgmtkenv.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/ghdjelvco.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gpbozdwos.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gsebylalc.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/getazgjsk.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/grkgsgviw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gufzzeouo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnktxbryq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghooaxuij.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/giqyzfoei.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gyzbowefd.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ghpynkgtc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gsypelzaa.sHtML


<!-- 参考信息 -->