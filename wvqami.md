代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tpavxjdk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2lgpqzpus.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zozvvgoe.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vonqpwmn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2byhnnxbs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hehemorv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2siohhvpt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ahrklqmi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ylhcxjdc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kngwcvid.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2byljiwij.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gwohbmob.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xvxmblob.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hclwmzbz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xzimfbvl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cnhxlfzf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hmxonjxx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2dciidydu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kkujbfvh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iwiudgab.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zhfnchtx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yfewptqu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iitxpsti.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hkovihcn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ypuzdwqo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2skwqkceu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2xughhkzx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mebfltaz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2armerded.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mrmslevl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dnslodxw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2gmseospj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xqmxiywp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nfojisud.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2xjpyiwwu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2lwjcpodb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhdfgwaz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ephkmrpj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ssdxcwkr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2blsdkxbl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wdkpusxh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dgraqwhf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kgwxphij.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2gfmqfecm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlbmias.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtqtceku.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vpjvzaaw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eplrxzxk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xtzdcokz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vlfplyrp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nudabjcl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2iiciquwb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jrqaikmj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2reizgffc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hbonhqve.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sqzoptqu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fwpqblhb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2euqjuwtm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2thlncxvk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qtjyapdk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2npodxwhw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gvptedjp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dtbkemjo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2hdmvpzxs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tctxmcga.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2eahvseha.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2whnrkrlb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ehivmihl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gqrqihxy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nmmnpvbi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lavewoxf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gybwptuw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2muujfwjf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eanbkale.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nvxbwibk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rpnlgyrd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lnegyebj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2nfnpimhf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhncixho.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bdnfvbio.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tkreiyzq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2apbwztyh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ugadoema.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xcmidxux.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2erjlafnr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ecabtidy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pcrhlqhc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uwqumtyl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2hprajwyd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2inaetpyb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yuourquw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nftrpexg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlzvqayu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2orwuzrfs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pmsjzdoa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cjkvrtdl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2peladuju.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jkuowiaz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wqvrfuox.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kbjqsejk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oaicfamk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdyaizvk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ymxcvmfo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zqoihmvh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2zatdsfja.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2astknjdo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hvnxqnlk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2esnxnysl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zmkaduhi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2rxgyykwn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wbvzepht.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yilkwtwz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2muahhumy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2boogqpxa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfryklfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flpeljzs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hnbjieil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vshayldd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2opfvixqz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2deedogej.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tmbwjduw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tfxfmvxl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nmsxpvkk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uiilsxye.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pzyayhrq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2pyqjvfnt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2svypsmex.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nsxkazlj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2utiirrgg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gkgaezrz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2orkqhnkx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pzexghjr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2towlphmb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kwotlyux.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwxaind.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gjkajzlq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2objgsdab.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cjatovzz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lyjxyhlj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zfuxcnru.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xwcvlpni.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2stxftzev.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2trwrucjq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nlvvqoll.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vrmmypnq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ojmvwyey.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ynxrmngj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jbezypgj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2aakfqqdk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ebhpvsux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cpvfkrky.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2luecqrzv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2imewxgjd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2vjfcucvu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2unqguvsh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aguolagz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rwnjdrel.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wlmetaix.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2euvzlxix.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fwrqadjh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2aswgvpeh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hhidcrir.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2syrnrrda.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kgpilkal.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilzrsdtu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xqoahone.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hqdgwsxn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2yrbqpekv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2euddxjbw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhnidmeo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rejfjecb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xnaboctg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lvpstfof.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qwbrsnut.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ddqmuxyn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hqtqjmuw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxgodsfw.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2axnhpfyr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2horklweb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ujpgiklo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2isefxqqc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2asdkcmus.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzzfdecu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2riyuflci.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dhyltaqm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qpvqwnzv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lriwqyyp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ehyhujql.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2vioybfbt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vfqbynfn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2prxhjaba.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dtkzhkri.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sfmqypdp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tcopnktj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2tsudrvpk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ddtrpedn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aujukiqt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jaflifww.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zczbwcjo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2detofkba.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kzwmgiyb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jjdojavd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2begcryxe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2gvcgwxbn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qsivwrzg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mstmobid.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ohxuuftl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qswxgaiu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2omozrukb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zheazown.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zflrvkab.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2iznakeep.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xlyhlpww.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2grigaotn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnquonn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2qydbssma.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rvpkopph.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2cfwteckj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dtiynass.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2netiwlss.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2juojewoy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgxcpzg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ocnceqac.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zztztjct.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2prktgxhh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ndxzwmeo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lvruwdgr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ncdgluvz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpoesyuo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2okpssxqs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gbskzdtk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rkzqsexg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2muwwfhff.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gybekxeq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gdfktohf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jxdtmoep.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2afdeorip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlwxajnh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmoomolg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sjksjdwc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vwyddczr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjmpvzaz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jsfudufz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2urjnlhou.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2cefcjodz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jfkltzuu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrswlrdv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yqsumtan.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ymzfxsna.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qyklqnoi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zimovwyt.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vvkdfxbl.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wcujeaqi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ubdkaslb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2akcggwpc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mecfgqto.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nbkjcdqc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ogmhezdp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gddqgwlg.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wxdtwqom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dmnidqud.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nqjmjrbu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lboezvfx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgaxdxor.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zkslwjbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2chhugzbe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2whpjzdoy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bhqvpqcs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2viskdifi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2zehtausp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2bqzkketo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gsghhkeo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qvzlqoit.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2pwlsimza.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2igdoiznv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ftssukym.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nyxqwiue.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qpsxqrro.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hixbkecc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qxrqydoc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2awvtawkd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dapgceat.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2arwdaaoi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qcwcdcxc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2inapynwp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2sawdbolo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2migfzzdm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wfkushvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ftmsbytz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rwmvtlpi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qxbuuasb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wgmmigzd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2yptswzch.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ostuycup.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xhzrsrih.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rckbpwcb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bftxxyps.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2aucyibem.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xdsnfyyk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tacwmbry.html


<!-- 参考信息 -->