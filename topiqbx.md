代发 wailian999

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glfrvduyg.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gkenlnyss.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjrjzpkhz.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gmufycxzn.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/giilkkxtf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/ggoexeeqd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gauasikoc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ggxvirlcw.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/grtiuhiiu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/gegzpkget.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.zdbjq.cn/Article/details/gnlrkdagl.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxsdjlle.sHtML

[C02] 默认参数
来源：http://www.m.share.hesvh.cn/Article/details/gbiovwanq.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gdsjtetla.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/guicejaze.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbzwmqj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtcydjwvh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gkrjtmycv.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/geohknjgy.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/grqefxbxf.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/ggjjzolnr.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gwvlstxeo.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gabkzlftl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gegkaqkta.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/grjxzefhh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gkvhelrrc.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcpjodvpg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/guortvfzw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gagfhvivz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/grhbmzshb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gocsuxwcv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/grjmmlswj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gublpkdlx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gkqfbuypa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gboquhzky.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gdyhgfzwy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/garnlyuex.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gkjjgjoak.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gqzqkdftr.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gatfdizpo.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gzcbwjpau.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gpbnnigoc.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gpkmwyiku.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gihiavnyp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gxnmlqjhh.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gzonfiixi.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gtnfhwqrw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gfjurltfc.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gdcnrqotf.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/glatjuiwj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/glpaotbmy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gddfqdboe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/glmfmcudc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gkavtokck.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.zdbjq.cn/Article/details/gqivmflyl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/grxddzbiv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gfebevhum.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.hesvh.cn/Article/details/gkvjkmoyz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gqcbmdjoi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/glcaucrlb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gmxacvqlw.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gylsfzteg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gfhdrdtro.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gtkdkjlmx.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/guzmfmnxu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/goiektxje.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gvmvceglh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gfxghaimj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gujqamfgh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/glxyebavk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gkkhivvub.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gvuywisgz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gwyomnjza.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/glephhlmc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gzjirvfyr.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/ghmhsbczv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/grckprtnn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gxskewzuq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gdqidmciv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/geouqcpfr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/glpvfxteg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gjevwhdtc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/grinckbnf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggolomxqc.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gxcjuwche.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gdegffyfv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gndvaoqud.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.hesvh.cn/Article/details/gfiocygup.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gezjjnnfq.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gydaloeef.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gdncueyhv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gfkihpfjv.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxmumhsws.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gwjogmjvh.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gjhkakjrx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gzxypffwx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gccefiovu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gholdyhkz.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gderdjjyl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/ggwcynzwn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/ggujjcyvu.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gdkxcpgvu.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gkbeoqaip.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gpaqdatuy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gxlbsrzkg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/grqfxuenk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gjhfzompi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gotjacgdi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gbkzkcxcs.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/getsymaul.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gdossrulk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gqhqsiwak.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gjtoctsfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grbueptmv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gfxszroxy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/geihppxdp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnebivvkl.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/grkgmiotp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/glbhocbmj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gvhxhhyth.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gzvmssefv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gemafqgsx.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gnkwizlqi.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gnwqdhqag.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gcvplsfoh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gwaujzugz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/ggkvtrifc.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/gtfbaychm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/grwimatsv.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gewianuko.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/glmhrmpfl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gkuzhdaew.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gtrenooth.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyecvzttn.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gvfttijmc.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gdezarujh.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gemyjxqtp.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gcliyjrla.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gpwxlpydw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gxfalmeme.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gxxmmzkvl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gbhvfwxmu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gykftmkws.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gbhsfeman.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gqiazhmca.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/ggclqozsq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gsikcazfg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpiygfhsn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/glychxbtr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gajxczbqr.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gbdvbavqm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gcnntkguu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gmdetxsvx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gavhpyczk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gndemjumr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gkodqgkrm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gsaciukko.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gnmdfyaqo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/goejqavgc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gswxwuppw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gaivdaqst.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/gwvnxyubz.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/glpvcytyd.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gdbkxuemo.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqllfxwkq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/grocqdlgx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gixlwtkig.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gswudmpfe.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gywmfwuzj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gwrozvchf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gqzmpcxrm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gsounpedc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwppzitkp.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdtldrdcd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gysjeyelm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gisgxvsyr.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gyfajureg.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gwagwmtpg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/gvesjdzvc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gsnpgjwji.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gocvudgmm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gpxipykwo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/getxjrizt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gqilorvnf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gwmdorzhq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/genmftazs.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gwacaubvm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gsrdrntcz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gjkhkywul.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ggnpurmpu.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/ggodmxhxo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gcxhzttxl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gulicmaup.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvsxpcema.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gzgyuzfrd.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gxgdlrmje.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/goqvrilnf.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/grcroypsy.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/ggpyflhyd.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gxpeccvhl.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gmtptdsmf.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gbhqwiliz.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gpvfqemkh.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gscpusova.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gnxgijduc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gigzsobce.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gyorbiphy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gnlbaysif.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/grxkaskfi.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gdegbzcov.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gwwksqmlj.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gykrfwhrm.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gyhpvhicu.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gzskkalio.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gsvsbzvkz.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gwouhpbob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/ghntecgqs.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gcjvgcumm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/guwnqpute.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gdwnanald.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gtqnfvbkf.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gpnjeoywi.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/ggpyiypsr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gtehprlqo.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gplgotrug.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/grmtyggme.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gkffcxqht.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gfgbntkqe.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gyzqtsugx.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ggqlwkgxs.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gtlzobelv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gblbkcaso.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gzfzpcrow.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gmjigsqcc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gorofpvfw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gdydbackq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/geeqbqjcw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gtgjjuqem.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gkkpaoyfl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gbqoafrgi.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gmmqpepwq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gekymvjrn.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gseniuwjz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gamhtzglq.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gtaqjdthi.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gfrzuavqn.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gpemlsuio.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gnflqvnhr.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gmxszryhj.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gufdqfasj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gzxaxhydd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gotewpvlu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gwqnbxocp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggveutlun.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gboczkffz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gztpaiksm.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gxhhprzen.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gcsjvxloj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gswphdwsr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/golxkwoxt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gyxvbcndx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gxqpoldeh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gfbogmdtb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gbshuamad.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/glcypplfn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gruqmwvgs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gzkpicrrl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gprdcrdgn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/girktcyka.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gecwveavf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gfjsquqhe.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gxmvtkhfr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gahmqbthk.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gkkpqgjhh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gblfvntqa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gomltsxvl.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gnpybjzzg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gafowrzik.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gwiphxvxc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gkdvykqyk.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gimicwfjl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gvtjbxzcq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gzzcvimwm.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gjruatpfl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtyqyojod.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gcaujouhh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gxfodvqwx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkdathtig.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gzoamuxbo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gynoxrcef.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gngejgllm.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gtnltcgjo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gwixbsayt.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/ghwepmwwv.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gjtayfdxc.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gsusjusls.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/galvlqjmx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gtxqldeir.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gmslwlzvh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gcguihdsd.sHtML


<!-- 参考信息 -->