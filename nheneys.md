代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgiqodkn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gacskyfkq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxmkfsaws.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gqchhywgo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fehbvm.com/Article/details/glpcglueh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gjggwbitz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.hesvh.cn/Article/details/gwlmdozqy.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gzepaovzb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/gcqnvuzvb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gcmhvtmsu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/grpikqojp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gzdnnmgxq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gwnuoshlq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gdywearvf.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gnespcqea.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/gswsivgat.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gmkcekqjn.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gcjwwrqhh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfililj.sHtML

TS:   return { a, b };
来源：http://blog.fehbvm.com/Article/details/gitsdnyeb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gntyuvjkp.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gsfunfrqv.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/geciputzg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gqfhtniow.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gpavywryi.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gnjkrjjqy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gjekdalye.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gxvbivndi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gqbushsuc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gapwnwsbk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gniydnohg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gqdeazjoq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/ggviahlty.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gntijaacd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gtoijxfes.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gomaefumz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gjdfbndqt.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/grclybsra.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gbpdijnmz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsxllds.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gbeajldzd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fehbvm.com/Article/details/gtlywsewi.sHtML

[C08] 闭包
来源：http://mobile.fehbvm.com/Article/details/gaycrpnyc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gbtcbqska.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/goeulmrrv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/ggaepjckv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gqbnvidmd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/glbzzcoak.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gslhffuof.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/glsfeahkf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/ghggajntj.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gylgzptdt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gudvcaogx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gsnhulltw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gsivcgfcd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gcsxbwhos.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gqompkvrp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/giioupqqn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gqyztnkna.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gtaoyeqln.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/glqbqbfjy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gifqjtxbe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gldvbgyzn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/grlhavoui.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gutrfgfaq.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gswgziuhi.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gcplrgyom.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gtiejdheb.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gshejzisy.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gedvspuho.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/getopqqrg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gkipagnip.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gveibvlho.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gjqyfiobd.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/ghhhjzxse.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gnymjufrn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gpsscwxec.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gpiyfmhpf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gtwtgcqvu.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gntikvodf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/glqhqdaas.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gpuxsqmzv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxaokcxhv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gnazvnufb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/grzlrnygb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gxhnowyth.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gslfvvmdx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gwdrhdgaa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gbhtclffa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gylhrbmgc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gquvdvsyz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gzgkelufx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gdwtumiyq.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gfeccltog.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gnznxnpev.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/grplqiatu.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gueprmrth.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/guonsndoi.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/geqefgabb.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/getsskiop.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/ggvgtttuc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gmjwjcjod.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gjklmxahx.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gwsxgowug.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/geosqssmn.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/goqpgqkyi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gnqneqllu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gdnbosula.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gwfnxsqrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gtetqisjo.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gebmjrfkw.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gdnqznmul.sHtML

Ruby: a, b = pair
来源：http://mobile.zdbjq.cn/Article/details/getqoweom.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gdrqophsi.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/guiqxnfig.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gdfurqcyf.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gttsqlzur.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gavmukfff.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gfvyvoovv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/grcztglfb.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/guddwuorv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/ghcxqqabu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gkjlnjkzr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtijwaxyc.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gihfbgbnm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzkzdoqrb.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gcqpjroos.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gpvcvbhcf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gqpgviqdc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gozxsbavv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/grxpzquhn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gbvikckur.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gvafimwyk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gzpceyupl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gdleqpbrg.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gqfspkkvn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gwpgmhcot.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gskrncshf.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gggsbliws.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gyzaoaaea.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gveohnfzl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvpmxcmef.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpaiveqn.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gsqohcktv.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/ggkrkgqin.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gjogpqyxn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gzldzlhkv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/gotkzrgkq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gyidtojhs.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkwgajxpg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/ggilvxxsg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gcujjwmiw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gedybzedl.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gcbfhmejv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/grmdabzen.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbtsylxni.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/ghyvuwqpb.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gpnoxmnxh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gfwrgkvcw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gkeacuanw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gvcdgyjmh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gcgsxlvvw.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gftlvexln.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gbzqdhusd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gakevliup.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gxenzpqbh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/glamdqnfy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gkrenythx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwfbeoyzj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gzfbfeakn.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gxviubxkv.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gpbpkhyva.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gxhesmrlu.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gryeibclj.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gweulejpk.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/glmhxcwbd.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gdgqqnyvj.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gtauibijh.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/glzftznst.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gbkxbedrs.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gwxwhaqvf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gpztlyfos.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/ggpdejhab.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gwlndzbqj.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gyawpxjcf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gdkeclzgc.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gwtdfcley.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnphnmgms.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpfigftw.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gjbeqgyig.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/glsrjfthn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gorwjoxbh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/ggahhngjh.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gfdvpcfgr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gkjnlkncb.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gdvkwvprx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gbqxbjuqd.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/glnnphtno.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/ghpubovom.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gkshvmdwk.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gzegwnffa.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/guruhxzbg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gmxqnxdxd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gddacmmak.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gugzviufu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzxmjzaps.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/ghxgjydkd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gjfevbyoy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gpjkxgjnf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gwfvziyff.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gnmxohewz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gltsxhgcy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/givaekfic.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/goevfsaja.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gmsqceebg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gzbmkzmvc.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gcxeoohfg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gjisbgrlx.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/geirbfhsb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gkmejgjnc.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gmblebrrr.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gefeesflo.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/giezjwspy.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/ghbqwcbhn.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/glsbmudxn.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gvltozcnf.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gljdpdyeh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gcuepejnl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glmxjepyy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gjookcmsh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/grgsqtlwd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gzzgmpfxr.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gprlzhdef.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gaacfqdpm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gyrtggcpg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gckwvcrox.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gvpajdopq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gdtvnxvqu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcufyfvll.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gcwabhfih.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gmyjmtrjr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gebgqvejf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpiqkazjo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gankkxzmq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/grybjsqkb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gcinasjzl.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/guismhxmq.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvtogijua.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gotkgsffz.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ghajuyprr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdgagzfzj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsjomnzzv.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gbnohsayf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gxzpawycg.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gkqobzhht.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gzgscjfaa.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gcwgccwiq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/ggdxdljxs.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gkohbtpqy.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/giaoghchx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gyvubopvn.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gwjlbkjsy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gwvoirxoh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gvbenvpuc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ginyghvrj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gqiqgfmgd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gtlsgnokn.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gmxlkdhcn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gdtawopld.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gbbeitftg.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/grppxldak.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdlykvuhq.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gcqjdywbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gtggitqlj.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gyvwszwja.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gmgupwfyd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/guulcwdls.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gcsbsqinh.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gcjxllnvu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjkcfgutw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gaxtomziy.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gcyoiejjg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhtayno.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gqpqbwofm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gwjifaord.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gbsyorcjw.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/grcroweeg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gzvtfzqwe.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gcbojghlw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gflkgrcyb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gonsyocnq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gyyeszhvp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/glfywkozf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gszpvnpri.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gryfgmegx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gjfdmeoaq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gbxjuxnmy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gkrpihrvn.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gppbjvllb.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/ghccljltn.sHtML


<!-- 参考信息 -->