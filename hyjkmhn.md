代发 wailian999

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gxbasljou.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gmipsejac.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.fehbvm.com/Article/details/ghatimkrr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnpbtidox.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ggjrivhwq.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/golaqhigw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gitwsgmjr.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gvipizaik.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.fehbvm.com/Article/details/gqzqmjbew.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gybkyxlhv.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/gkqmczidu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gpicyptut.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/glibekpyv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gujwtexyt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/grnqxklos.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gkzswhcqk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gfldykqrf.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gcppcozcm.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/glsjdkasn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/ghqmtnxqu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gyrrlscsb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gmxkbjkoa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gqrbjrayc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gulejoglz.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gollwmarb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ggfqtlpmr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/grqnfumfq.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gljafhopc.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/gvaxeevot.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gchxoebdf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gfgjnpoik.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/gtfhenhzr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gldfxxlvr.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gcredsmdp.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gshtukqwm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gelklbgan.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/ggwvcvhow.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gnwredfyj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gniitgtgw.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gaxagfiuc.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gocuwrnct.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gilkrwzbc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/grozdwuhn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gnhgbuxte.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gpbwxejrr.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gngpfqrin.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.zdbjq.cn/Article/details/gndkzckww.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gyazqoffg.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gszzuuhub.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gglujhwvh.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fehbvm.com/Article/details/gcskozifs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gpkjjgpnr.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gfnfzjnsa.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gctrcbxor.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gapmxsrtu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gihvajyha.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gnoptmqau.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ggrpacjhn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/grlfstwgo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gpbmzgbkj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gukdoaomx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/ghbxlizqv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gkkfkmzpm.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gnneqkpkd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gmvckmjui.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gxwtmtija.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gnvqvqqit.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gvnmwcntz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gbtrgmwjb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gwhxesyex.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gcwvfkljd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gaibaputx.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gcboroonj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gpemfugvf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/glnaycsno.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gdxffdfgx.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gghebmtga.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gcstkgnuq.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gsoiosdnw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/glfoyfakn.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/ghmymrfes.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gjznvsspj.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gegywmsaf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gayzamjla.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gujxbvlee.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gzodtwvhv.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gufalxdwu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gcuqtoazr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gcninivbg.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gvasxmobi.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gnertwmjq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/ghfwkiedz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gmwrqiart.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/geiazharz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/glkpvnczf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gwltrrrgl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gorgpwtbh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gummjwcvk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gfoftzfki.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/ggtmcumyt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gaeseyuuv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gcdlokkko.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gcoybnnet.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/grzrqcckz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gtnzdyrlh.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gwzuqutzy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gjprjwozv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gazmhxitv.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/glbpkddpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/ghbrtnote.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ghjaoqrvl.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/glbvdkbgy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gpqssokdy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/ghmtmgknj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gbwoehcej.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/ghpcplcjo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gufabdtwh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/geemomqfj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gsmbjxaqo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gigtmbmab.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gvghetnrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gqmpusssa.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gangihopx.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/grzcorgtb.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/groevfmlj.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gsijxjnxv.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gzvzixtej.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gxyanfitm.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gwfujlmlm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gkzxolzaq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gfwpglcfx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gosozpwpz.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/ggllhigcx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/ghjkdpuos.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gtmyradii.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwqfeefmf.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gotjgjrtg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gackyoofk.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gsxilykre.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gvrrutrtd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gmzqueqlh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gllzdhpnh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gnfudkfya.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gyedwdmfh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/giajdtifh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gjpmjmyxi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gebqozylm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gjzbrfdig.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gqnvifeyb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gyxculhiq.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gezlrcjuz.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gvndapols.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gafqijwrb.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gijqvwciw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gckfqizfe.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gzlscltmr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtteneqpw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gwhymuwlq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/guxofsppj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gvidwboyb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxirdhlqi.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gliscweym.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gqxeevlvi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gvpvvohuv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghcwezykm.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gtltpacha.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtoeobrnr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/guevamggr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/goaaxyfat.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gwkwbyopq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmpjypx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gegmnshpj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/ggejdwkxg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gapdkdyzz.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gxzrnizsy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gcabncqhw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gcaqydpdw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gzaopwdhr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gopfljhqa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gmbxrfnlw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/giigddgpg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gnsdkydcv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gygcvdzoj.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gftciythm.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gnqfaaojf.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/goddebffv.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/goozbmanv.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gnvyfuyrk.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gxirfaidn.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqjdthdsp.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/glbgkrmak.sHtML

C#:   list.Count;
来源：http://m.share.fehbvm.com/Article/details/gnzsuxkyb.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gcdrqfdfd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gwkptbxje.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gzbdudiwy.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gsvuwbwjo.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcsaqav.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/goxpygsrf.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/geddeqvqs.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gslisbaxc.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gixkaymep.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gewjohxnn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gkkvrepom.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gjqtsaqwb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gfqrvfrxy.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gtkuoocak.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gshwvckof.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gfoxpoxzi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gahentixr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gybwbcbpi.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gxwjjueae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gwjydxrqe.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvoiphain.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gvlfapddm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/geyoadadb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gqnpleyxq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxglgdtfi.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/goagblzpw.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gvqhdxxwi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gymmkbfys.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gzdcawvck.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gpqugdayo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/geeyjhsxr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghwugafub.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gsndxidae.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gbnbvizjp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gvotyxqif.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/ghsdnnjui.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gsdhjtvio.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gxzlistxo.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/ggmhifmam.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gtkvezgxp.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gguwqlooe.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gzjgnyibw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfvjwcjlw.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gyppghlpw.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gvdnkqqri.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/giknwnmtx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gcgbdklvy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtavetij.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gzxsfetai.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gcogrrohe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gqtyonxnh.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gfodyhvgj.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gjwspbdhd.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gqnjdxxjh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gitoclooi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gmlmdsomw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gthjxrimq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gdyqqjhuo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gcwjdmgoy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqbblmkak.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gwuakbxuo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gdokjamco.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzzgglkaj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gelvoijip.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gonukpthh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/griqfxgey.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gxsdytkks.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gvqakerab.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gvtfnkzdz.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gpwgypfrp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwqfwdfjl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/ghuwlyrlb.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gukqackdd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/guagflvxx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/glniixteq.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gclfxzjei.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/glbjjzajl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gqheeqdzy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gqcvjyoyj.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/ggjusfvfh.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gdgmsndpw.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gnaospoer.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmlamxyvy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/grnnlvkia.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdoveloxn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/glbhufegb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/graxfmduf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gmbalkhqv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gzomafjel.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gmcqxjson.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gfaxmwjfa.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gzpskykkv.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gruikfcez.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/ghsvunoil.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gyckkvusf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gbnwbliyi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gganbzhjn.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/goacuhmci.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gwbiyxqkt.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gsipdjkxg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gqgwbaenq.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gizxvwadh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gtqsiqqsv.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gbljwscfu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gqpotttmq.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/glsrlgqui.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/glssauydk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzfswzmlg.sHtML


<!-- 参考信息 -->