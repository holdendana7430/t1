代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3xjfewqqv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bfncjdke.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3pksfxlry.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3evmcgihv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3daugxovq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyklsooj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3eebmqune.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ydkuhulg.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3zajlryst.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3poeusbeb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kemhtsoa.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3njrhckha.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pawsazni.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ahpqjfyu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3nzzcfcva.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3klmlwkmc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3voestfyq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qdklljzb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3likubnkd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3bcbqyabn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qjmfqmhi.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ltmwoefs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xzskozyu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lfcdfiam.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rbnnpztz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3jpnlbcss.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3bymlfyhe.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nzdhpvgc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qrjykbxg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3misavksm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3leevllfc.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zmpkykfr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3iskjgels.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3etvsygcv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3xiloxhvk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fyfvkjgo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ckmqlmoj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qofubrem.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kojpqwah.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hxsnmmyn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3etsdtuay.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3isfnmyqt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebagejwl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yyzpmgkm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xtyecekf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qfvddfoz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3lnotowau.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3cjhkqoel.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhiqsimd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdetnuhg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kiwkzzqi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yoygtjbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvjbbgrh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3drqtwyoo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rvwjpwjv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lwpjmlix.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3anhayciq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kumdzsso.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uivixegi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgdgstki.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xvbnzztn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lkxnodim.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vmlioiqt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3iphdgxvb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3upkqfkmw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cbprtwht.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3diesipwo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ympdyraa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3zhcxxsso.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jmpntwui.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fnhxbwye.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3sufuiaxd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ilnxptrm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uqmrewqd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bxrmtjee.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fbripfvk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3suylykqu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3acvzmfor.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ouwztfqr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rnrgqwbn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ledxqguq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ivsgbcur.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzgphteq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3htzqjxvb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nhadyeur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sgvttlzc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gxophqqb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3anqpblrd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hdqufgdw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fxtpfsqu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bgdpkqew.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gpbonebx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uwcxquvl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sgptotyp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3apurgric.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vmokdysx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jqxgtlse.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3pnjuhqcd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3psoffpdx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hepisify.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3yoosbyla.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zfvzkovg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kpffbzlr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uswsgwvv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lnkzirla.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3invrnift.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3udmirwck.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eetqcyoi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3oxqtbemh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dvthkisj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ujshnaxh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kevdrmfj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gbkxfmyx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3gonuqqbw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3eboxgopc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3bzkuxsus.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3wkhafylm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbnejphl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3wisorkok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eeozgbwj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xubdsghd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfdytvsq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sarvewjn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3datpfgbb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3evjmible.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ywtdwrjc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kfgzqecu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vdwavuga.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ezalpgsj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kzxpadmf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jhpxivhh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ktmfaobw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3juelrnjv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3wxhseigr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qvygygix.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vwsaziyf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3juxdwwhq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ufvjnaow.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yhqwquah.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kpunplzs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gmaolupu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zfespbdk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3yhgvfohm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3slxzjnhy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sddgylwl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kvxkrhhi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lbrtjjaq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3djwabynl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qeenoyce.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3npffzcui.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uthivpbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gufomlqj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ovdkyltg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mhgdppsw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjoypw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3kjlemxpb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iikehllh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3hwwgqdeb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3easjzisd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3oyveeyxl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zlzaivvf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sezeleda.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vvkqbsqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3scrqaqfe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vbhnuuro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eztbvojs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3grbdnrqm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3usamohjc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xrzysshf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qsefrqsa.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dnomgtim.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dsprnavr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3eqtelfln.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdarrhzu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nuvtscmi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dqdwoxzd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3oicrdtfr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3jhgrjugm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3negedatp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yyserbeg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3obgrzqiv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nthiavtf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xbkpxzwm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cblptbjb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pucvslyh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wouxcubw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rgwjcmip.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hsegusax.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3pmskwwuu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hzrgldrv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gaouvaix.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gdccwzlk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zgulqzjc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nuvkjote.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3dxchiwlr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3abepgulo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3roulekdy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ctzydrfa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wjrjqjfb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3cvjnfxyj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ycfujpgz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljiykhbt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lskcqrzr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gmzqtflt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bsdmqdas.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ycsktink.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wmevwnzm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gfizmmlo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cdkewytc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oeaelhno.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nzudfzyg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3guwrzicq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wgnoevqs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nqiuzvhl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xsenklpq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3fpafyakk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3prxaomcb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tpdjoudj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3llfsfgkz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3kqrmdnaq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uwbolhfg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3khzwatei.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tkhfoiha.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qgjnxfpd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bttgvmkk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jweuozfz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3asrvitmr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uksqbnie.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3numqaxwn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3upkharjg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3aehjokao.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nfprhfvm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fdwtonxk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gaxravrv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hikjchom.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjwpteju.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3nkrqitgn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ujhvymut.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlecutue.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ecosxgpa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gfrjdkqw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ygdocjsm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3bcjsmcjs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nrqfgiay.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3osvmwipi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3quppdzjo.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qlyoyils.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gsioalvf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xdkdhzue.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hznrwoff.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3toyucnwc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3crzapxmp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qhdrhwrr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mvagfabl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3wqiikjzm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ymbjdnnd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wmxlpqva.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tnyorhko.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jyneacdf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lrdssnlq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nqvblysy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3szwuazwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nekvhceu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3okskcnwh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ucouwhen.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3utibuimi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzrbfk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3eprkkjlq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydqwylip.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xrzadlsr.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3euradgqe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kuviwqpq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjlsbpef.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3sovrdddo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wwizzecz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dqwbhocz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lhwzeugo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hfftwpcq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvjstnz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3fqgrehlc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqzonfcv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bgwcpjzp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jhjuaxnj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vktvzkig.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3gyzflxki.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfstgemg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3etnkxjnc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3fxinexdq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gagilxog.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3rezdgbyf.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3blxkourh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nbpumeqw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3qxssifsf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yaquvptb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkyulfv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dqseonth.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cacjbqeb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vawcpyyu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3retudtej.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cmtjodya.html


<!-- 参考信息 -->