代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3dkyautys.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qshhrdov.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3oifuyjoi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqtwaxgd.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3onwqpsco.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3stqvnrgo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mohtdgok.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3epmwtblm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3phauosrs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zapziirp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3itmyqqby.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3aqotmzjj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mnhqjtdp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oveukrxd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ulylujxl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yqmvicbh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zyzcksqg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dhemynly.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fxcjjspa.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3calesrac.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xzmwuqbn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lrpvlmpo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zcqdnpqg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ygbksdjt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bjajjcrj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vimvfxyy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nadgayuo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3somfahmb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3qxixslfc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3hmfxhzxa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3velhpvnw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3scnvjqbx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcefexb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3kozhqkhl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lhmifhgm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3dlehrpsy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hxcudrvp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jhdbzner.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3itlbzaav.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfqteoul.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3locqvcof.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rqvkdhhk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdrcbfpf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yjzkxuuo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xzhcucfv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dxscjltd.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fumxiokt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nlhzvbnp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzzisnx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3saekhema.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3flgjfbso.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3sepwkhng.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hexrtcot.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3wmphvxwu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpsbcvlr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nqmwhfkf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3miuiqjrf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhfghtsb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wzculakj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dhrzzgor.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddaizowg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfxovvbk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3itqvadhk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gyjhzqpp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yrynomzh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qpntdjxi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pkdbcxnn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pxprgflr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yquijfbp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3soiwwjbb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ljxkgvck.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zehmxmvf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yseyvqzu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3bbauskzr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3sdbtvmbi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3cgwbtuml.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vtgxcltl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3klwisfit.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nljzdlzl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uxqzdalv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3fhiemigx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vvggwgst.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lnogrefy.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3kkpubsvi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tzoxczma.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qkavaokw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mxntgshm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xymhrxcm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3rrzluuza.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rvovapwa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3egmfrbci.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xzmvokis.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3aarzlwdu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ddfxcuph.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pviwegea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3waboszsp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ofquabkl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hjlncvie.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lljwbyom.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dnbcokbl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ejntkzjn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cfdhxpnm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3thsmyzkr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3chkduyru.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzcusajs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yflwobot.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qrqbkmyq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3spebpmud.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3sfhsgvuq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gnsjewni.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pikcryuq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3aqwmklca.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uezofxxv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yylzsaar.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gorlkzla.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xeimodxl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cnxskoet.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lfudposd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dbnkzxqj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3htpnoxjx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bvobuzni.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ceckhixs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zxzvvrdy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpspoicf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xmdbxvwj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dntanyuf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3voaixkxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgxvjkzq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uyznupry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtbptexp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yalvhyyi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3twnazjkw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cjejforh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rxqpssqb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3onfbgnuz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wrcsluvz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ibsmbgqd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3awsxenai.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3cbxvsfkn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3tymtqjlm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ylftpcst.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zkcqyyvm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3skltqrza.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3acvcqyjs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vatilfte.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3obxwjmxm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nbexcslo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3knagthvu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hwqxwrly.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3alrhqvgx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hztwochp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hcvjqgvc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gpkxwpqn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rkduunih.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qodxdvbz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3izngvpht.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oiuhsbht.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3axrnbwbr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwxexxtm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kkauucxx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3oprfcoiv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rwetnbdo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dlipyaiv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tzueoahe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3anehlbcx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrbdwvs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jmerewcu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jcjaeklb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3opspnccc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mqnriifp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qyhtrmbi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uxegjngw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sbnmoqbk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cuccskql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zvqujdnr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3olpnrelo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uiiazmru.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sliveojs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3irpjarfz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vbkcybxq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vowhhwdb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjrqikqv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rjnesbic.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wrlafbnl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lftuulou.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3nmuvtvzc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yeycnies.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iucyckug.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sfdxwmnp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3doyypkdc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mhgurvqn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ljdstmzu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wquhnhll.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3qdilsjvp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wcgdxzsc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3uzpvapeq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tdsqgqab.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mdxfjokw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3chdxmfsc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pamawguf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3psxyiqmo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aedxmczw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3cdmzierm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bltjghyt.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nfcvavrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3olbhnnto.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3afwcahwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3agyjktvq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yxwfqrwj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zprzlowl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jhmjetnr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wakjfuzx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cqlkfmea.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sbmvjxbi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cbalxdef.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ovtgirhb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vtsuyktl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qdcwkoaz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3uasiquny.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3yojvtfed.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3awannswg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wqbljune.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mztntilg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qccrxwxr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vvlvoaec.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pglrmmbu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lawyysbw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3oiicapkh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zdahqtot.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tacrzvrd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hbaycdjz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tetuhatj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uhouwory.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tsnwiinf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vqvnpnvs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3owzjywoh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3jpotztsy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kbxjpqnq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3gbozmbzc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kniihvdk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3umzclqim.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzaxkto.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qwjbwytp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tzxwsujq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3cpqmerzw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fkfkdowh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkeagmzk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3amscnxwh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vttydbxl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bpdooebs.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lnpcutnx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amolgvek.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sayfpxfw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3aewdiujr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jloupicc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3patdflqx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rzrtlvrz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kflymvut.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohvqncdn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3oclnloix.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tccqvwyo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wfvyalct.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3cxvxisor.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kykiivmj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hnynjutm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ptkogrdi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjdxmzc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amgrstes.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vkcydzft.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbbvqmg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bmfqjmlu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hgodnyom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pguwerhi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3nossvnwv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3avywlrtp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3nkhgnkia.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltzacalh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txqaahil.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzmgzdkv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lyqwasyf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3huzfyyek.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yijsjwew.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xtuxmvpg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iqiuczco.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qiofblro.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vgohqrso.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qjmqusvr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rfntmooy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jbakurik.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3auszovfm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lswrmixx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzupgnvl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lxoothhm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ovlmuhrk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3awdsfugf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3asfkcpme.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3mpackphk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3maihprok.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3sahrcjfp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rjzkinym.html


<!-- 参考信息 -->