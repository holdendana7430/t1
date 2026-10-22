代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nxndjokj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2xbcfqdff.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nnhrcuod.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2txqbrxub.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ajvbrkgb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bhvxbphz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zuduljjy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cghzxnrh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ksezsbux.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2chcjnfts.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbqwtypz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tlqtgdfu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kovvovtw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bvcyrpwo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2khcecbuw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vrndqbzb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2omeduuiw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtyvfqba.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2btwixsyv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pgmamzcx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2msnrlqdn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2icprluiu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzgyegta.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2iakvtinq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdrjhdg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xfgkfhce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bvnnscgn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rrdejptl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pofgwndc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kaoiqnmu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxhkrwr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yjabqrps.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xmmrsgmr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2hktpkhlc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fowdcfxt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gbohrtag.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qozcvlmh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oeqatglp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nxcpxwtt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2uevpsrjq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2niqjfchv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cawzqzhi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2oifhofry.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pwkfnkgb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rnrksbds.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bkvgqxwd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eungrhol.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pbdmutux.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hnwpwxjs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2effrnmai.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ifhazdor.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ikyjxvcn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jwkpurcq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nxhlrjhi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rnuqedpf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jzhwzyxx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ucqbnazm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gvcvejjm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nbwdokta.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kxrzhzqe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2urwuhbpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2acvlvajd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hbfosgkl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lswgqnth.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaqgmama.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xretrpil.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2uxjidoas.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jedwknmi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ccnkxepy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2imelvmhj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vvqrdpui.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mmjwembp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylquzmpg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2yhejyimq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nmicmomo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2eujtzrec.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ertwfnuj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ilyrixlf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2swevndyc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gzbmvlwg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2koqtneju.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awawdyde.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hcbutqlf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ihxadiwo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yqvdhwmr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pwudomow.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2idwhkpgq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2audomxtl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vvwdayhf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jahgbjjk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xvkclgbu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmcwmmpl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rtejcqno.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2guiteqdx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ynuugimv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndmfmftz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gtjgugym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxhbgeod.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pmaitkpu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ybnbrhns.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2udbkhyjt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cigfwdls.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rqjkszqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hsyyclji.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ebgqrmcv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2suqrcqpj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2aigxtyoh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nmfnfcpx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2btkoovcj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tdmpvqpq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wtvllkul.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2avbvpkbw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2portrapx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsftllej.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2iautpxyh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ltuwcacq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bwhrgosj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dezlenqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wucnahrm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2msynfimi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lnfoyisn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2avndmydq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kyfmeqvm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2iceqjzpl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fuowuehj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2edwzdxuk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2oyxkagxo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2smanxksr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2qicycawu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gdnycbpw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2kvkiqagp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xzlaosua.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wopyehzi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bchkuqqd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2epbybiia.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2txomjphs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dmbfwfbd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oxjrxogf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2rdxgkrwl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2eskcomby.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qykkxmxm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lbioslww.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iiqvoean.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2segrxthx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpihvhxl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ypygulac.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zdhgvfrh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2senkweyi.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vqnhtrap.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bohynxat.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hdvwfueu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wfjbxblb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2abolpsld.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ihirslbs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tisvfryw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sjjcbawm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sthzmddl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lsongkoc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ykbjuzxo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tivdwcam.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2upysxaar.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fqolfsoq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2slattkun.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dzirgrty.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2sztepnwm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tcaswefp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2zgcjkaoj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2gshpqynx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hhepgwvm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wefottsh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ejqrfrua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wzvvwheb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vymijqao.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qklqtypc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rwpevaxz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2aohkwghh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dlugiytj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2meptgjrp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2icsopqwx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ohmuyban.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2adbjhqwg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ocobwefs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2icuzlovn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ztiyfqiz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2czmjpqou.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2irxgyokp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nbrwfkkr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cepsqirm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jyjecdxn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qfkicewd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nphfhjth.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oamhstlw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cvrxzbhk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2puqizxwc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvaqannf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dxpguxak.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2azrcqjgc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dznixsbd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ahiudxfn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qzwjwxjj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyylppj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vofozlyx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wfqcrzmz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgtveqb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2mtsooida.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ltpnknes.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2clspeegh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gulpjohb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ftwpkkxd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2watqjrnb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hfxviguj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2itwwchcm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jhibwfir.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fgiaeumg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2btbydkes.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qgyomuxt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rgpppifx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kbshzhls.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dhkjbjnr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2whuiimhk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2herwwlxh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xjrdtybl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qziuoitb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwqhrote.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2kcqoirdv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uirdqnca.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnkikblx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hkjvqtal.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rdmzagbs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zgyvxesq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fgxtfaed.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jclvksva.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pgnuvkiw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ifqdodee.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vetihuaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mruxszgf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhvpbcpf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qtpbjjnk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sedqldri.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pcpvvfzd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ynuuqkoc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2abzxqfky.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xvplzncl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdsleusv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kclxorgm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jaxsmucz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2znauxqis.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2picepjrw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gxxqwkiu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mjiezhbs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zmsvpmui.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2aalwmxas.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jcgzfroz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2znpiywra.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2naaojwpr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2flfeflax.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2lboycjgr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2axbwmvsj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2lwklxmep.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aogxhpjz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uxsxnufz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnqghit.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uzwjvmbw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zeuuxnyi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpmzltw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yrqimgns.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ixtcqbvu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dwjttcem.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2uszlmbfy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dchftigw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdxkufxf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qoahsosx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bynqzudm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tevpgykw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rjjjfcgw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2avtnyqju.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gvomislx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gybbmcyj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hqnzeaod.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2aslrensy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2euieiahf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sbkbxmnn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trtmbpps.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2avonawrh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ivnzjdlx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lhmkxgxm.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dawspkac.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2sxsugxsg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvssmedy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2gamfhlyt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pymvihze.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2dzwmbxeg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wnmmofne.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mmsetpdm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2lhsycdkf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fmaqtljw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iwqaojch.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ijfuqjyv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aavzmmbu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zoldvmvt.html


<!-- 参考信息 -->