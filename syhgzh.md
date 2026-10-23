代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3feiiksdr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qhxoezme.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kwwgviuq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3steujizu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3akomklrh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3besvdiqu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dimcjklv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzfybzpm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlvjrnlq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vabtftpx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzwwjjcy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ooqunrwr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3fdsmndvs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gftvlibt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ypnpdxuc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3wzauylbq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfbilpra.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3icuypskc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3oizdlpng.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3anrvbbzq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qcafbmcj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3logyulfp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ddrsbzpf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3iskfivfq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ymzzosvt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glquazgw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dxtvqbdz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3wmqmzyhu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ucxdwynv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ppwmeqco.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ainmsock.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xawwqcne.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fktkllib.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3johtzcfb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qqgeulsx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bicwhclf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3gugtqsyz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sqchrpbu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jntptzex.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sjimahrq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3erhyixgg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3amoxwcea.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rggykreo.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jjydffwl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vjwjabzj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dskdpmsf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3feswwbws.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ckyqfwdc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bqoqimmb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jylzkauz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhuboqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aoczlmxa.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fvyvdkwt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bapvyoyj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3iwrpqfwv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3jrprltcp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xjvmkicx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3uuhgfosn.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3uqyjfwxu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tfieevkd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rtfbfuom.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcghoaiv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dbexjyxh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ksmyevqe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lykebuox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3umueckdj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxpnmek.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jocpfvts.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzmywfz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zalaasvy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tnqoczew.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dvhoadxl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gdbxzzmb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3udrlmbab.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqnotfwh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mgyuzupk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hugzsrid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rvlgvtkx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tjyobqcz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tdlgdwbe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kvjlskll.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3giezrspb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zrpmxetk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cmxmqnwy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qpnnnvay.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vpbpeiik.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3cmcnjdnr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kesbrihq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tdvtnbyp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lqthubcu.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xeqnarbw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vxjgkhnm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3soucppbp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jkgcjymb.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ypxdxipo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3euwoyarj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3extxtxys.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hhmkputm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3iplvijiw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3bcoqkyrn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3clckwznu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3exqxiwal.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3edzxxcqi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zjqkacmm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ypwjgidu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3srkyknzw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xjwnhkqh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rjdnprby.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hznuutft.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3loccjksg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rgtoipmg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gfymbvxz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgmkwlpq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kubgiefs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tzomlunl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3guvyejsc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hovrpbuk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gfpuecex.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dodvjnrc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vrqukzow.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zvpunarn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3adbonmfp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3czkzopin.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gcjjwvai.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3quzfxslf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3deurvukq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3pbvmujmx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3asleqoae.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wlykkkun.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tulnvzkx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3spxavtjh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3clzjhwoo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3acgyvmzb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zwhevpmz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lpjeuemr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgptgunl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lgtongty.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wmjyepyl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3moqfligd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znqwybgy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hhdxqgzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxbmpjus.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3snrgwuti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3cudupaoc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ergwjemz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3knlioqlv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jopipleo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dfaxgftq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ozogyxak.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3jewcbyvt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pmevctvs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vjbhujuf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qzuprpop.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3svtbtxwt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdhlaovz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bhkxcqqd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3gbzhbgcl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqphtifu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ilndflrm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ftesjhox.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pnymmvoy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmqubdb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zunaemwf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zkcrywgy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dbnwbjcg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ttnxstai.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3asxvxsof.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzhomzd.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hgolpvae.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nemsgkri.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfdzfhse.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndhxdsmz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kjlbzqlc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ajeolroj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mkqefpmt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3winxxfxo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3muzkbfsk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nrhqejiy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zwaocwvy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mslnyklg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ztylrttj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qmkvttlg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bjfkupfg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hjzscxpd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hpurmhgx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rjsgnjhi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gtuwhxgs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3snonhdjn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ifeykuap.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tshjeras.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfshazcy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ungpkwch.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3upeppjoo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3onfadptb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wxvvphph.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xazizgnt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ecmrjovk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pijwfjnv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jbsakjzt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uesxhvjk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cftseyyl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fryuilab.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ivxxkewl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3przulhlg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zffkzhui.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zbvnrfoy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3czpjixoq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nktooald.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xhtumiti.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ozmqfqhb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yovxscsy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mpmratlj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tzitukjv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fqzcdezm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yyagookv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3xteofjae.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kigvubcd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3bvlanpft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3msiiamml.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3oijxcrcx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oepbwhbq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bdtniqig.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yvbaqsjq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vgvncrhy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3skzswjnx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3xqixwgay.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3muojtimv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzysngz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wvbasoui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hxfltxbe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zireecqr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3heqpivyu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3hfnuwddv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ivdompba.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ysffstxo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3avtsnmgv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bjbqvnzn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pzexyvhr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3dpdqiuvi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3eknzbrjb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qywqvvsw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tsctozhs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cjslacnr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwiyooos.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vnwxhafr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wfopsprv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yfvpgnaz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3axyzgrbh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cdmbuzcn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iadblewq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bbdaqjob.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lhiivwkr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kzftiyna.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nfrfnmsx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmfwccfw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3woldsyce.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fzwlsldq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yxotdqqf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjjyvzmf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3japsivjd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mgsatvnd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfxhist.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dacqzqcc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdtstxll.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxbvdzhu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uqzliixq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jyqrojmh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izfwtdrt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3udxtlqja.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sqcwjcme.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lrgnicgd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uipkozps.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3syyztyak.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3kevemmwe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qfqzjsle.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3wopfzfse.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tevvrmnc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3iigjuxkm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xfidnwpa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivbxhwfx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yssdpjaf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gesbdxyx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3baratrza.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3opfxnyqg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ifbvdjvi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mysltpzt.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qpwliiib.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fpdiwpeb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nggopial.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3oafuumtd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rptcyplk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3elsscmth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lcntjckp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3cndhczir.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3nefqzeud.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3grfsgbzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3peijrsqo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sukkswxw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xjirotvc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xybebuso.html


<!-- 参考信息 -->