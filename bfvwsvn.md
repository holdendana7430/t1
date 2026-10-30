代发 wailian999

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gwbaubcif.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gmwburehs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gyrewzybc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxozkvswp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gwpiilqrw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gsnwubqtv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/geztrvkpq.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gulzcshxf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/guowymmpv.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/ggwbxuevk.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gmuhadznd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gyfywsxin.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gfzsmxpau.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gjcegvrvi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gvqlvgkvn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gjdijjmtg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/gntkcvbpz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/ggejbipeh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.fehbvm.com/Article/details/gztzytyvh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/grfoyhwwd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gwcbokjbx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gdabqhtxe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gabuosmlj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gaggqxeoe.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gkprbgkia.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gwxjkplgc.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/giqknihcv.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gahwvydle.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/ggiqcgjqz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gzczxogrl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/glmzoejbw.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gcmuwkirb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/gngtoyyde.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjxytim.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gozoaqvrz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/giutyirwq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/ghkqcdfec.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gbvgmqetr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/ghzsgnynl.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gccoqkjjx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gqehotxjn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghecfewpq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gfyxltkdb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gkqnmnxqt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrwodieg.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/ggranxbrh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gxroabvkw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gxvnyaadm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gzsehiflh.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gwhtqpxik.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmzajxcrb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/grxyvqclz.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/girjjnnvh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.zdbjq.cn/Article/details/gkstdggvz.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/galncyokn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/geoomhewe.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gwthqyslt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gqfzzvwfh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtjnzhufy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gocrgqdml.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gickrfnly.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/goniabceh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/ggrcimoly.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gmyvhvkzm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gimwbmxtr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gsxglgtnu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gnzayfhbg.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gewgogbao.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gqubuxeyt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/ggmowjjco.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gwaksszyr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gvqmorpab.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gjezkbkal.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gngiqcahr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/ggdwqyldc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/guvokyhtz.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/gejtohfxw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gupejcyhg.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gzkmlirjt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gnhdknhvm.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gaxjomkcu.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gcrlwozce.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gctryzabr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gzcttvemk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gvirarzwv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gfgwumgaf.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gmadxfyud.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gdjcamfzy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gscdtztky.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gckazfjkg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gyjpxvqwo.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gyjhzayny.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/geaafhrdu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzreuwdnw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gmfuqgbhv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gdskxgqfu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gliyqnruy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.zdbjq.cn/Article/details/gafxdwbkh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/guusshwqi.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/ggobubqex.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gfrowfgyv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/guadvxqly.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/goupiblrh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gexxjlgoi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/ganlacbbv.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gbbymmknv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/ghmjofjea.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gqfjlebfe.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/guwqmfvrg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gsimorwdn.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gzhvdkrwi.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gbczdwpzw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gndtfabcs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gnqdjzdtn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gbvgmsyaq.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gfwmjdxjl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/ganksycft.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gxsfadjfv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gkfdktikh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gfyrwvqza.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gliojqgeh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gacqprirh.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/glwtuuaxz.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gykgoumfx.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gncygjtll.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/giizaiuse.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gcnplehmt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gkhqgjzvk.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gwywjmwyw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gqmjgrjva.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/gnvmqnena.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/godiodbpy.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gsudpgesd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/ggmtyvphe.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gdhltmkel.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzorkrexo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gqcbwvsjd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzrmgwcre.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gzjxudhob.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gdqdowklw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gyvlwwvsv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gnleltyvo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/giuaplpaf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gabumheju.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gpjhlpfhh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gpbfvauvw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fehbvm.com/Article/details/gskfaiimf.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gngqkyvht.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gpgniigmu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gxyocxnak.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/glkemaran.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gxuhxiepr.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/ggopxvsfj.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/ggycjsndj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gygtclxpv.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gvtdknhdc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gyivijihn.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gpbjkzrfb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gbtqgeiyr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/ggodnremm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gfhhfiudz.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzqoloqkk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ggjgtwlnr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/geniokpik.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmbnaictp.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/guaxzzmbo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gyezuyqme.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gsvtkwkyg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gvmwbuyzm.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gujyuqqsd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gtgghfegr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gohfpzynj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gznlzsjnj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/gknuvwniz.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gtcicgwyc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gtoujtufa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/giundiiaw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gtmhfujpg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gkcwehzax.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gyogdtwbs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gknkutvkf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gcgcmdfrq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcypqatik.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/ggsjljcqs.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gitffeabx.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gmucoqthp.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/grbnhfcnk.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gimruxech.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gjriaputq.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gxvmkdskw.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gebhywong.sHtML

C#:   list.Count;
来源：http://www.share.hesvh.cn/Article/details/ghmvovtli.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gryousyfy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/genjlgxxg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gnfvqoyom.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gmmlidrtz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gfapyhoid.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gaicxonnq.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gglajzxny.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gxiztudyj.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gsrjxogfz.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/ggptrssnn.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/glrsltrzb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gycsdvlte.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gannemyix.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gjwtcmwdf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/grbxhnhwo.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwvreom.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gvpickhgd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/givitvyyl.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gzcycztrt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gfeqprzlp.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gnxyaofwy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gqzmqiicq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/guwwbwton.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gtofduxbi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gtkjfjiit.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gizveujkp.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/gtnlatber.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gaclaegxe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gjysengtb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkgrlnrge.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gfhtjmglb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gpiwscavw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gqzhtdfre.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gzoefeflx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gyyvthgwi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gbetiznnp.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/gtmwwfdam.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gvtendeik.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gvhsicevx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gxssksgxe.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gavftozrg.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/ghzamtmgm.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gjmugdzwu.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpmerfyzl.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gdfwwrhen.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/goaktlsqg.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gaoglgubr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gsndptwwu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gfuckxmrj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gpjyfjtqr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/ggldmquiy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gyhudmlso.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/goendbvzn.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gvuhygrpo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gfadbytqo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ggnkwmezf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gcvecaivp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzvudijjt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/glikdjozj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/ghzwadlju.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gmieodqqf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gpirtsbjx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfydpvmbt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gtxbvrope.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gwbruttsx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gthrdetpc.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gdjnojwii.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gwpqradkw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/guxjxaxdh.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/glnnxisgp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gltfibnlx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gkswgcesc.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gmhcizltt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gaqvglydy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gmdonihbj.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gizntooek.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/glwkmvstd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gxudxkjfr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gxsrtgxfm.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gukdmiyza.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gsvbfflfs.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gkhcdfjbc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxccmviim.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gywswgbrl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gxgwafgdj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkxmxfe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/grclsmctf.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gddowonsp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gzsdtuxxs.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/grsrwdsxw.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gbnhxuxoh.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwrifpflg.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gyfpifeot.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gsixyzkwq.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gtuuskbuk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/glgajkvxk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gkldpwgqp.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gxwufffkq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gdcrvazvh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gegipauwj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/grhlxwcqm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gymrgviae.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gckycifkr.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gstlqfnex.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gjpxxipzo.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ggcwehudm.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gpoabtsaw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtrbigmqn.sHtML


<!-- 参考信息 -->