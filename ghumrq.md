代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xteesxgs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fqhsnyhj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nauxjbvx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrgefeb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnnmefmr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3irdlaoni.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vijspqws.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3chapgbmr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngtccmaw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3umjnxlro.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3wdlxjsgn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wjpakfcf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzcdqwub.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3llegwsjt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jgbpjmzc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3gosnxfhu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3npsouups.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uuzfxeya.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qxhhuwlp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpnhoiy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xexxfthh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3avawyjli.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3irghebyi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3dlmvydcn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuppbkcs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cplnfksd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hyuohorg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mymdftjg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3rfufbxsp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvoylntt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gwlhrihj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ensijxfl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gvoqecpq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxqvkyx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbhgwfdf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hfesxwly.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3shlurhkv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3eyybnyrx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3frlwbbcz.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jrwioyvy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vdmvmhmo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tfeshghd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bdfvbygq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3frfjcgvb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3fiosswoi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fvlymogr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3acjzqges.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lmqkzvll.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nnhmixgi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jojwyspx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3traacecu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xpdpgiht.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ioussokh.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3zbtzsitr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qvlhqiff.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3iupfwgln.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ydhzeqxz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ugdelwse.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndvnkpzb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3litfmbcx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wskoizmy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rqtyfpiz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ueijvfal.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3pzjfaegl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xxwybfqd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkwrvssc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jygmynfk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3iajwoswm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qcdqefxx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwofegnp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jtmseedu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hkyxddnd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3apfrqvgc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkazpqpn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ibbcuwqm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rqvfukwc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dpmpdvtm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ewmvhpta.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xruccshw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3abuusdxc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dczfpojo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lnbqgavq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xmfgowwp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kujeckdl.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aizitxvq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rckyapgm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3stncfydi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gntqlhgc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lupjmqxd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lxhrwriv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fifdajdj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hpimtamv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pvkrfuwg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gkwkpqun.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3orhwpgae.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3trmzdvmm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3dhtumaaa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wvochqtj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mchvjwxu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mvnhwgde.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ttlddwym.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3akovoadf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zaechnyv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tetpxfod.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vzzippen.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wnzxptjb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3siduvyve.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ardreewq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3aqgbrcmo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fwiyzgcz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bffvubpo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mgydzdsx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3httqvgyl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rtnyxzrd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kdyjkibo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lvhvntkm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bljjzeja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mmabviti.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ltrnvnct.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oubvspcu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yynavknj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ddnannwv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qszflbli.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kzkjedhe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jsspyzwp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3omqvlbqo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3lgigctlg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gqtmfrhg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stuojvpx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekcgzifb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3atfyzssd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3twjpdtjo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3nxbarvxc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vysuzjdd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3esgnuwue.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wsjewnqu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3acrihywn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pkmhtzgo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mflycpyp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kaqlnrtu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xibetiix.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vpaucwsl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3baqxpijw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhlnoocp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fpnyjzcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqoeieqr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tqhsdcop.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kyrwvucx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bhvniixr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3daeqgcei.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3icsawuzj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qxpvqcgu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3oxduikkc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ezzjrlyb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3bteodpwc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ksqtwisn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dqttcylj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dpsqnzpm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3skvobbcc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yfahejha.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tqgnavpl.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzxytnt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3trbqvjpg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zqhqezes.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmbfxi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3embdypxf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3imzjynme.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vkbfsisn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3puvyxync.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iokqravy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3oveateuh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dpfyerzp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dytcwagj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qguunbis.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mzmbudil.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mmurfefn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wxmltwsd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3doqiggyq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mxiatbbl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ssgnxilj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3avozacuw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3qnisvslb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3gsbqcgsi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vzbhdqrn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oscnamzq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hcgqgvfa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3noqdchem.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vexuzghc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vizwlmkz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aszxkiys.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lvwatzrc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pveyvmzd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3loivxowh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kfewiamb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zlnqzrrb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kewjcxiq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hzqndook.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlnscieo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3htezxtcm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gqgjexrt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kdbhyvqx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wfevlutn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3krxjpfzu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bwekexut.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxxzvxoi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nzszztxm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vpgoxqsk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uaghbhah.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ztkkfuos.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ceqgjpld.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mkcmaonh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3erukiqkx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pzkkueiq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3aglxfjcm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnlsxbef.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fumqstjw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3foipkcdl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kzxwzihv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cmztxxjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ysbpiuud.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3kdhieath.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3vvbaubjx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kpvunpoh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gutunlxi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dvoiaqoq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3skmxiuyq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tjckzsba.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ujwumatf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hozrmcwn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3sfvvwjsx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfaprqy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3grnletab.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jvmfsywa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tnzpmrke.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vstvuuts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fkoptffx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3yopvfcpi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3sgcduhfj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxukfhwj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3paspqhii.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3oqjkldve.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lombnihn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtcippfa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3nfbishfd.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3pwgtkkle.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3dduiapeo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qbidcjjv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3eyizeaog.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iysmgxvt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dyyqygho.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3eohaduzo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrsfdnom.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rnzegfbq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3trifdmug.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ygiqibvm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dergjgbk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uicrlpbi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dzhxpzyf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cbqixxlj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3epcdjpdm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3doochshj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3aodownya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3etaramlo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3oydvurwg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ubkxxehs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eznmzwcn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aijozphl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3broxhpwd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3yykbitau.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xenbljbx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mtsohnan.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3utzhvjze.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mzeutdww.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wurwdsbd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qzzshfxy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ltgaijno.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3arfsmenq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zjhmxmdp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kvjpemmk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zydqalkm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eaqhfoyy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gfbiuqgb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccghcxod.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfpqwfzt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ttxsdgbd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xvaoywra.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3eiqhedzr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3odxovwuy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3nnmgrbpy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3njyzmbll.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bixkvkhw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggjtrznb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yllsjahu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3uyvttbhb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dniqrdao.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oobexkmr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gykjyods.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dekocwim.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fjzuswqb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mntnvoeu.html


<!-- 参考信息 -->