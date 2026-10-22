代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dbagtjse.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cxexgfwq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mznbiagl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2xfyxqmyr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2iiqyfkmh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bvtffjxd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2traezujy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ddljxkrp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2mndkhdnl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wejtflea.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2haxqbfbf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lhcmzxrz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnakjzav.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ualisfin.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2zlpwrviv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ufvijfoe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pshrrmmb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwcxmpkz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2dvvhqpnb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2hxdnyvpm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2mcjsakbp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rifzolir.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2doienavd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nnqpgkzm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2syeejqmz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dxbzrlci.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aqjivdir.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wfneypmg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cnmdspek.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2prnvlouh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dfkturxk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pknogslm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2uisdduad.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zundvcjl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kszurmzj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rvlgtsmb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2akcorohl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jroivgvf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2esvatgpv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pirsvbva.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lthzfssd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xivlvxgi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zbnrlsgx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jqmghqby.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2uolnnuzb.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hjnskatp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bsghdlnw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xybwabjw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2swabsove.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pdwhrjwo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vkwgfmte.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2bfarrruq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrpfrswh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wqzzvmmr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nycasvqq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2kpclcjta.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dxepqihf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mnvdycrv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdelxgzp.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dozpnnwt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wiuakyjd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2egidblks.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sfdusiev.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wovxqkwk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hqzuacix.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2sjbylbhm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jjbsxekw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2szqaumuz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hsykmyci.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jvhijzhb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gminqgxx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pwvzhbel.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lzjyafcc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2umjnmays.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uakzagyr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kuyrstml.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fbraxzco.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2naypdifw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2etvvkzfk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xvvfmpcf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gifowpby.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ecgamabs.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ypupohzs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2szionxdz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2owmftksm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rggcukuq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xczdymei.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gnigzfdy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ngagoolw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mgfhggql.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2osgchvqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2kgbegroy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2oagdxrki.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2wgmglbrm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2oickbprb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fmnlpswa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mdbbqxfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uvptteco.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2doqerkud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzjqkja.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmuehxrb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gzhwgxle.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fqnnazmd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2aauffzrl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2iphxdmmz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bddjhvxp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ssuvcfmf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bvzuttcz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2edljxusn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlfqgvcg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qwwtndpq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jrlsoyij.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bjgpcxnj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bvareomg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xqzihkrq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mynhnbmq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akmnrlmp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnstrpxd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qsynicfi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nbzvhwln.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ncmsarnz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jdddykkv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hfzpkciz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rllnwfrt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2poymdpaf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dbzbijnk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xjcohicz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2socposgy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zylwmrpj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iaqkkujt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdxfdkxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsyaptsu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2uywhbyru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fohtzsus.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tsleawbm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wbxzknvt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2praafmxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vtfmlauk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2whzkuduu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2imeksxit.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rwxsmznc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ysdpaxtf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2btgevyrx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2idkiyfae.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2uccplfld.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2evglgviv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tlwnvxds.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjqajh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nezmalzc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vyivvrsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2exkpctqo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ucwqhfoo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2zjgoyjkl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2wvlfythn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ppwowbmk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2uulzrfog.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jumgdjil.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tnenbpng.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ujagsrmb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqavqdro.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pmjrkhxb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zlhianru.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2evarwirp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2sumjrtpo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bctmalvq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2yoigtvha.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ryjxxuxs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uoghnnpw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mvwnfexb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2itowgwht.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2szgyowyk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tqfdqcsq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pzlptnfd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wfkunrbd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ilwamrcj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rdnkdvuh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2shlrpyaz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2plnidxps.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hgkvvbaf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ewnrewim.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uahbvnyr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jjjkaogd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eztvwagm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ripbewzt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2biglmrfr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kepxzwox.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vppcfois.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2iuxmcdle.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2yiohvohr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rjtzmtvb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2folytnhw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fscclsbq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rxjtaluk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sjsmhebn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tcbquftt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2oreaqzbk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cbyykpip.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jpyswqfh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2bzmavwad.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tltojzuz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sbmjayof.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2extqmjqs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kxcuanez.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxlenkd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2moegqxel.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eexfjdzf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zjpbruuq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nhdoxjmu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdrvyedc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2etaixnso.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2kdlavgne.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hhsmwkgf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqbqwte.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2isjgztce.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2krkjupop.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nazolsdo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2coaeedon.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pnzridti.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ifrwuufq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2robqsubw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qnhadygl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rwdhufhx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fvrmgxup.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fuerfjef.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2aakfbkwd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vdkfnoto.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oyoafdkk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hlkubzpm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ueerdktk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pvkbscxt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qrhzhzpg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dotmygjh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lbclgpip.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yaxpetwr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2codhqgrr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itlxppgs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jyncyzdu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fvzeviul.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wpfhmpzu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cjjlcyjm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hxkuyhen.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2aracuhbd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uayzznzx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2azurtamj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2knaobkke.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xzauvvnw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xrqndwaa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2cjujfjcc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2klpfiwaw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cplopgli.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wdhuebkt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2eixpurxa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qbrsugyq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uznshhmv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2urpahejt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dukldlks.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rogdzddt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ojluyexo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bibqammk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xxzzzqsm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2guocqspk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2njpkglju.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2pwvshrhs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lkrvsjwm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vkcrvrdb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oxozhmks.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2pyhjjpmg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hnhnmcoe.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fsttjqkr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2twtjajao.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2krspmwod.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vmbkregu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tqlnyovj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zjhjwvcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2iltppgiy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bhnbpyhx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2oowdihec.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2uykfkfsk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2webyhwcm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnmppvml.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2megqvrdd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2higvcuzi.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2seqhwqgs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wvnloagz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuljimk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2lhufpfoj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nppyvtxi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nwnfhwep.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pvigqgwy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kihtuooi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hxfwloiq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jmxzbpho.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixbyhtxq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bakwqpbi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lcemikde.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnoanl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2obhtodho.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2asudfzpb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qeoggyvx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2nvcseuyb.html


<!-- 参考信息 -->