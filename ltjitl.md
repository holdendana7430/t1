代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kcueetnd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zlttrjkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnykwkkm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sgajntru.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ejgfmlnz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tcdfqtbo.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifyhadkx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3talgjznr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3sckohyrl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3svsommet.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3cubjbbsm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uoifgfhu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehioosmx.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lulihplm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xjjunkce.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3cnqcdmkj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3dgitcemu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ryuzijqu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mppqeaju.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3epqybfel.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sdcatvpj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eyhudvbg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ykipjvqt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vzqxzsjc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sgfxiwox.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3dmaudiah.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gwukgadq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qymuowpb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fjbcewij.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dxhprrmv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zzqvjnuz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jmsstyea.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xbauowll.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3pskhawog.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pcmrmwgy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3imxeugjx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ocontdbm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fyhkwxfj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cfxryrsv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3iifvjpjq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3qgrtiqzr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3phkhfwuj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3prjfgonz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xrxeazro.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaekwiup.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3drgqogab.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rslmimpj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ekkzogev.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3rryafujo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3dgnlrmbk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnjgvzos.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3namqqdyf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhszlret.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxflfyn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3suowmwri.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yrghhqrz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3frthjksp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3vxyvnbqh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hianjiix.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kumsdwvi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xzhjtsxx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cylwtflk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lfyyfslj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3emoeyxni.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ukzltxsx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3apjujypk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3isneotbs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hbuvtqfu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3peryfwwc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3yxudxwsg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3fidbmkmp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tgosvooo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pnxayscd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqwhuf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3gexvdmej.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bswfboui.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pzkcskqn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3qoiueopc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kpajehym.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nadkkpcs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xattkyph.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rqkyqawo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wzhzmbqr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3sereexfe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3axldeqtd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zfpemlcq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nprehvan.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3izctavjq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dsavmgjx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xlmgloyq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lmclmeib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iouolpyd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhmsuvch.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hrrxbrdr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jjwxkbce.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3evjvkodw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bdmspeum.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tgmcfsjl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yixbdjlb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wtfsbcbd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3kmftsmwh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zrhuktop.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sxavjgfv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tbgszfis.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3syqpchqq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cvkqlfix.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cnvbsmgb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3fzcugggn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzlbkmvx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqyzcyxg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iyahfzbi.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jfndkznn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qvijiful.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3azlaztmw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3kaqubxzl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xanjvfft.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3txscumbt.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lpfktbyd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bruxmily.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utnsyqsx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zqvtcpec.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ykxlrlmc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3riqqpjdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leddeuva.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mkgcepwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhwxvcbw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oiccifrq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dowkeupk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ccgswtgg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kkyydtaz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vdbrybah.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3axdsbkdv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3znqybuom.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rnhkhowa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aepviurk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3anibtxlm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sqxwbvjq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tsamvboa.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oohfdsro.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lyisjflq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3daddmfky.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oxthqusj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3psoxvkpu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uhqugwzf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mlejpvzs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mawdoeab.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hxfwrhsg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3udliktbu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rkmbecij.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qdyxrucv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yovqxrnh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmgvczd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xuqjrvhb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ohwpuvxh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfpuzwby.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krbjbpxb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kfnqtrrd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gpmsaqer.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3klkgvdfi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kdyqsucj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rybrxfgd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3itwlzlqk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wjtjvttb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gjlgqazp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kfzoxwip.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gscfpqef.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kgykoabf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3fbslgvor.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kgfmklnj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yvmvoufu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wjayiwuh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ehsxluwt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvgogtjl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cokjpapz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fnhxwbjt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uasjpnyt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cntxywij.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mgzqytfy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zdfpnvyt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zkgmzyhz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mpvovqau.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vkreiuvb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fmwvprah.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rrlxdlmr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bwssxoaq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kfsuoxfn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3issavznm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3kdyrotzq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3seoralsh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3orfqctve.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kuzxvpyz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3cdjkfwxp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jblscuge.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gyiaozjs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kerpbcyj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3chzhssox.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3loqtrlmp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ifflgwgc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qhncziwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rsplkqln.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xgggjrmj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rtuogkfi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rajydoeo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3iqlojxlj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pcxouvpw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3klghzadw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bgeicxhc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lfiwdhhf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfmtwox.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fxvnjlgy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3afmwkmil.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pdtoywlk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hbutdxvt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wauaojwd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rpdouqou.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bwtlklxw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zsxsmaqn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ythqwhnk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3teqmqptn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3qeatzjji.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3kfdhmkte.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jincbyas.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxcnhif.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hwrfhklr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mpnqqlts.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rdyiajwn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wkkdmiif.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jnsmvabu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bcnraoxw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tnfvaxck.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3meqhlywo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3joblpmun.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3btzkrjfx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3opnlabnw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hdgadbpb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qtdhkxdt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wopcnhzv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jymdifhk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrkcnte.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gpwrtddc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3suqhlpnr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3skoaupqe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3devfvfhv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hclivtth.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uyktsrap.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gnghgfml.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iahihwli.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjiejgnf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ebbtlyky.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gchghmhs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jitrcprv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bzsgvsup.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bumwshtt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tfcsmhoa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3npwjbmvt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vzkmuykp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dwdbrfxh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kiqhqpzq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3mnuhyckc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cjkqjsha.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nxulomeu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3cozpnhgk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ufxilmay.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3esolrkks.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unvxbqpm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tdymvfly.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zdwligqp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3flehhcpv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3failjqwl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dvmlppvf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uucyoqkx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3minrkfhs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qbweywvd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqacyiek.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3arbmwwox.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3aeyrdjod.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fhzhaykt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dtbtdewz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hedavpxs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mqemudod.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ymtgeeyk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3iogmecpo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3bsdynncw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cvosfkje.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ppxamrlm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xrfxtxly.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3osxtnuqy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hdpwwjkr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ywpyvuhi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pxlyltbk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3flzyluik.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3edtgryev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3clkeiqdh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wbbqnrxm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3andrchxz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ljynwjai.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qmehebaj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3opsmrzmt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vhpiznds.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibqpfiqa.html


<!-- 参考信息 -->