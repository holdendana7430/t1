代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ykiqhgod.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtpgmvip.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qhmukyqt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zrxhyeii.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tkeaidog.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kzhorizn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pinfcmsl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3owjvnztl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yqhxmegb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3jcwzbzvk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wwfzvziv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3axujndxq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nemmjexc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yigmknsq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hlmlqone.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ivwpssht.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xtoyxhwr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3lqioayji.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gpqmomko.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xmzobmcy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eiqtadwg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yrwtqoub.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uykdedps.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kjvhcsqo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3otmkrszv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qdviygpj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sklzjyrn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uzzgsbdu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tfdbkari.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3spfiqojb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lxknpwcy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fknmoqsm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jkbzrkzv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sogdyvdv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gcpnpgzc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3svmktrhh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ihfsveml.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3olbfzqyh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgbgucpq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3exzncxsb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3czcpxtdh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghahnhkk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ojcprbrq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3amxmpxoi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3uzvoevvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxjypalq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nkncvdbh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3eefnfgwi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3acykziac.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwsqnzql.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3pzgtszta.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mekzuihs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3apsfjgwe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qfjngqmf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vhlktrmf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dgfmveer.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3sjemmisf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wjiteece.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cuotzooi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gwmawpvd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xigtbzoh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xfkbdmnx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xmklxbov.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mhemnmvk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ndjwugcl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3gumtvngg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kmsddkcg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3jbnzxvgh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jioklyvc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hzeptwwf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3vpbwqjyh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3erhoaapq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bxvuxitv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mgygwudo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fksxbezh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ujneguro.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qdtdveog.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ieewkpdg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3swntwylq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3emtklkot.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vssufqvm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tauayffs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dijhholq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kdgzxewe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3anevborv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3tiwvbgsq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ygymkidj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vlnyduaw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dgfupdrm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3jtpaucgg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ssnkmmoz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cgjrgfhn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmfpqslj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3fzullgbn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ctsxgtkh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pzpsybpe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rquvzxhx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3omfuupnf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fosfrnnx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3msuszfre.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjmzuyet.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3leocmqtg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yssbwdwt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3fxeusvzc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qyaivuvo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tuirudfi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3mvbobezj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cgzfojbe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3uabkpmxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fkncnukz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3wwosstzw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3aozqguui.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vbocjcur.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3apbxbcaz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kemvzlig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3blcmyvqp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ubcahivh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnlhqjjh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qufzprqa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jygtvjcx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3glgtvwvf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mslzpixq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3keftzwif.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ziyhoefu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3amdhqaeh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ldxzwdsj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vhngiklu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cgekbycq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bzekzbfe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3qoihmwsn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3praovzkk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3koeodimc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gtmdoclq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nuediuxx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vinigkug.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qdpgwhty.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lbwndopg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btvvitcn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3muwlibfs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tlfonial.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ilrmryup.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jomfkism.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqnhmdc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3twzhpesw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wdrmwnft.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wfbiyhgi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aylgwbcu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpckwigc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3azqpgjbq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zkhnkgvj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3xmnlkxwz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dinkdzdk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3slheabcp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ugdpbxyl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3tlbtbvbx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aeidiewm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3itkucmvl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xbsrffas.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yaazgydm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hlamqgfo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3egyyrelx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pstrdntv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lnfcqzwf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mqbngrny.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qlcesxcz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hldwycwu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bsvstjfb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3byyagftw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3iuphqcvn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idggtwhm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nunvhidm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pagekxkx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3piztbvqo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3vyuzmmpz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lqejbcfn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wwsncztx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lsfdbtso.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lfvynjkj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3doykrpdt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qbsnptjn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3imwqzvji.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3uhqvrngk.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sufpgcnq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3qwaezsqo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3edzoihmi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lvqkdoof.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jklumufo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yfkvwvtn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3voajicug.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxfotpnc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3jsefkqor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oxbltrpk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3micysosh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3owpvsoro.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rzjfaekm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cdrgarmh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txejrbtl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mkjudgug.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zxykggxn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gyzrfbwn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mzgehajo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnnjztpq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uilozguq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ggehbjpj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3wdybqpmf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fiujenca.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vowwyqog.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tkdxrrkx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3steokpnt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3klanhyvo.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ruyqbuvz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jgojznqu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mwagwzhh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fdpnbhuj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yuzahxby.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fpgbvhwl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uwidkcfs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nnlaxszi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mtnjtbio.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zszigftu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmiuwvh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ogxhtzrz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3szxfubdb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hciuebib.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwoyazbh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3csnqlnal.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rnrmvptd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jwnvwrqs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3tilxqmdx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xuumurcf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jcyrgzuk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fyeqgvwh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3iexuapcn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xcojcsnt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fkmtqoea.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xeuekzlw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3fibjbnak.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iittismd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iudcrafx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpuclnvy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wgpprdoc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ewxeqeaa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cttuevih.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3knmvkivh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bepwnite.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xxviorxb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezliwuzp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xkdbepwk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xchzpfvk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3siwebvfg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3juqsmskn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cgbegbhn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bagnquix.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dcseogbi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ebwqmhoe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sihqzzra.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3njugqquw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dikbhvuz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3iplqsbje.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bulmtlzj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ipghiafo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3egpncqgj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3edsuzenm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eifekatk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onweleik.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cpgcochd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3famcyucj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rizosquw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgtqqmcc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3aqmtcmjw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wopkgdno.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nkeigmhe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rgtghzza.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3aeinsrtw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jfpzfnkc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3pwacglun.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oknyfhqc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wnkcjwmc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hptjqczg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzdnjbxf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3werldkir.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3efcgtvwm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qwfdxhec.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vuqredzt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3heqrhecl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3wflnjqgr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zfgrcksu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rhdffyho.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lfmohiyx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nrzsamhw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzynrcmt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3oigrvqsm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jhcjleyj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jfekmprk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3sybvibeb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3avcdjyhs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rwxbzvyj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3fntasyvh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ucmjropb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ysijtppq.html


<!-- 参考信息 -->