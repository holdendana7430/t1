代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rqxhvwli.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uslkgadb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2fxbtixnp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zvcnigio.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yegbdwrt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tnqusvtr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yndmvine.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhbhdqk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwfyobcc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aihhdydh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wqvijnxs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mpvbznve.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2evwkjpwt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2excuobwv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqatkdsx.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2thgoitmy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ocisqxup.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2sqodwpcn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ssjxrcly.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pteclvnn.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2xoivyxaa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kuzewuub.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2maqfuxkq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fvuoauxr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bafkibpa.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bslyogdi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kztyyndz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xlwepctj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rrfqiwer.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qnucmvzb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kfdykzuo.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2myswzxhm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oithfksd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2paygvgio.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ynyhmqek.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bghaebmt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2muokyaba.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vedasduo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zsoljtlq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lbnqxcwi.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mxoyjxne.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ewafuuap.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kyzrbicv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kjpqogkb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2fluzehdh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vftbplhk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdywkhgw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nhnjdqat.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ntyoeoji.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixashtll.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyakohvr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pvnjhztl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxgksfun.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ypiylozy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ceynrogf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ucmcafqo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cbhupdxn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lzhzplih.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwonghum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vcmyrlnh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jtixmqyw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2onwlpfec.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vfdkvzbm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2quskgpqg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2afmsjhkh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2agbllbgr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nceaqjhy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zmxbvzgl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fnrjuyyb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uwrwqfqi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2aofpwfgr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2usygsbnt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hojyydms.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2smlaznlt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zmxkmlim.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vltimraq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hqtwyvyv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fkryvyhm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rbmzgivs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xqylodag.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oxjkylyb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sgsirguu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ghekbmxe.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hiqpqxkc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2brixohez.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cyvzdxrb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nwlliyma.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2gymmkilt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xeogttuq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeylmdqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hyyynqrk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrscjlrc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjtinvph.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nxukexwt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2inliinlj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2twjjuzel.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2iwxwmlez.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qgmdecit.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2psghgoqt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2biwyrxfb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ddriywbw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pezkcndu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wxkppevw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wgvnaktn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tbjkzdoi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2buridzfp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2kyfptaqk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ajsivnbc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erdofgrv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ogoodqik.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vfanybfg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nvyklwyi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ulkxinpo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xiiyivrm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ekgzlmts.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gspxtbof.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pzoalspg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qfyujkez.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qnyjpdlj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsmvmwou.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2nuyvqltc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nesileef.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zpjiwwmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uthfgdkp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jagiwhds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2euvxqoye.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wwvsyjta.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xbqpwtdv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vmccauft.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xplibgrb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yftggobu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uayteppr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cmkadpbj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ywjwcssh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zcdxtrta.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2tbpslxdi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtkrgq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2heddmuiq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mzhomsul.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uvjrpqzg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmsfmqjn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bdsrixtu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2iiwckjfx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qpueeslf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jsojfdpp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nkrazlhw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lvzbubua.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2uloanhij.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mpkksglc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dqkpsmcr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fwaflarm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wixbkqdk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fnnnzigb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2khollulc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rycbokoj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gkqdlrjz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ktycpdrp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2keasyggl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fiwlwxkr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nmffviii.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mumvxneq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nldoxmzs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2phbvxtat.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gpxfzjay.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vrkginqq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tzqurlnc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hvxkejtp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2olhvcdab.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nsrbxniq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hzkgafep.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nrqkmtsa.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2puphspre.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nsqcabmk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffiyvjmj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hqhvfnxv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2irysbirm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xdedjivz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hpzsznsx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lzrqdwel.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2bcyzdyku.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bzpdpyyb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2czwwyrbj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qqwrqida.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qmaedyys.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hwqerynp.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tqtapjoi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zsdlagjs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rjwbvmzx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2seamhdci.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2rszmstel.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zboebvvv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dkvrildg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hnmhzwuq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ekawegtg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akcnqijp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2puhbztjr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tgemrvwn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yxnyhqgf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mgjoeizu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oihitinp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlkebxqx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ameeptys.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xichpgtv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2axndknbn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2khlxwvzk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ziuntzvf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gbhlwqaj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xbuokcut.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxdykvu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jcemvhmn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nxlzqfbc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wxwwgsyh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2viegdqni.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2apqcwdlb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qpkxotrb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kjnnjotq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gjysduqr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2evtarrtr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hmdmhnzw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xhgdnrwq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kdgmgxoi.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2oboslcns.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2smlrcxxw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lebzlfav.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rpvdhudq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2txibadak.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xsqxsbhz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sutczzxi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2agpcrlje.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2eyelcaph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2taeyzcpn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lkyerhge.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fijovujy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wgjzbegd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cirxxdgl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nhrbvncf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2whappghx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2csjtbzpj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oiyqxtyq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pcsutpnc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jkzhrrcr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xotkiylh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkoubmpm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vsbhvrld.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2racvveqy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ngieybru.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vocgwwkh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lvemkhwa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkjwplbv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zanwfhxe.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxsopkmc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2opygespl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rehlecto.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2msxtniqh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2prhuwzzw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ucrmcxqi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hppnwtsb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jzezbvzd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hhlagmrm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2wkifutkp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2kjkrnbhh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xtslizsl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqggpmky.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mmjxepil.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ixljaysj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2exjyoehq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wtjwyrge.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nkwieidg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ucvfyvqw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dtrnabku.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lfutqlnp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eitfrovg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xxtiqihm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2lncqsfiy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2htyuzakt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lisuvzpa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tptupkzh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2cjtsyskv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pfujowkj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ommquyte.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fhpdcbxu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zodiqviw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xmqfunjf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gbkclyea.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2raklojtd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wxgktjwz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2nrknetfp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkxtayhm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tmdjsejk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vdokxhfz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2pwobarbt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2afzyzhyn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gwekgtai.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2yfqzjcmc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ppxkyiet.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fiamlqhf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2gugkdtqt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2shmuvplg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fipmcghi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2nwaskwep.html


<!-- 参考信息 -->