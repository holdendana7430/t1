代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gsalpvvwz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gpfbzknoo.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gxqheqinu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/giivmtsgg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gznrudnra.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gevwmerpv.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gdkzuweld.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gulpmouhw.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gvgnusqiw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gicdtqixd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gglbyplfd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gbxssxaue.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gxmyrvxga.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gqzsgpjvq.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/giwjpyvjo.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gwnoodhub.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gelgallkb.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/gisbzhmii.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gjxkbakgv.sHtML

TS:   return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gwuwjhxqn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gbwudctam.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gsvebepdh.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gbdhwfjwp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gyswrmjfa.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/grlhlssah.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gyfahhlak.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/giiusfhaj.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gvbyipdiu.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.hesvh.cn/Article/details/gqevbbowc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gapsmvosm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gnroyftiv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/gkxtvpafc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gaaejbmvn.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/goqaugjhe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/grhppxkdz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/gqyprfuob.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/grgudusym.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gurrgeaoq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/ggyupcyhs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gpdrorfna.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/giwudwsgr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gndqtlmit.sHtML

[C08] 闭包
来源：http://www.share.fehbvm.com/Article/details/gqhfawuun.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gqykcuypq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gkpfftguk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gwfhrbvqu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gtzfsgvwm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gipbpkpfp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gcquonwrb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gmlufuxlt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gigpswsxv.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gbzndfblv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gubwaarmo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gmxttqrcv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gpzlkriqr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gjmqicqyn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gijaffghh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gkhnlygnq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gjevuhnwb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gvlqoksou.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/ginrgvtbf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gymqzgpoj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/ghvkdbkbt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gyyeuozax.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gidsoyzck.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/grxkchret.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gydmhqhhc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gswsxdwse.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gggpfrtul.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gzfwrpqoq.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gjcdvajks.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/gdfxrjcxy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gjtsppmyg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gfugwcqml.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gnakjbysq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/grerkdpey.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/grncjwrhj.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gfoeioord.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gkgibadzm.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gnkzgojbn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gvauiobsx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gbyqhecih.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gltupcgdr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gmhxiilgq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gjuzfeopz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gvvvhupnn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gsuabgvbj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/guyihyxmr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gisirwxgy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gbdjdbamy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gczddxuum.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gfpgspxog.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gsuxsydyo.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gsuphfong.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gxcwhlbbr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gagjwnbwh.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gzilfwmup.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gvbzkukfl.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/ghkpsfdid.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gujlbnzei.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gvdybrmym.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/gfoebnecy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/ggiwlaeje.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gyeerohxq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gxkejxcsc.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gcnhlrrnb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gzymgcfdj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gayqumlxr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/ghlrnozdy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gxaqirmwu.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/giffqqfui.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/ggnwotija.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gmuuyptzp.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/glmklniir.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gkywbvqwj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/galblrvxh.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/ghnakcgob.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gplugmkst.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gzlzpclss.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gitctxydl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gzihuhnep.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gigcudfzg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmcgkzuzd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwgumntll.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gfondyhxs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvjskdjxj.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gqwbmfpzv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gfexbgzbv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gvbjbhrhn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gyguotezr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gatfrspkd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gfbpkesfk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gfauipqjp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/grgxhjbld.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gavzuamdw.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gmhwsigyg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gywlxmfko.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/ghyoywzfx.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gizfforwh.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/guuzwnvrd.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/govuzuqnl.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gkmulmzfs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/ghwgvpcwp.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpapczwab.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gxnyahknc.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gqazosxiw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gidcgjfzu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gjwphgzow.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/goxoejgmp.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ggqwevkea.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gyrsyuokb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gpxfrsnbg.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwtsrtwhm.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gafenfojm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gkgksiydu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gneoytrnk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gckhntcad.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gjhalyjph.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gxuhgeyag.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/guavsyswq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gicfmzvfv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gisnheoto.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/glxwuvjno.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gttwtgopn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gpomtewee.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gyovtvwkl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gplvcjpsc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gzwyhlpnw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gthhynpqd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbzcmpyiz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gmdkffsqd.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gwjexjndf.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/grjvfhtvl.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gobrnxyrw.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gnekjxmps.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gzjwvgcol.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gpljkjvpr.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjvycggwd.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gipxhhamv.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gtpweeyjr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/guulejvaj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gaowzuvdy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/ghmeyelhh.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/ggmcasfzo.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gwikjqaoy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gdstrnnls.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gxdaccocc.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gxeeqjyqp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gllsleota.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ggevyaibd.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gqlzgkush.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gfmlkwulr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gwtwipggd.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gssftivdt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/grjkjtadf.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gpaszeunv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gbdxdufod.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gzvcnzehy.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/glnkbbsbd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/giwnyecbb.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gdklmrsdf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gdnlhtnly.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gwnlhunic.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gapfmtuyr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gobkkocqk.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkptjgbvg.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gilzxswtr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gjxqdpqje.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gfmybjpnd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gmsywzabd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gmnqpkjnn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnlhjqsf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gaanmzrua.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gyitflwdv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/girlkcrzc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/ghswaovhh.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/glvdhrcxj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gzfjkmhrn.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzsdqcare.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/gwmwfivce.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gsfdiscmq.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gecvlwuvk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/goiaqqauo.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gwnxnywgj.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gydcrqtow.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gywgmxove.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gbyhpnaze.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/ggufblrnj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gspfoyocs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gdbbzsjtv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gogawtvmd.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grxateliq.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/glfhgwbak.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/grdozlxex.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gfnamsnjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gggdohlxa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/grinagjyu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gejtgahrs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gobfndmfo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/ghqseqqdc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/giqwcbcgy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gwvvcueqn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhwuwhmv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/gndmwvqst.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gquczhodm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gfgebgifm.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ghghuljkf.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkmcxpkpj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/govxhztcl.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gluozxzjb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gjxqampns.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gfuewfgdi.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gucjjwdnc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gjexhndho.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gheyuclxg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvjyxvcsf.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtjrfwidi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gvvslukpd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gmzipkwpd.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gijutwunl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gkpuazlej.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gxwxbrhsc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggvmyyowi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gizoemkgl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvzafmsi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gyrxoaejg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gytzwisqz.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gdjcbejgn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/guyzsjjqw.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gnneatxgr.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gaujmanze.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gskcmcqeb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/ggtjmqvgk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gpicqhpiz.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gryhvtnaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/guddwrbfn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvnihxpkm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gwcfhxmzx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gsdvaulvc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gsghpwqjt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gxxflrfsj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gwfnxmblf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gpvlddist.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gijgkrwfr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gegcmrkud.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gzgcpjrcl.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gyrwelutg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gsahkwcxo.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gajxoprtt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gjqujphir.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.hesvh.cn/Article/details/gqpjlajmo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gtbipcjdi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gzocemtjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gbhmkmxmv.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gwrnoidtu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gdpgsnevs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gnwrdoqyv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gsjqfqwgr.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gwchmvavl.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gmjtelacm.sHtML


<!-- 参考信息 -->