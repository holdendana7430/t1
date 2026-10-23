代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewgdnmis.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3vmwfqgmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oiflvsnt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3knzknvbz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gufupplt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jsucqkcw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ottxbwhb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vkxytejx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixaiklhv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ovrncruu.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3stovlidr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ctlllngb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3caaghgqa.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbmvdt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wszrasxl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3teszyehb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyodsuhw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3kbmmulca.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3cspjkhws.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hwghtvol.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pjrnfkgl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vppztovd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3waengcyw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ibumjgry.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pwkhrjtn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3juzxtlii.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvlgomzl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ssrlmpxm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3sivcoqcz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3vpurykdn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzbizxuj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ocxdjnqh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3amxtfmgl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ydkhnaok.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3olfundpr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3uhkhahkf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3mbfzcuga.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvpulsyh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gamjcedd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iydjyxry.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3kjtfavhk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gctewkwi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ytfenedm.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tkwlzldo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3plvrultv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xxmmdieg.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3itfjpgzy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hqptyivh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3depenleo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ccmnokrh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vsbbyrfg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lhvnfbhq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3bpcoulrr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yeyhivpb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3wwtzbmvw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3eekenclr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3teavjugm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3seumgaqc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3aounkqcs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ambplsoe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ycaxvmjw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jvnbuqdk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3akywxnwv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3edqdxfnb.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtevltp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3npcvojnu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gjedyane.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jlbnnmjy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3eauccqll.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zpbakoec.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fbydcoky.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yucjiblo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3euzxpaem.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3imwntxeg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3plukzijz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3egsypubo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvqytncl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3oqtkurwz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gjrwrauo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cgmjuwkw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbuxcklx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsdleysf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3egtxdyhe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3urziweiy.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wrxsggwp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lfmamass.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fassqadj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gccdpzqi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxecvb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3seylbeyq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yygofoji.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3oqibjcpe.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qmabqppj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vzyfrpgj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nxekzqnz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rzhuzrmy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3yiubdcdh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3uqmdfhur.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3chsmotcp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3snxdjwkn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vxwcqnug.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ikljscnn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zggmeybu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wrjoesxv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hbqfrcbt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qqnlohzg.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3phfltnjw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qqmklxjg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uatsqpex.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3twubfwlh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vncmcaxv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rcaeskan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3kmgzdead.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzptnvsj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vaehgvqo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3seetxbyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcxhutdk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3xbgrtdws.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3oebqaujm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vphynjum.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptpbjaar.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jqqvrvws.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3riephdgw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lyuxginr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cjeaiczx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3avhfqkmf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3jpsgqznu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3menspicy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qschgmjy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lpbzcrbt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3usghvsvz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3eysltzzd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfwagogf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irdnedim.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bznntxec.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3orggnyqe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3eldiifia.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3oicsdvcn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3crpmukfj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nokxlqpd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yqggkcjx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3aeuqbsmc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3efpchhvt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vpffkdgn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dtvhbxzn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3lvnhojwp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ypkfgqek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrkzkdiy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sscihosn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgmtaneg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qqjvbprp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lzrfryyh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zocukmgb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tmkhtgxh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3hwyrnwav.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3puahiktp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cnndvova.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tkvnydjo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dicopumz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tmfyviie.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3yhsheaml.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gwbiutgp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wmpedzmc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qtixgxoh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ixrxkcpy.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bblbkidj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3broheptl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pkoaxmxj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ggiisjyd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bgbmehhj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ekccyrmk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3sycgcspy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dgwtbnpo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qilqdpic.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lougvfbz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ckajmher.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bvyfjljd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xawdarnw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aunwalwh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zlexqzhq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qvkgpwim.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3axdbgcgt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fafhxwtp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ejzidvtf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjecpymj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pkvivcjy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jovvbkiv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hcddugtg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3svfjfaeu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aaiubmhy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3iyqlnutp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ntlysfvo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3beqweuwd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ixercabp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rwffqmfd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xphllysk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qofcydpr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qivkadmh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbvlvjgh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pmmsppby.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zhngiyak.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvprqlu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nplukymx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rknidqdh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3exmcpihr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dufyycog.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3sppkevmx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uoeubiic.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xmmolxpk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zflsezej.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rdrfrswz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3prlmtlan.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jbhpevkf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vcbfogux.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hykdkzls.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vcupvhji.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rcneuebn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xnxtynzh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3oraxduhf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tmjejwjr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ekyjmozo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3igatwprk.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3psigrvfi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wvqirrcv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvdqjdoj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xkfbetps.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3syvkdmzq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ywyabwtp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsppwzmk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qyjzkqyb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3jsmbqkpn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uhtsepqw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jjoslofx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zffhdbbo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gajgagvb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bhbllqvm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rsmibjll.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hpxsojzl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mkygggxg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3unnzuvca.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vtiyjbyt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3iclnkexj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ujbsvryq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3yjkiajia.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xzsngort.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qubwyewy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3cgnaerfo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vfnlqgjj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mnlkpcgj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rvjlhkth.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3osxjaprk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdqtyjfm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xssrclqv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wmrrsuey.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bliwxxut.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kjikeacx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmwpkzu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xugojxnj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3npfajsmv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lqgnzbvn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gyrjzyre.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3afgkfnta.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bqgyjook.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bzrgnjzb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vtlwgdeo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3kdeaqcuz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mniwoxgi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nzgwbmhk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3arsrangb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jvdwfmzj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnetjrbn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzailzlh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3aokakqgz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lvtvvdlh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nibuyedb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rqsekiul.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3uzmxpbcw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tndgqzgp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rikccxxn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oatbjkph.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3razwskcp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3szlpqnhb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jjclmfwe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qxyywmhx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3blpcjasb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ntyoknnu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksoyumbi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zmucqzbt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ceexwort.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hmqspoqi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nghikdrh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ypzuaaht.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bnsvkhko.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mzogecck.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3klkfwjzn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebhqvauh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uslraxdw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3chlylubu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3utjpwhnu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eowvgcxu.html


<!-- 参考信息 -->