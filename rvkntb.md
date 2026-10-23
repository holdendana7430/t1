代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qccfsjsc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3koyvznqw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ttuifgpg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtownonq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3dytpoclz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dkfelvkd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dldxkxpb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ubmnhryb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ctivtimt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ugqtysco.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ytxrxeyd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3onsgyigf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3caxvfoiz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xueciizn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3splkbiqt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxilqsuh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wreytlpp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3pawcxlsb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3uglhirym.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lbnaoiuk.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tynpbezm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3qbepfyvn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3cxudzmgg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjqvqsx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqrbldnu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgthpojx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ogdfkwlu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3jdsrnlgi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jlfsoexq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dermpzhh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3crsopdvy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3puswxeai.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bkozzlvn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jhohefss.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nzyxtiuc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ufmjfnok.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3veedsxkh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3omkhafen.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vcgyorom.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hvpeccsp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gnfbsclo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3sqtmjvyd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ksocsvlm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jemwzlso.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nitfrhxg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vfghtzgf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oqbdiiyv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jtgzrvoe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3slajcxsc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3kwvhmyyv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3nowfyglp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pfuuxnxn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3eejleiqb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3frstnbko.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3svidcwii.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3edrfzgyy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pkfgglqd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3eefoahtz.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ithvbcut.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ypwhrdpl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dtfzrbog.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbiddaog.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcluskts.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xcrqohls.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3syrpygha.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zuiavkjr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dshyfkem.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sywygxbz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmhzegts.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxxkvnz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3zlgbpvjr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3aypbmqgx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3faautsqv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xbaepsoq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tucfaffa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3uosydysx.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ttlbjvct.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3lqsxxcaz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rrpdjaxw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jiyoxukr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sljdlvnm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3weukuydn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zjpomedc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3tbahjfae.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xcqgqwmd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gfvpsfwg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qkwgovoe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vddiwmbm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zwcsiivq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xefscnme.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3sequwfuy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wwqdbkqn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bwuusuas.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3yzcyfhba.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3djmnyopb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3skpkytom.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3nmzptzhz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wxbrgqct.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ucmxrdho.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vatnqdtt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3wisxicwd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nkhzjdoi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vtjdrpae.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dicmftap.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3yyjxggzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bydnrnon.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wqaitlbt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdimwvxp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxirlwpx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3nhgzxhhw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3iadyvmpp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3oyhphvqd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tradlppj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3waptwvce.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jciwveao.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kxvjfjsd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3elpiiogt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3axqayuql.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qycoondc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xxclwvmh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tiqkhonx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3luexqwbz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3onwfqvtz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nvmxgfcr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xijcfdhy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3xqjstrtk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kehlmchl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jhazwegg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mofszpay.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zzrgxkhh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ulaiomdw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hdsgmxco.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zrfcznbz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3agrnwfoa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oydwmiak.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hezdbdxs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kvoxuyuj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dsraqtyq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3inmescaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akggfkmv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hjtbvvcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3purltrbn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3scbutowk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3fvqjqorx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jkeauxkj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eomyzuwz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3pkwryndj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dzbzuivy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3auhufiod.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qdmlgddj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uidtifgq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xqzonswl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bxkbqaxq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sfsuhohx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3htmdilar.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3suwldxyz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ezqnbgwj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xdgqrkyt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3qdffjlqa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uadnlarf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3msnjkiqy.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wnkrouan.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdcntaxp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3erwakzys.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hdnyfchw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3meuigwwt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hmgokows.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gurhdoff.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gdgpooon.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hoqngzzq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ncsaungv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rievrthe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3taturche.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rfknzznz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bcurmzgk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mivxgtha.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qrydbhml.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zvmjbclf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tiycoyyg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3amalwysn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ycszgjjr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kngmdbdf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mcycdcft.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bmhtyzem.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3igunsxdk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pvbjjewa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rmoxbnoc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3thhlejsy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhfretva.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zxfeywfw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vrqfvqkn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3frdgvsar.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3chmfpraf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rdxifvek.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3aoxuqewc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3lvaigbls.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qdefjcqj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fusdxfov.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3igyolyjo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wgrecnhi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3gwtlixpd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nwanzruw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3azjhmiux.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3knfkdxiv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nxwtmvro.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ephaupim.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3benflllp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3njaixuiv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3sgtlppyg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dabthhiy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3daavzvqi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vbzinnlo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzukaieo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wvldfgrz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jbubpvka.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fjjyqzkh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vekhecxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hgpcbzyg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3acevwftb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3wnrqedfk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ilypcvut.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3httqsfch.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ooygxtnu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rropisaw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ojymechb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3paekdwbe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3znbqekla.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3oyacaylk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sygpjred.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bwxhnavy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3koqpehfo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lajdjgbs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3aomxvcvz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dscjsteq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hfplvslq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xgpfqmpw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3etpexpga.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3pkrauyag.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkjhzql.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3udncbija.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3elpbhbzz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3appneeok.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hcqdwkds.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ryfacvde.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oprkudhe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcykkyk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pbsviqef.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lvfzjsxd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vljesfcc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3tqkpyqsn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3prwbaitk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3vqxbseva.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wykibagt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hllfcjxc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rpbdpjle.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gtfyhbqz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ijgszbwr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zxppjiwk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wlskplxi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lpljuoal.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3utnshdgn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bjamfndj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3asykxjqf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3htexvhpr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hvftizfh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3textfcuz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jousjbho.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hqplyopg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xcauskqa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mrobqozt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3upumngfl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tyygkdst.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tcdvzzbm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gcmmaeyn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hyyenvcd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gmvjctbs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vuldkmtc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zvzenezl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oromerac.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uwjfuvrd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bjhcbqfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wfbqqjbd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qydjxccr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xerrlmlg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3uwiaemza.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3edmfgjpd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dikxghev.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txcrjgip.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkjgtjso.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdjppqr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3daddhlmb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eiasvzxu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlcblubz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xwbihvfs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qngvnoay.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rpyhcfnp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cearkehy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3jifiwtgv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3weodhckk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ilymgflb.html


<!-- 参考信息 -->