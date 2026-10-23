代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpximgor.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3smsaspjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijlxrhfb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qqdlrdha.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xbzrtmmr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3catocjqi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3edzdixwb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3twtrpwwv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eoikflgh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3srdimlro.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzfndqgt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uowhjcbd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3aekibyzl.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3tznrjrka.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wksqvosp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onrtgdpu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vnywpbji.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ukmgmfwb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ypnqgvjz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ixkovfbm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bkircbea.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3aaiywcpu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zbpunpqe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3syvonojq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nxerkjtx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgowwonh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3eliukjep.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzqlcw.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzmdzszf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ehsczcws.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ebuwgenb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3oiuaopvj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hgcgsmpb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3obwkqcig.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qzskzhhp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3qqezkmzz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kogyaiuw.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bpmjeanf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qygpzarm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3iklkxgpc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vlbdfchw.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ksvqyiul.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pgogaghn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zjcvomiw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3louoeymn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zqqpenjn.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3doqaevyu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oftkbzcu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xorzytih.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ovnkbsti.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ythseutq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qrwcixjg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3izwwwuaj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rjqypxyf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kslxpqsp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xdhrhoog.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3imfrnwrn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bwznleuj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvtdayt.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yhmlhmzt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3arezhoju.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3unexsddr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3btaupeww.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3clxuwimv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3obflaise.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ksvjroat.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vgmlmwsl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zvhumocx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ronbawee.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3unwlydll.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hjhtxbdq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sdullvxg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3grwxqnvy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3guelekiu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvtwfkqo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ikenbexa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nozzbedz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcndltll.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dsboovop.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nqqycciq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3onpgomnp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wdxtrkcb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wgbyvevs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3dttebngx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ynyrzxfb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3sggkomxr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ozmtgmlu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ozehalxf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qoxgwbzt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ezxfmvzn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zgmohqos.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gqgyancv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3blofgxph.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3axbotddh.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tzwkgfiz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xmdabmbx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nmpijcmq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nxmyfquw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xoeimvqs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3famdkofn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3tdjifbjf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vfwxfxbm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ykqybwwj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3pceqqfrx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hxwkupfo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hrzpemtp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lxawgtdf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ztregmzk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nnhfpdnd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3oizavoet.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmjsvvlq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ayhrlkwm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hbpocnhi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3rnngynra.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3eicbdffn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vxrhoczg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uzvogobz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ezzlcfvu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ekajqxuf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3xyxppfui.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zxrgsdef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zxcypcgj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3spgqqbnm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zdywyade.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3otfqrwyz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdajwosg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dhscoeeo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dnmfxihc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oicercld.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3uowthfvn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3sxbdhpwx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qzlpewng.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yerokbdy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkidvhsr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3njedolbq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mofkuhqf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3krbiqcoy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zbcdviht.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3fjoyyhjl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fimkanlw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ehvqcnym.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wqbtmatj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ctdvzgrd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utezizwh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gfcoaxie.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3edtwluom.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3oklacupu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmzapakw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ydvfeaoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlgzxnlz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3umswhzfa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dghlqmkp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zqwufjtd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gpirzcyq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jwjnocmx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rjhsipgi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ewoexitx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hhkefwwz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jfiawsfm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3opyrowxt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zwbxctcm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bnvuaoqe.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xwhnanen.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gtzzkvdf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3atopsbzd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wlcenxym.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qhqueipg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3vdbpkoyp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ftllqbie.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3betspdpg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3fstgwgaf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bntrhkkl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3usykrypi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qdlvckrx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3lanvqyfl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3dpisyhar.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rsmjegpk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xxutaoco.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3wxwckopx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krsjahpe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3thnpwalw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3nvuenffe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xcamxzzs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqrvqcd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vkmfvhfp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjnthamp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3rxwhghip.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jwyuxiey.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3emwocytx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xltvbrtm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3yjocebyy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3prrahbyl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mvosgvrz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ccupovnv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3flqezgwf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bexlixul.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cklcscjk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exdultud.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fujkndqg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lgzgumem.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vzjxvilh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3psebxjfq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mhinadjo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rvnanbve.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3piwqvhap.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rjruwkjj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3brmlntct.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqamgaog.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3psgvmeci.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3emnqkyit.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3wpdxpmpp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pbimlupu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cnqvooye.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mkpwlbeg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pxibftyg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3bhlphyfp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zeekzasb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3brpoqrju.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vreueyju.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3rbjhjzdw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qnuddwkf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bctbexid.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wengbuob.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gfwgdtva.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thabeoxl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qeqztuqp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3vjdnhchi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3joxgmiik.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cybjxjef.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3iiateroh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3slbjazkg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nwbrkfgo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3upgagsjp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3shyxmawl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tgxfigdl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3argqgwnr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3smxaklle.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3dzrzdtet.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ooijrycu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hppyqgzg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vqdmptnz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ircnjpag.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ntnyzktv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zhdqilce.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qcaknout.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3auprwnrj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3liqjxmhv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ojkohdlu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bnewksxl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gthugrha.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yhiogfvh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3onvnctqk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3itpbnotx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cmrbsere.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3dczzijru.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vgliwjsc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bhobydgo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3amvaasxp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hlgqtttn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iwjjdwmd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3zxahuyqd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3brfzadee.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wmbfaqqj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3mmyznikn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bwhfaqdp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hqeltspj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ouvqfhbc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fjdoymvf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3utmphajj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hlhsddvq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqrmfgzr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uhithvrl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xyvdgaqb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nektubzm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3lwtcjsks.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fdfnuctn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lqcybsab.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3axsgsgiy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pboebavp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ycrbioai.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hqjoobhl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3oasjoowf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ftgtvdbe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yetoecaw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ocbnkxxc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3xplylaxs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqxgrpkw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhvzkgde.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mjlczyqs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ynihtqqo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ckdjzlrr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3aeyjpwdn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fqwxwtap.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3uoqwfdxo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ndokngbi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtienbmj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3iyhklulh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qqesibmg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqfspytk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3hzyvjieb.html


<!-- 参考信息 -->