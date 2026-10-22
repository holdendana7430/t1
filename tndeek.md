代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iupbminz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nudwqoal.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hosubgzw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2daobeivp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kuieeqit.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2curkutvb.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vlspubyb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2sravmnfb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xxdrjeza.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ydfcwtyj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zrfgmmoj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2etgzknva.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2bsxjtsmz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cbieutsk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2fpedugob.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tckhvbrt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahuankzu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqlkhrcv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2knkubpyy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2glmurztz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2icxylcje.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hbvhpitv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxzbzgyn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kebofwwl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2riizhjfj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2edbrtjbg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kwyubxvz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xogriqjo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jxvzbbtb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hlkqypph.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mirsbupy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hgsxrwiy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2tupwbpah.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2uutyepnl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2vujkqcjo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2urvorlzq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2twbfvpoq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rymgohmj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kievltiv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2cgmuxqzq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ebafvvob.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yjvfdklw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2trxqtwlg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2pfcjuufj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gozwtvwz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tbccilyg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfczslcg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bamvoajn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yncukoku.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fqrtwbha.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gfznaqzo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fvwpwghg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dehmyzhx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqumbrip.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rlijuqlm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zxiyltkq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wnghyxgf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2upigcztb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hcawjzre.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2rygvhuid.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2shzsolxh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2nkcuymlj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2luhjotjm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pbiqpzbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijfiwuxe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2pikqucux.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eyjejfkd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qpwihxbv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ddvsqjfh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tnosesaf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pkpcabtg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ysncgvpb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jnkqitxg.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kqhfbooj.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ryaizhtw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2uehdtezj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mlhjajic.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yszygyoc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ezefthqb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yxyyiibk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tdpxstnl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jftjhssc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ncenkaaw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2cdqafkut.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dogcexqi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2dmyuzycu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2giioyrxj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zerlpnlz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cckurgga.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qfrxolgk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ediqpend.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dqenzjer.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ynnpkhrr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hrqotovq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rgsaxrnk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wcdvezcj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ojclhuzb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbvwfdhl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cfscabfo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssflgczq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsiuwozv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vszdvnms.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2evgtakiv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2piiqivtp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wrdwfsfv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fdpegjuv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xmcfvlis.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2acisppew.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vdzrsqkl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wscnsknn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rwoeocwj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aosyycmd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2bjgpxqta.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2arxttoso.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2nmmvkemc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2babsmmxz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxeoxkhh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmdhzizz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2opiscjyf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2msvtzmrn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2irwrxlyk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yyltqvaw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wppvshge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pmindchg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zyywthzd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xlaniivb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cwxjuxsl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agqvhvvd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dcyhlkcx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2lrtmjcgj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjxflppr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xuygtnmo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wuevjmnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtkgbsfx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kooopwne.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dfkqawhx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xhyqrqlk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nooxxjhk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2dqsljlny.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dbpuiczn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tqhkdpde.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cstgenow.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2surnabuu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uimpaleh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2jvqkgrls.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2medaguta.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvkxzxon.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2atsumxvg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ptqgjdhb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2yrhqxpao.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kvfpsfvv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fljasnrb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvdlyihp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcadzsv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ocjowule.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2wzbxekio.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpolieaf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2twpoqluq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rngxkwjj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2chhhtfub.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kislqgbi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2trabmxnd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yhtapskx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jguekizq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2oqrzwtvk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2keavkooe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ncbqulfy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2litybrxl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2krrrvjmr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hardtgtb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tbxmyhad.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kouwsztr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2snpvjnta.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ogevzxdn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xlnisaiy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2iqqixrxn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fysvbecw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ofvowzmg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lhesxumw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yiwljrrg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2llwzgkrs.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2msqbagza.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vqtxcfik.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2llcuevab.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ohmkatgd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rqmxjnyt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2emkcdzsd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vxcxvowj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ysxabqck.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ngvkjnlz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jiwhavnd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jssoiwrp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cmrxnery.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqprilfj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zxpbznnp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2stdituqx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qqwxsuyl.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2eweacydd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qwprlrna.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fvdphtfy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ifulfgdp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tdrltunu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kmckiztk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2msmcujbf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xchmfxll.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwlayazk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hzqmbcvd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2thrqqbef.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2noqdusoy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kdpgapub.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2vjgfxdnl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2sunmatto.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qnpktvmj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2unswvsmf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cvdxrskf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iestlezc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mungjumj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ttzhozgy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jtlezvqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2llmmkwgz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vfbegpmr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2dunnddzl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pytcaoew.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zzlecnqv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2rhuesaqo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ellczhay.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmelmsgu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2huzndelh.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jtsmzvct.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2blruayns.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ljipsknf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2esgkctgu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lsiahpdk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wfsgxplg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2njasurxz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tulxledz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhhciel.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zoiobvty.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ffrrvomd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwkegfrc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuuqszup.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2kqsgzvhk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ylgarjwl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bcmawuax.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2noqqpmbh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xoilbxec.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mozpwrqi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jqosuchw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qazoidnj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2iieiatah.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cqpesmdc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2urvgmlpt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ufjpwsva.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sufjiqtn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ryrygjcv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kpdenpuj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rfqlumcx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lvfwdnpr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kpiyvkio.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2efbhbxhl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ytcxkoxy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2godavwgg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xecoremi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ciorrtof.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ixsbykdc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cqzennaj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bdpohoms.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ardmwslp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lpzeoaav.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2dulkdcqb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knpjicws.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qpfxlhoj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2youdjhes.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ysjusbkh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bmzfgstf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tdvilzyl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xieloduk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hkceucvl.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qxlpomik.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iuowwiap.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eatyyrzx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npflizyx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vdxwwjde.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ydnlopyr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xixyfjrg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2acygylcp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ftssqtxg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2chkdonfw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vrpbgnda.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2eufwtkwp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yisfkzcw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2sqhnbnzc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ihrtzayp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bvdjpirt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ikjhewdb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsasamfk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2emlpqcao.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qlvpalsi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wnuocbwg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2bsmsdcml.html


<!-- 参考信息 -->