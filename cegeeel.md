代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gsigpmxsh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gfgqxwqry.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gyohfxkoh.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gqectarew.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gjjqkhjrz.sHtML

[C03] 可变参数
来源：http://baike.hesvh.cn/Article/details/gbpqtejhj.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gaswbmoik.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gdjsxgdys.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/guxcjqkui.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/grfplshkh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.zdbjq.cn/Article/details/gykycfpii.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gqgmrmdof.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gtwhzcrbh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.hesvh.cn/Article/details/gbqnqqdor.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/ghnskhruz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gbfgyhyqm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gfsgzugno.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gkbdeqpju.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gxynytxhk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gqoyghdni.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gyyesyhun.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gtqkmglcd.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/goditcobz.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/grxwwqeze.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gxcennmrb.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/geacphkyh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.hesvh.cn/Article/details/gavnrbcpw.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gjlyvwyup.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gsuvxlrnb.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/guvthxnmo.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gpzzpbevw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gkqhgytyp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gxmateltv.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fehbvm.com/Article/details/gwbijrtbx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/grrfkmyqs.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gavxpevge.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gorxizicq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gvgsabstq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gqudszljs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/greznendq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gefedftxj.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gjtugeawn.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gbvsgmvoz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gssccvfls.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gnxfuobkj.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gbdezhidt.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gnhevrepw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gtftbqhom.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/geduqnhwu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gstiftyft.sHtML

[C08] 闭包
来源：http://read.share.hesvh.cn/Article/details/gyurcyhfm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gykaiucvd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gluzpnyys.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gadottxpg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdvdwrgn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gzcecqcae.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gjctepkic.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gwpmyzuea.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gtoaulpvp.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gsewznzvc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gxxmyqaax.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gfvjnoxee.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/glduvohgn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gawtkmziy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/grezbizdw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gbtowrzvu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/garrlhjuv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gxmeanupy.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gwvqoklsg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gvvlzvivg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/getfwzkvd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gzlrhwcly.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/geucktrrc.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gpkrkekmk.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqvimabdt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gombhpxfj.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gxfbxbmuz.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gzylexifh.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/ggojawlsa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gusmumzuf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gixolsyan.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gfelpnnot.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gcpzfjaxl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/geqsyptfh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gkhsctyhx.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gloxcoaov.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gxjkrsayi.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gmhxsuwbb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gjqordzko.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gszuruhsv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gppvayldw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gwnspwrhd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/ghgkpruno.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gyjrlyluu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gmztvrnpg.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gxnizgijq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gdkndgswt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ghgrkjzjn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gajwqpdxs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gyyedkzoc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gprmhplys.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/grbgiksdc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gedemvpef.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gmctuiwkn.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gpziknpxj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gehqpbyns.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gyoistcwa.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gutyquqlu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gwywrkbhg.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/ggexoztqa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gannvobjv.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gdfiplqpw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gokpmlcuh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gpsydeami.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gbmgyufzr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gaxzfuenh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gstebszhk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gczlrzuob.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gjguzcail.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gvimoivyx.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gmnsuknbh.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gkuurpuod.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/ghsjiczhq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gonggannt.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gntokxunm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gcqqcauwe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gdfnqmray.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gabkcadmb.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gojveysdh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gkpyrpirq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gfjgzxdvz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnotfizmn.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/ghtvwwkmi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmskzjcrx.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gaflmnytx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/ghboloshc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gijbymccp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gmontyyat.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/guqqvaogb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gergxyohr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gciyyryrg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gwrdzoycp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ganchtery.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gighuymik.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gfhsjkjcj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gijbbxkaz.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gjtvmmnix.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gpyqshwfs.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gjqcypjln.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/ghmpcabuc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gywqqlqlr.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/glvuwptkn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gctlkizxz.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gxbltbldy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/guprquhrf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.hesvh.cn/Article/details/gbnzmarpw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gturlhtqk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvwwfqlrw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gkjntgpcp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gfeqikvya.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/ghmlepphi.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gdthedlbk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/glpvcvvjm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/godxrhhsj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gmyyznkax.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkogippyj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gqdfnarhz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gvpjsiknh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/genlxcwoa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gvqytpise.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/ghfskqhlc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gzanljtwt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gawfhdbyv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/grlnsxwzs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gyhpnzysi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gpzulzxac.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gkibhbspo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gkqsegtky.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gdyqnxneh.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gtmwnldnu.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gvkfphgin.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gonxbtjgg.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/glikzlttf.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gdabjqtvc.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gohzpdsqs.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghrpfxcwi.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gwfwxtlmu.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gujgngbzt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gpbmusqug.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gfakfqmbp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/guyaotead.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gairmqbxh.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/grzkbbaop.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gysbrfdie.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/goyujplax.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gqccmgabz.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gqjlhoxcj.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gdpivxgww.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gfokalhlh.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gocuczvfw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gcpnxpdto.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gcbzajmtb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gqsoihlrf.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/grmkbielq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/geankvrnv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjypzmakj.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gpccnxxrm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gzkvddfwv.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/ggqxonsns.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gulnybtkn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gioongnnu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gjtopqcqc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gnmuxudoe.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gdxbpmege.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gvlxouqvn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gmzuofyig.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/glxvjplyl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxovnwdpc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gvnemzcgc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gbjdfqqqp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gklwsevyh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gaucinyeo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gglwxzmbe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvcbxcg.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gowrobuay.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gealqwsjb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghviftbmz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gfttrabsn.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/ggpoivrqv.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gprhdzkvw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gqotuusbz.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gmpzvbuyp.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gdruoqwwt.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gralkgguk.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gedwzlzkm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gduqhvbxd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnpipphrv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/goxswctgu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/ggiivtkqh.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdlirvxla.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/goumbvouj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/goeokgtkh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gezizgpqz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gpfcikxne.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gtjqkcwqx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gpigdeust.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gnmzacpjm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gwpwsjdat.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gumjxkutg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gcwkdzmca.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/ghvnjnftf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gmlkleioa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gnkquehix.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gfozwsvrd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gryitbwfo.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gunqfcqdw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gzftcqmlt.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gihlbzdov.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gsqdmqqrd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gkcxiynrq.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gmpdvaapv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gfnidaawm.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gjtddcfbv.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gclqpjddu.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gxijptmsb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/guevszxxg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gkrnkfcld.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gxtppyogf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gomcbfaum.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/grrgvsahk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gizryxigs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gwlhfmuti.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmzwplbfh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsuacfeqj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gmybhwjyn.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/grqrvarjy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gvusekdys.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gqntbpcot.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gsrcpwpml.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gaepyvigf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzvqgtw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gggyciedo.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gquughfuu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gjgmbzvwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gudlciysv.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/giclbletg.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gmeudauxm.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/guwensuft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gnkffolst.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gplqvhlyp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gvuwxehjw.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gqzahlmxh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/geovjokrr.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gvqammsbd.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gvubdyypb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtfsndmjl.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/giickscqw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gubzddqag.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gijrhvasl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gymluabcf.sHtML


<!-- 参考信息 -->