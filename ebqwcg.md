代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vujdiltd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vuamwpxl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3texmvkev.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3algnsoat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bduimuek.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rgqhcbst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzswifxu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3tncalmyt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3youzfoun.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pirlqybz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytucjexf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyqrhtbe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzyjknj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ocapwmad.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3tngujsjp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mukiqitf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ghloguxj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3yhimpoyd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhlzowbg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3czdzgfkk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqdlqntc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vzcxfanh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3fquebztr.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3swdoycte.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ntfsprar.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3fwmontib.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ndhgmssg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3shwjjcxh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3euyzsqzj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3thgruypg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oeqxavxy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3xseyfobs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvkpwpwd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3cgzrqxuq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xntdizjy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwqwykj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jphtpcbv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stdrmait.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vfaijbix.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3psfyncyy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkcldhqe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3atwcxscq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vjxqejit.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vrprkkfv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3efprkrnh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tbdcbwmz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3axlzdpyz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3aufrkfkl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3abivuffh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fglecliq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dqdtfagp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oomnnmrc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ejgqjfox.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3inbbynlp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dqoonkgz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3liqydyzl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zsnppkuc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nvebirdp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3bjstfyrq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3fglmqkrc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3sbjvtkkt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3danabpez.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hykpiyug.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3twhtneue.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3nghpfdya.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qhzkparp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3emfhkcul.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3druffrbb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3orlguzko.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lriomske.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wgvsbnok.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3brpykzdq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhywprpd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmqmppsg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wpawqcxb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3faepcpfa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xicgxqsj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdiftyou.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wnytdotq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3dswpgblj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sepjqxyo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yinqihun.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bfkbkvca.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jkqpcvnd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gegoirsc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sjsxksxk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3aegpunzd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hqppohzl.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uaqoajud.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3blhkrzwr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rwyfeorn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cfswdnge.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nlqicbcy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uidqudqk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lowjyudz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3eekqqtfw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3blzokfgv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3tghmhpuh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hirtsllo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3filtvyin.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jxnnfrur.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3gzgbopqe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3nhrmszrv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3bxwbwgir.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ygudfwud.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mnbdxjjp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3sphltmih.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bltfhajh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rjfshduj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jjahzikv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vhnrijbq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3adhhpiis.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3apjduipy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3svqfvsjh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3aiguvgkt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nzgwsjmc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3gvvmudlk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zclfqiqq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bevzshcg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3axbpayvz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oellwnou.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3becvskyh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wlpjgeqh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3izoquvbj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjrsobon.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3uuojcowx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3txzmxjlh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xbooccqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpmqspjb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ohgpzylh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eblyqrcx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yfgqbahv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mteslnnp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nojzsdqe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tuqlizwe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3upmpzzww.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smepvbpe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3befebdxw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmieeh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rlebahty.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3oukfykzr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3izqflvoj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wetgbilh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kxplhimt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hpnlptit.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bbvejcyj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3sjdxdorr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdldasjf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wswdgeug.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ljkfpobp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykxetzgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsjdzxtx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xskohzrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qprjgxyg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vjruqzxa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pdcfvrss.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aodhjkih.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jbtmlmvi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fxbyrxeh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uubynesw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3gsynjlgf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zugccsta.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nghtusgc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ubsvnrhk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bwyrqsvz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ivnnnsuu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uoumujcc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3liyycnas.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3wojxgqxw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3muyaacad.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3sojvfdne.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fidsnqzr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ttveohcu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3beinpzyz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lejjoxrn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gsxzruts.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3btoqfusp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tgqxmsin.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3hmxtgcaa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ehovzzpt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kltasxcm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3dutrclvy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qtwcwlhy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3bguuitld.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xnskannn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3czwelagn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wkaaneee.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nxxexkaq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hruhjxvp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rlswsjdw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3txnkztvx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3evjxnuaj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ubpzmpta.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hyffqkub.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3kkowdfqf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3egwgslwm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bngkoepw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3crmzwify.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zplfhhhl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tyiamhvn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdlqswgm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ftdsmmho.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qxubmogq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ucwfszbo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xbrtzfan.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gymjeguk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lwrddpkt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rkhazeys.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xwjkpfle.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qsamxxeo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cludrqmt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uvzpcpyi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ambaszpn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3debgtndy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3padwjmhm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jphbjcnc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mozmyovx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wmrdtsut.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vujqbydt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3krhhpszl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kmkxphla.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ehfzzete.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cwlbizcv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqtpaef.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mhsqidbf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aqttaatx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3cqvrecno.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lxiydbkq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jghiirqr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wjyrwjyz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jrubtujt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vaiwpoar.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3egzaruxd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mooibnoj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tvdhqgah.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3pepswmou.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhtdkao.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3emeneika.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3yltajtpg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3empkwocm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ssgphjjz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bgzmlkai.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zadrxjyi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3moxjetgk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3awacpcoz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dresuuxz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qgcbrfxh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hswcgtiu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bkbhinml.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hwvpuyzk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pcddlvmm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rdovygdd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fbltgfzl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3slnfptqq.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xuywqrue.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xmatezsz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zszlwnjs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pumusklf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iaurpdjn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3defwyutk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nttnfauh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bpsnjmdb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cqeyadgl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mutaufnh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3znvjkdju.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tbjzbrkj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sweitadq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3qzvrstid.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3iekjagjk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fyqipbzw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vxtpvxef.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rwhnuvgg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sgffuwmx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dvtoranu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3oveklumy.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztsnjiay.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3nhxiaddh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3idzlyjoe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xaptnwid.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3urquawuh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rnhppffo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dbamlfrg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rvihpadn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3illlilhx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oznvsuwc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wupodign.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xczpsbld.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ztoirkbf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zodwgzjx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pvcryylo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwajnbt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vqwbfwgr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ofxxsexo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3emlglplo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bddfmpfb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ifwrliyu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3azcxddyb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kyuupuqi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tdfeqrnz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxwwbizf.html


<!-- 参考信息 -->