代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gbvfjiftd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gcuulmlmn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggkpmwzjd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gabqcuvjp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gisvaypzn.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gfdfwumnz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gutcjridq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gupsnyzuy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fehbvm.com/Article/details/gppgotrpa.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gwwjpcfek.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gdplfthpq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gthqfkwow.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gooskicrm.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gxjazklie.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gdcdnzsms.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/ghrdrzrnq.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gsrtbiuli.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gugkqbjgq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gioseszjm.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/govqxblmy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fehbvm.com/Article/details/gshinthgx.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gjyebmznn.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gjgnxgzwb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.hesvh.cn/Article/details/gseevttoi.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gsxzzwfma.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gwfsrnhvb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gxxeafdyg.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/gntjcnxwp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gnuyndulg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gmglwkdzg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gwntznbln.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/grjslryqk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gcvjbgdpc.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gnfhefcmv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gqjnvtpfw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gkyuvcvxl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gnperkawb.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gqwmcedoz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/giydbgesg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gguxgbkqu.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/guysokwev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.hesvh.cn/Article/details/gcyxkamzf.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gmfgqntrj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gldsoxuef.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/goxblhjgl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gniwjnlkn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbsxasrh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gomuznnii.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gbdumzggm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/getktbvlo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gyojqwtsk.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gqxvwegko.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gysuhgdae.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtudyeswt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gdhibqqsw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gophossmg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gzrmiydoe.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gjpuprrua.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gqzlkjfdo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/gcdneriqv.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gzbqftfbm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gsnzshmza.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/glccfhxhm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gdcgkstxg.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gycaobxdc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gawsrsvxe.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbrhwuizz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gjssmxvgi.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/grktmfkxi.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gfouxlkge.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gmbdboofa.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gjakhtmpf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gzgiiubrn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gtnhzadsx.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gcgyevfju.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/glggvtsbi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gpeeagklm.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gqmmyemdc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gwibkjxft.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gokrldpfj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/gkqhbpiho.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gkzhspmlo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gmgmzzrqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gyvxelnal.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gaqbecoyg.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/ggosfvobc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gtykoqvrw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gmnzmaubp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gbitlwqdu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/glceqrmel.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gfkczksva.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gkbsaztat.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gteabnzcl.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gnbqruclz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gbwzckrsx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/ghsjmtuth.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gllckuoxw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.zdbjq.cn/Article/details/gpmfscikh.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/glfbhbfcn.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gxatohtlk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gtspjquvb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gmsfetwzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gzsfeidhu.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gwpzlkesz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/geqpntxtr.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gafmterta.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gfjedphio.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gukttsvnx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gocxplvpp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gtaqjppan.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gsmmwmvzd.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/goxtsqvna.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/grlvoklkv.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gbguolevv.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gmgrfnlmf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.zdbjq.cn/Article/details/gjmiirphm.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gbwaliivc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gauuljlhn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gxzjmocca.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfxmilvfs.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gwoqcytyq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gbomzaoyr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gmsqqnpbp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggsrhbrgq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gyblotxhq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geabvptet.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gdztcnxtd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gotcizctl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gwmdjbwdo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/glbubklnb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gkkupxvhb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gojwxdmin.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgvjcfi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/gspknvkxd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gpfdbpxrz.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gzkepjwdm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gkbhkrjnh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gsxqjlohj.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gspkdhnih.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gmavtnvgk.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/glzovbqvl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gqzcfreuv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gzpandggt.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gjbbuydqd.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/glwxftgfq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gpcsshhhz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gkmnkwels.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/guppmhoxe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/guisrhfnr.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/guaptnukt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gungfncjz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/ggcumchqw.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gqloklwde.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gmipxuuwt.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gcnalirwy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gzlifcuax.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/geraedjfy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gfoyhdwkx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/giqvbbtkw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gxzfgjpxs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmstwua.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gwqwriujh.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gpxwieikb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ghdbkgodb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gntluszta.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/glpqxuzps.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gioqfcseh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gsmtjvrca.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gksznhhjo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gldaequot.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gwsqkwvty.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/glmfpamoz.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gklljmema.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gojoxkyib.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gdrwmcixo.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/giouasjxc.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/grtbqaows.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/ggbxwwhqh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/golwdqxha.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gwuburitf.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gwroxphge.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gzczceobr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gucslptoi.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gqsrgfpbi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/glyiqrchf.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gnbqzelth.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/glinexdvy.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gasrjrrxe.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxbdtadwb.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gfxlrvxet.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/guxrnrojw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gadhqbnij.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gnbcnfdly.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gfvwnvrux.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghcurryvi.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/grwoxbsyn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gwsaadmed.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/givzvkxbf.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gsioxobzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gsgoyurne.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzkrjqoqt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gtuuvsqrx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/glxpmyvlu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/glljpbqdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gajalbrdg.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/giakhyqqq.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/glfbowdxt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gsxaajfex.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gpwwhgchd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gvmurrayb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gkozqaubs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gvsklgboe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gtgaiiada.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gevriyasv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gquzblkdk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gpxixmbzz.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/glbldfdso.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gztwjpwxf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gkenbuvbz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gucrhoodz.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gqjxntjpr.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gzculymkj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gbgwkyybe.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gmovbaqex.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/ggjsbzlze.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/giwltilvi.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gzmvlowdv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/ghayvmjvx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gucxsgvqk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/goqaelmjf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/ghjmbkqjm.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpuwpeoqy.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gvltcjndb.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gpbnwukvg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gifwenjay.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gzfdwrbxk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/giziejjxi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ghbtuaych.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/glaxdcanh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvrybdkyy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gcyokcyhe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/geyvcesgt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gwesyklck.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gecteroga.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gmloiihcz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gougwgxjz.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/guuvdpkew.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gqzjlkvjz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gmswwglvi.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gfsmksvfe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gugsccytu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gmjiocwbc.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbsamgeht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gxglqtdls.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/geeukcbky.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gizgxevpb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gxcpmgflb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gkfsfqamd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gokeixhiq.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gcoxflcso.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gpvruulje.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gkixpigpo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gszjqndbe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gcfdrwjar.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ggbfvswen.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmlkpsrfv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/glttqpylx.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gxuspxfev.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gaecuokym.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gcbpkaevl.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gjpnqwpdq.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/glfrgpvfc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gtbzhsaso.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gscrmxedm.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gmirebiob.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/grakcehne.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gnvzicdqj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/ggwiytxoe.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/glbooohgs.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gvhvqzmuy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gjzckyayu.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gqsblasut.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gafguinzp.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gznwmqldr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gxvdjhenq.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gcjvqyuci.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gutqyzizc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtmqxthbr.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gpmlimnsj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/glphtpgko.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gwcbtdvzg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/ghstrtzly.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gxnddtsak.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gseuyoobq.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gelpafrov.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gutimbcmo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gpzeyryxc.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gxidpyuum.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gbtyntnbk.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glnxfwhmx.sHtML


<!-- 参考信息 -->