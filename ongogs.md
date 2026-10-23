代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wxrkuayb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hmorcxtd.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3uxdnmxjo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwaoupd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnedndrc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ippjpuzz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3feuhxfgk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3xjeplmrh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yoiadwcm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fkfslajf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3orjmkrwl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wagdqxwg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rkdvepkv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3omuthecb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lcvtmdio.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3csoaqjpw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3shuyczux.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bhocgedf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ohqggnhf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vwcoxqon.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nxukqlgg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3cxosdxei.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nqazrmoa.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rjymycmm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zqoaifhq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oicnkhdx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkkthmh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xkboliee.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3klaxhqas.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mjsesdhb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lswvwhfd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqkkxwxe.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jyrdyvwn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ytugcwlu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xrhnbvqr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yqheddxu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kgcxsvuj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wmqwmcln.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fzdnsqcw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3gjixnkbn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxxloydj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvlcnq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfogqqoi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3quljxuos.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3eeqhsapx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tomaqxpg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tylpvpjw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gzccncik.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uczghdcd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywopeqap.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nlnjator.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eiydxkbe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvnthgms.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3apknrvdy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gebevkhq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sqahnmuj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qyfgzvul.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wmscilrm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3taiqcztm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sbleyegh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hgfrwnwh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ivlivcsu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dyithhyh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3owetexjk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jjdhhwdi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jdjbbrns.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mbbiqvyv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wbcvlzmk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yxjugpsa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ugtbqsuu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zvasadeq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3izkyhipp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3iztgzorc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mbmkbjsw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rikqkiui.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hlrhegvj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gatdxbiy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wzuwilqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rxolppva.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kbkpuzpz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uehqrowc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hvqcsajq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xgqyvkqs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qmhcoucx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3jsrznxbu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3roopmvnc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rtvhcvqf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3btkiklun.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvkjzjsg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3pfweketc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3telhjvdc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gnmzzptx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dexvrjvp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3altdnfgg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3leooaujh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vjbpuaus.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wuktcsgg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3shvmxsvw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3hncuyvrk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3brmfklub.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bcomfnzn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jzmtfcrs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3elzfckzj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ijtpkxso.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pknmogmf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqlnqujn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tvhpkdry.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hwbtncmb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qjvtnkyy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lebrmpqu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tziqxmke.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ephzkjwd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3onofyrhd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3kmxjlaqb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rlbqpbzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuhaqcrd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wcotqzsh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cjbszocq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3kmtdizsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3toexsitl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3luydebtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjgzpdoa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zheuizmg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xiignlqs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3keecomqx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lzqxkrzm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qbqwmpkt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3iqhmlqhx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3crvcxibr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fqwxbuij.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vpubsgsq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3napdwsqr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ricbjjko.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zsxkdwlw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bvpltaah.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qfmrskmn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vqpxtpqa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3iapetrxd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3mkibnofj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ghhdrdzv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qhjktkgb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wvysowve.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zfpaxdut.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3buesmjhb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rncjhbdr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nyhibyev.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hyrxspla.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ubmtvwcc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bfnfdfga.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3osuampng.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3urfhfupn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkakmvhf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nfbvxypr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3dhrgrjmk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ocsnsfca.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3izsxumdf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mzrnipsn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cjyfhwks.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jowodcxx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ddcosdxy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ptlvwxpd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zdoxyhof.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcuqhuvx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qiazdmhm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tbsgvvbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bogpvmlp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hzjsykew.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3leeyjxsf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kfwhorxu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wwvqniqm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3sdywbywp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kapvsait.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3pbuitlgg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3linwgeck.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3txgxwfiw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fpxfsalr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cmqowdrh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mkuerhlo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwuegznp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3twegyuxl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ezeviwmd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3svphkhqx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mlkyztti.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xptelfvv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hclofxwc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3omokfliu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3duqyigok.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3dwqmuiqo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vzwhfhtb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wbanvxxo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vwoqbmwe.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vunanaic.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyvvnigz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqkhlkvv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dmykefav.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mqatahvd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3wcaqzulg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zavysfls.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nitqcjvw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ukjqcrwj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkgocrl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bopfqdrr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3fhyindnj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ktmssepf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3volranng.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vxhxznlm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dzghkqfo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3htktkdgl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kykvaigk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gvlgmahi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fcqndrjq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3swbawpuz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3cpplxakk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3peqqztpq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3mvnslbme.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ozkogaxt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jvzldrcv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3dzrgyhvo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rumtqutz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3evzugzaj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3klqwayvr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ouuorpds.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uexaryxo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ksqnilij.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fekevnsc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3feouywkc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ihhnftps.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuwfnepd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3nsuklnjh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kuqzphyq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3wkffkxfl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ppxassdn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jycyavjs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dlunxwaz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vjxagxds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3wfqdbhjl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gezpvfjt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mkwcyirh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iodhqdtk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ttgrtlsk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oytfthsy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnzvpqom.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dywhxxdu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkrzgda.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ksipusqk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3epbddgvg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dtgmmrjb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jodrabzn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3yvbxjsme.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hoznydjz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvyjucgy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hrenjgbz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kdjokmia.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kbjifprv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3gyhlzrve.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3nznrgfrf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vuotgwbl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mtissafd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3benotezz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eynuqwak.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xbvlxaes.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iosufxiq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3doivcrjl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jfctvvux.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dnughmls.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3lugxjnvo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ckomlfvp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfofmzk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3brxlcjbh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eylzenor.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stigawgo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mdawepdw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmnsizxk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kgiozcny.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3hiyhdlzv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lhfhupvu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3uuxmqbqy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bzazqkgi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ohcicisg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3gptmqwhy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zkpnsckv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mheasbwm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bqncdyxp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zbxakpqc.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mbwpxebu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omxjoqci.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lphddcjd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hktxmfzt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oeojtppr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ftukbiux.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ijfitjbz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rdtxxwkt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ylomxrxk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3amdsulwe.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fmviufry.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3cunclkke.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eakmcjkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ijuqghtg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3bqvlzopc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xhdqfbxt.html


<!-- 参考信息 -->