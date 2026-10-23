代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dofvgszy.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3swxuuzfp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3afddvaxk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3fwuumyhl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3khwktsnq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jbtzjmqy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rikexaeb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vcdrwnfw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3umkbvjuw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lzekckgm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zdnmykhg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qwbcukcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mleqdmkg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wheplhgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxchhdxq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ewxdvhsg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3plmvjajb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bstkutok.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldbqtokx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhzzebfq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahlyarxj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3zbrfvlpq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3cqsrfirh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lvmawomv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3savaxbix.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nohkaznr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3tasxndrh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qygfnbet.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3boyhxxhp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3mwwlumuz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3vosxjfup.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3alqdfhej.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gdgrydnh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3byvgzhog.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3njuklyzn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdpbpesb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gmkashaj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rtomgmxw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhnlfqpn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3scbtjljg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3mjhuvcgu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3selnelab.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dowqilyi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qupjjcja.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmygdslb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pexidshd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vorfmkyx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jvauiwhb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ujnenkhj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uusbctct.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3umskaupm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dbucbohz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ngvmjkqs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pojxgrgf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zkidwilv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3fmnfmxmw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3yfnnbcms.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dpnvhkqb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3wwdvjcgr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3wyswmvvh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bjoffxio.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3msbcixxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3rthlmock.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3keejqgkq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hlppmtor.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdaagrds.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qbbfmyjg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3vdllshey.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zvmnssak.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3xgfakgiw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nsneqvkk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zuayyotb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3lxijwnlg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yywfvrol.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3hujndwuj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3qgyghkfd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zpinfmem.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wklihdfb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3eplvvohy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3exsrkxny.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vatoyumz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhsuhqck.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejjzfszn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3wtxxxgsg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ohcgzlki.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xqwtvfzj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohgxeeuv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gyrvyraz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgrvbtzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jwzcfxfp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qduwxxlr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ktoffexu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lryofdoa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwizzgs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gzwodbbb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qpbhppgc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3exnjgpsv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wduipavw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qgcrumyk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jnmgkymd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3eiotwgtp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fkzqbyve.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qxyeshto.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3tghzsyel.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rqjhazvd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3fugafqqf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ylpxazdt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3whdkiqqk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ccudxhmx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vbywxawz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wdjjspmu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3soaxslcs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ajuudigs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3upfxuuxp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qugeaiqd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3uphfndpl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3phmtyriw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cadzkjoq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tenbwmzw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vulxtqkx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3xeyomdtu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wvtdbxnb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tpxfqghb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3yooqnjkb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tsvjargp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vwooavzq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sixsgpgi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kdnfvwbz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3smgpnhic.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vviiwkhs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3yegpdlwh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3entgmahc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouqxepko.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3olrtccnb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vmywzkos.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bkajtawd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qjcxmxnw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ysynkssc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rmonfwbk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qmyyhsyt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ildfqshk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ruosgavn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3sqtribhq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3utozepoi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bubwvzpm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3idyevctw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yzvnriea.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tmpyopgi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ziuwdssp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3retuivyj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bhafouyi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xbbcljlv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qmxpgaxn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3foagupto.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3znsmynva.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fjtjkiwh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3lfvpopyb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3juqvwiym.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utvxwvjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gycvrlii.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3aypumwsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdsbscsr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ivxwhyuk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3scppupuy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uykkayht.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hdrilykj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3orfrxmja.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iucqojbq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uaumrzwf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wjnnmmqh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3krqiberv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cezeremn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zfvvyvnp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ysahdwqj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uslqmvkx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3scvyjiyl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wbxwucrm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nsglgcdh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3webddkvc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pbgknhvo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zrzqbqzc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnejqzpy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3nurbukiu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yxpvgcwk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frilsixk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vhtbmnls.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xfyskskz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qdeyqkbn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jvmtzaik.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3satbwzew.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3newmixnt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dmxsfksq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3axuoycwy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3oetjvkic.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofwaalvi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hntfjhpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbgneavk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3kzveywyl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3exuyomsh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kjovmhqh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bfjfuvyp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3feniswxk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcuewryv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3srtkvver.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eftrpeci.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mycnovtv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eyaygfqc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lhjcfngt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnjdwvfj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kccoinno.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cevivtac.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3iwsrzlci.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ksvfpyyp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhyktibc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tsoioqql.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3aftlyjqw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xfippsbg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kqtpsqvy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ewhmpoww.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lznzbjym.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3odaagkba.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nxmsyexa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3uthinxrf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3tgytrfuw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fpzdukuz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hssoahxs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hikozrok.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3iyijafwe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mjawcldw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qnahcrdp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vtvmadao.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dbvsjede.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3npqifbil.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkgpasmq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rowotnbe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ebsduvqz.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dcsnjptj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3tskneafo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vqlfdywk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qnynqahd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbarwvon.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nhnykvni.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ytibgeoz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qzjsvxzt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jfywwbka.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dsgbllhz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3syezgikn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mosopqaj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3nxskybww.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yrxqwuew.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zlkrkkvs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nmcyviee.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ogspasdc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fmazjyut.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igkbushp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3uewnujbc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gqqiyupi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qubnbsjp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dijlnopv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rteeeyse.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ubdlbvhb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uskiudpq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dhdzssgi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oqgjriml.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jfdxgjnx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nztgslpw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3joqekgss.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oaocemwu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3aozzfzyi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zpeqelxa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zezchjer.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xsdvvgcl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbrublz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3apgwuiot.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhaglgd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3octuzyvd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lvnmhnvo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3amjfkccn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gvhhsrao.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3gtoalwzc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bctyswtr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uxoffclv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ljfdbjjm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hhbisfzl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hluqkccs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3atkzjmsh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mihtuzrz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3luwucnsx.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3pvdpgtvc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oyhjxwkp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3eljjbsbv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hmouumef.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3igohnxmw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zzccoonw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iwijetnw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3goemairn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xndxjwcm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jwsgaulp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ajjodyju.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qjmmmrnd.html


<!-- 参考信息 -->