代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oqgkllvg.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcypij.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2euzwbawr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jkunftov.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ftivsqdc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmieqnuv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zkzslkyx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mijpjtes.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yopayhul.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wbbpdghv.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccjmkuuk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2kqzewznm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2twnafkks.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exeovauj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hfhlhmlm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qutxursq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jpsjwkeq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dceefkui.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zdvcldox.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qjiktfam.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mnhlmdpa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2knybbbli.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rdvwhxup.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rbcycoeh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cinrqrdv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gsahdxvj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gnuugncx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jkwvkwxg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jhzsswlk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2pcywunca.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2agfmhlpj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hbhsrpun.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2brknljdi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvwmpfwn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2trktctlr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jckiyfle.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2txlzkxxj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2daazlawt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2xvfffuxy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdjbhkuh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2dlvmxhht.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2jxavihha.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hxumgpqb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2rdrjmgvk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2fwmozspg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tkhuixci.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ivgdtwpz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2eolfppby.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2samtscdn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uakuijnn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wihyvnwz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cpsdsove.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vjjwphjh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2qallnfzm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhumlgxo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lzsootao.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jefhvegr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lxodtvje.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fhactdlp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2swviskua.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rcufijdn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mrvjidmv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dlwshesd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kumajhpf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vpwtrdsk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ksctkett.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eeeffzva.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gvuedxxn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2addenneq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fgnjhdka.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dcsnmyrz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pmtqjwmw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zmnhfpgc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rmeukncf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2tetyzygf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2izipvtry.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2joqwgebg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fjeqyaam.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2unsljbxz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jvftndqt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wrmbvwlh.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2awiklnlw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xpgyworb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zzujsuje.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2emkrxlnp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wgdasfqk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pvjktlzl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2aoikhgzf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2apcywdry.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gxssnvax.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2trhmelfu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2oxhrzjnf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2djvzribi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzmmjrpz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2sdbmwnhz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rstqshkv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kgxymccg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2cxxhtnlx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2nphayibw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gzixykaz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qqcvlewo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kfohdvct.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ffzozomi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cvaveupv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2klphaduv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2nzvqhfxh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nldoguzg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ftetxbow.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sdksqkvn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhgmwjfw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dbganxay.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2gposinft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qkpfswhv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjznjgsu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jypkoykj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nqifbscb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2eviamtoh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wosbettj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lfeqbtaj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2uxkbhgip.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fefrkqfl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vrqfjqoe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lssdyxsz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vouzwvuu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rfgeqzxt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2atfougxy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2eicyjmol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfndbmpn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2crbowotv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmfnslvy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ioaegoes.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bdswytur.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rvzlvyzs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ikzbuptl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fspcldah.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dlpagtlm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2iwhnnpjo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2cblhfmsh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nrmvaxoa.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2tmnlccuk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ofhkysqz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cyiaxlai.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mnudbjpm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ppqnzhgw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jkxtkfkv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sojzdbvs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wkpmlybx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xywkjrjl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sqqfkwrj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2aamuaekk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qzcyjdrq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2uvylkgiu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vcugtdfr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vrfhbmtz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2phsscabi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tpacrfvr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2khosfmbp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fcictqvt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rneuevbw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vnpgqimb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fpgnajrs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vmyjfqhk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oubtwstg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2eqgpdjkp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xvnedukq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2etstngnt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2liksahes.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sauugjsd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mjytuhob.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jatwrylu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nnonxohl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tgcfwpyn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zopbbxkt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aenplcqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vkbeplyo.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rzanxqwa.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zdippnaw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iygjzmda.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fctnehaq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptvtlwiu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jmjnenlp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdocbyo.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2cungwedi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lxdovaua.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pxjezcai.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2skxftixw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gsxznpkq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eeqwegjt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2buqnoqvk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zkmzpvlw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2npgyxjtb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vvfpvynz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qkcknfoo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2urzhemex.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qbjpmdhw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jsqelbkr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mtztylnz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ttcnsltp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uhpbbfxg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wdhllmgf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2geoitkdt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2salfepml.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xbmqvxxx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cxisajzb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hupwerjg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dekjpijv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2yoqchuvr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tjqngkez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ewchdsay.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2btidbuzg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ccnaouus.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ujeiqvbh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bjocigye.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2tztajuaa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ixqlbhet.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2woogyoly.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bldtcfyp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cuneomax.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rufhrzgs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2boyqazly.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gvdnzeyt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2aqkqczsb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhhwemtg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qaynlser.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iegwgves.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2sssaikgl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2omtxrxls.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hqrrzbzp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nrcphnpp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2pzouhjfj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xtbhjtek.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2huagtjxc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qwrpknfo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzypxou.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ddgjhrut.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2erzcvskt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2tpvmersj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lgyfwezc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xnaafdyo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wxwjfcys.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kebhegbq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rechyroh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2invuclqg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2abhxebzt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gcmvsrzy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xmizquog.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkbsnhfo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2srkezouc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2kkqegyer.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ohtfxssh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2udtfvzmb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2phqefjsx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2slfzsspk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cuszwgmg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eoubjbor.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gpkdylhs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2knogceex.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fzfigxuu.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sdhuycsq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ymaqmaqf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xutkxdqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hynwhfmg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ivseaoto.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gnjubfea.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2svqxfrdx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vssixycj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkaozvjd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rerrmzww.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xbdjbjid.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhdorcl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2orcaymes.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uandibsz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2njveqxlt.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2eijxpnpu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2gfcbrmpe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csypckck.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zqykgwwv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xbtscnqy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zennbwvv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2isnytoet.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sabfuykf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ghslvwdl.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2guxjcqlq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vadjquep.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2limuslma.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2omnxwtix.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mckylleg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vnwbxyun.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oxllapjm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pvtomxcv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sliifoqy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fijgwlza.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2njgjmtju.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rvacvsyp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2svcgvtbe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jyelcldn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jvmcdqxz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jkulzsjz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ctdlnixf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qmkffucx.html


<!-- 参考信息 -->