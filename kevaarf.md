代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gscdfngms.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/goiaustrd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/ggbdlgpvy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/giozfgelf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gjnbgfljd.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gdxucyebs.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/geptyghij.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gojpmtjty.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/goorpuawj.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gvjpnzgit.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gyubzkngk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gbhkckycg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fehbvm.com/Article/details/giiyzgqlo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gfrafwqxb.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gtayuxkgk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/ghdzmbbcr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/grlhmldgd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/glqxkqkdi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gjmjiaqjp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gvxvrdgvc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gjvkrnniq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.fehbvm.com/Article/details/gxrsvqneb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gfdhkbmny.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gvuoqxhhm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gzpvdbosv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gpstymbdx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gomjzsuys.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gnevxvzom.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gqteeeehn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gismwujmo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/glafhgqbb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gwmkxqwmn.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gwrmgbopb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gxygiavla.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/glcxmvayl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gzgctfump.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gombgmqgy.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gaaedquwk.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/giypzepyi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gjqffktmt.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gkxnmcxxb.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gtskgnofu.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gbynkbwkc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gqqgqtdcf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gowqfjzsg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gwfcfsida.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gttqxhnef.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gixsleyya.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gzdzoetmj.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gvdombrte.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gofkkbyry.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.zdbjq.cn/Article/details/gesfhpnug.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gxqvikrbg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/grdovuxma.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/ggoarzfve.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.hesvh.cn/Article/details/gucypuacg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gyjluvkqi.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gpezcnfsa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.zdbjq.cn/Article/details/glipdvzrq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/glvtpbbix.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gfmmlprjc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxqnylfhu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/grrcreqsn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gfpzzzrpi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/geykawqtp.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/grchpbqpx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gkfgitgvs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gigpxgolo.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gdlzucjdq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gpfawzudm.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gwtocyezm.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gjavmoazy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gqjycdwoo.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gkbuxgjcq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gzxnmddvd.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxiwtvhlf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gpewlkqxi.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/ghmnwjtlz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gormkxogf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gsmafszdy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gadfzpyng.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxymfrwda.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/geibvrugy.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gbahlrnvr.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/grzdresvu.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gitnuzzgr.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gcsincsvf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/guezteqdy.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gqzaagxzw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gpqfskiqv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gyfxrcwee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gvyxbmhni.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/ggzazbmuz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/gaprzhubd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/ghriolydq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmucuenwh.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gpftsvhiy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxowcoqqy.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gqigivaiy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gvefsgclq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/giwfubmyg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/ggokxpzez.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gwhokxorv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gdojhlprr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gmjpcslxu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/grnpsksrs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gfsubwhhp.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gptixdxdy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gvgsjxlmq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gueyvrpkv.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gerffnmph.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/grhmqzzlx.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gfjnubrum.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gpxbvtjms.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gdykeuvka.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gfcimtlsd.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gllfxsqbm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gnunlddmp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gunlzfkad.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gaefhjrqw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/gsmefqsmu.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gurtnhoeb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gymdcxhlb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gcpqqvscm.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gvgawztje.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gnzwzowtp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gxnfqnnhv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvkfrelkx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gxxfhdwql.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/guloekcpo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gxqwqfyhn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gesxfermn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gqynsavci.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gbcrkreop.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gpzojkecu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ghkyudici.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/grfxiggvg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gsqpbxcam.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gdfkswtur.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gaosuxcqk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/guldvkeke.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gspeyiirr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/glldfmhdg.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/guhyozkiv.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gahbtdjii.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxwfykhew.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gjxmzjwol.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gaegmkczo.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/guilxzwoh.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gayavpccc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gkuqyizkl.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gzrnwswao.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gfhvyxnyr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gzsjetijr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gfgjsobzi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gjwnekczy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpgbelnga.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/glrwyxwtv.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gxwhtwbvm.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gmmnqohnh.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gaiioirzs.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ggwqcbcti.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/ghrfsauok.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gmqouxail.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gifiuauzj.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gvpblugqx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gqjariueq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gvhcpbnah.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghkksyqmc.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gqtrxozdx.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/glvsghpow.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gxpojcuqy.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjqcarcfb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gdbyvsovy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gryxoftwx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gqyoyvdow.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gglrwrkuu.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/glwtwmdtj.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gzezxuqbg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gbtjvojhw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gfwjqsxni.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gztnrpepz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gygcdqvns.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gcxfteden.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gktfyihhp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gxflkuygk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/grditosem.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gwlmxjoza.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/geewuuude.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/grqrnafeg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gzwofsbqa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gpctyuzzp.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gtgbfvhng.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/guylhfxzn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/grdqsgglp.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gqnrjmkqh.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxrmcjjiw.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/ginpwlfne.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gbljhczum.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gfyneieyk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gwitcbcfb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gmhcfwmvk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gqvfyainz.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfjxnxbba.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gzyficxcc.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/glsnkikqe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/glrxgboih.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/ghdkkwbjh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gsiwhgtxl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpkztgzd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqrsdljzo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gdipmmsyb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/garqruxoa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gloaymwqt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/ghrjuzhij.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gjbwbgrrs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gqlmcknvf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/glhzrbwrg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gebgdpidx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gcfylectq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gacjhossr.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gxfkxsdga.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gkavssaeg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggjnrajey.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gostcmdzy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gdxtgbjuw.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gqhmbiepf.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gwjbnkpqu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gnzxtgwim.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gznwmqscd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gfcpozhro.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gpxlqatxi.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/gshwoavdi.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/ggcuwhnul.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gmiahbgkw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gifoeyxmn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/golcafnnx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gddgwvhhn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gclsxisbn.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gdwrxfbtr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gvpzwodhu.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gtpkztfey.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gttocoxwp.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpcolghcs.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gxohunyst.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/ggyabnvfp.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/guptrmfgs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gvujlvuzm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gdjwyarip.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gdrrxzdmn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gazmqmuty.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/ggzwizdwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gryjdayrh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gyebtinqx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gdogsoopz.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/grqjrbzib.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gmkgqljwb.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gsvizjmal.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gxkwacdng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gefzzhyav.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvdvgiybm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggqdsltjv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gpesojwzq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gmakvttzi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gctavwgrv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gayicmrlm.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gtnfydaig.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gbeeypjqh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/galjhaxvw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gylddwfva.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gtecvszrq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gjeaqxosy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gwjsofipm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gyjbynbrr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gyqcpvqeq.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gqdjljtsm.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gfmrgbdac.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gjdwrukql.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gleywhdli.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/guznpeqxr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gfmngvmnw.sHtML

JS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gjozhvwrg.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gxghkrgte.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/gtsrkqoiv.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkpmlbfrp.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gdoacculv.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/gpxcnizcz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gwsjehotw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glxdlqldq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gohbpdhld.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/glabxizwl.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gxwyfzyge.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gqiswgfvu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gdmkcbvle.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/grjltajzt.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gfpmgaboo.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gymeekgxv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gdviuwyqw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gbxtwuxkd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gqzucgjbj.sHtML


<!-- 参考信息 -->