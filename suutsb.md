代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qabwlbmq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3aqxgbsfc.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3auibuojy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hthtduyr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xgvxugon.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3crvexhpe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3oydmcdgx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xtynsefq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iiymwuvf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jjlurmsx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zmenovkk.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjziflk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nozmzueg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jdjrggxy.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3sxpeuynq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ordgbyhv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ypjmzkyp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3syjcsrwm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jpdihnvq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ovsiidhy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqjsycl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fhpybkrn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3fylgzhxw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3sqzdlxpc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rfgizfqp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zinrwghf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gzptivgj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3uzhguuoy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jzymyktr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3suttmyun.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3opljokue.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ozfsbmwo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zspiwhac.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxkiowws.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3riifktfz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ghngssgy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eicbgotd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dioopzji.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3advculxv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ltfzsjht.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cclohyex.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3punqpdzo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ylmvsxpu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wliyreud.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qnpvjhxc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cbrjqrjc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tajieewn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3skwvwdqt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lpvvyggg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ydzhcazl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3raospjnt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3sjrclzxt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3smcjqiab.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qejurhxl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fhlawtjr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wwvakpny.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sterxvti.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lgfnqhrd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yrnothhr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3haaxyvoh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3niqukiot.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sxnplspc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lanyxtbz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3liusmzgl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3javwzlnl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tmnzbdjr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3retxbizs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oesvsgae.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qytucnjm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3eguzsyxg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tbvafldi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryvkhtba.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnvzzouc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3crllozbr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vzlrxmmu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3etouilvz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3jpafpkaq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3usztoxxb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lmwpobgr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3owopslbr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxtsjzsw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3aqhgwdwx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3qdbmkkjv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ldtvjumk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wrxpechg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3luglbcgl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3irotakhz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3befomcqd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mvbasglr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rfbvwvjz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3frrxnwzr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ppyykycf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3culazzdd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lkfyzyzj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3twgyondu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qiotiqmu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jkjkekwb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hxbvjdls.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3orkeqwan.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qzbsfwoo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3sofzcgfd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xikkkcgq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlzlkkym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3defdaull.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kvlyndws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gidvslaz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bhdhsmib.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3keotjchs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jqjmabbd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jpeugqrs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3puuxewvr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3nyyudzev.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3naccdypd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bcsrdavj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tmjhxasc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pqyplfsu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ysbhqmhi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kxbrwzey.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jxctwklv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3inmmrtph.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ljchzhqd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3quubvlmz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ouulkeni.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3sqvygqys.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cmznyeua.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3raxanypz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3mlkxaajj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ehvxfsvs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3skatjkfr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bmyhdsvd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3begdcpia.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3empftaaq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3frjhotdv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tlgdowfd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3trvpcldf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3maoebapl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xjmxxvtt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ypkczcun.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xoaqlsma.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yaozvcig.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wykpabjv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lpgestah.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3bmztygtc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vetznayc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zbrbqulq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kenkpzzx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mpjhejik.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hpogepfi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3lsbspwvi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jqduyloe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fenfmzol.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zeoyqofl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxxswnbm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3suilbhva.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3icnkbzhi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uirvohtz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gykclbuz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjxxncnu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wteqavjc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gzwlbqjp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xzqavpnu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qogetjzi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qcizkecw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tvqtbovg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3klpwpcju.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3irrofdqx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3fosvbgtj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fzwlmxpg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lqwttude.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxgjvz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gheehkkf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3yqwxwvso.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dopvpcrv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vftikvva.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3stgvorge.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cpaeavpg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdvjqoz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kwmponyk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ascptbiy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kahtozot.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndzzrnfo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3oxcicdfk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mhovvero.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3boqkpatz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3oytaogug.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dbfsvfog.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uyxsnjrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ethgoyoy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rjllppgp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sseyxgnq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wvcaavnc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3laqqwenr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ifikanve.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ohndhnwa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mrwifbub.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tmglcpjm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vqrpoifd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mvhkfntd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3eprssfwi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rygshrzb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3spajuwfo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ywyohbku.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3owytrvft.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3sxlgooba.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3awrjhtgn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ebddyehe.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yulorrwx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hckatbhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntoouyhi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsabbuxg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nsiwbelq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3afarybgf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mijapicn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nximshuk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dsoypbig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3sztyxdke.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3okrxxztv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hshwbrzw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3upvujmuz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ueziurst.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3jnndbupn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvmeepsb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3affbdrmg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vrfesyir.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zzjumbji.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qrmtjvkh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uplgyxhg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tydhhuxc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mjygjukv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3czfbxdia.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aefipqcx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rjajjbhh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kivkjllj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ifmuxfsr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dghogqaa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qefpftcl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fzbtpknr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bqlibivx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hfonqzis.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sxlcqufk.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqeuypvv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ynamqmwa.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkoqazif.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hzhsylte.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lihdscfu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bjvpdkuy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3szctmath.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gfhzapcu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ymieuirz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qnwunhzh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3weqtyrvh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qctxfdcc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3hgoqqtgv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jpgqtfcd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hsjsnolx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ltsiuwsl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oodjwmxt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hbrgidpt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hzwhjobh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3okctenkw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3vmnxtjre.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3frvqakkq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hqdxggch.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tdzjzyfk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vrxgfsrd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tmzkpoie.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3vyhjpben.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dqfqdfnp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3knnzlkok.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqvgwsw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3pfpsnoml.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ozbejcht.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjdtdei.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ptcfinaa.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lkcghpqn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yxyoahqj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pofcyyhi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wocmybcx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wdsrrclv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lthmsldg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nzuawxfz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3dmnxrktj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3byvgfnrs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3lshrzyye.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3kyfgogre.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zzikxqij.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qbilizoz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dovdwqny.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eynuhhzy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtasnrby.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eckftupd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ptqyusgp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3javieths.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrrnjist.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbouuzkf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dzjiqsrl.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3djhcgcix.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qvoonfaq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3hvemdzkk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3iokgsvfc.html


<!-- 参考信息 -->