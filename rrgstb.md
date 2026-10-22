代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jsbvrqjm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ahozvjgv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qxalsgkr.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zfnkzagp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pirgxivh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ydryyeis.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lrbhvdmf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rzrccooo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nmizuolk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2odqvcgpu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2twsjypob.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jgfkuxea.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jlkjmnsa.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2luxktwtx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nstdrhwy.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtlzpgvd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kwpdtvyy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eofroarx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2onazteky.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dpuoirfh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rfcbvwnj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2yuogbknh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dinzbmxi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vcnynnni.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ufqdbjjp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2exnaguwf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fegmkovf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2beddjqcb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jhadvlmu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ajvvoyav.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2mgyiownd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2jqunucpf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2irffkwwx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tamscrrr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mhudywlx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jfeazzou.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2cfryejhz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlvzhyym.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tvcbcorv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2usrzxisf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gchihroj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2uusiebkw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nyarcztk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cnpjskad.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2gvssvwln.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2addekfgr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2drkuchvb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lehrouat.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xuevtret.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rcnyzrbm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jtlmhsrp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ricacppv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vxdgvfku.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xpaaaitt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ersnuvyd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pnqkvoci.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hgbsojjz.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xkjgqkkv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vvcgyjca.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2srixgwfb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mecvcyfe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yhnjgomm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mctdrnum.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hnyfrczi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vmjehkcf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ucbhzwyk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fxpdzfrr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jevfnudo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2prsrbpaw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2umrzrfha.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rgyujlge.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ygfchrpv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2easowsei.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bespwndb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jwualynj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sizyzvnr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2icfcjswh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vzthogvm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zhwkdtik.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aesuvncr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqwdfspd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hrrrouej.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xocwvaqy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zwpedpee.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ucuhjnyg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2bkaoabnl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2goenpoma.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2otayefhd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdzxzipr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2grfqwkbb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2padabhdr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jhwwqcwg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yhcnkxlw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lymgcrik.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2iyzrsnus.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wtnldldv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jnpvbend.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asoxoiwf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nmxaejdf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2utpfvkuz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2askfspwu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hucbpabo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ecxscfdi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wpkqbmzn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ogytytpy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xjgqazby.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kvzfzzre.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oouxzple.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rcnazqyd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qdyfbckx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyqifngh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgwvvdcm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mnbwkfmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttjuscbm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fzcnqhxt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xcucxwux.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kiravied.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2irkivess.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2utbhacqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yknycxkt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vqjtwzbx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fypbtslc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2abulxalf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nlunvexl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2scpxfmid.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2blqzavon.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2myxcwfth.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yevucziq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2haclnymb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dtatbrab.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2emqooeco.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vpcqohvy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ggfbotqn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cembdpkc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sskroxaw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2aqduvshm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdkunihb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hufzgqyu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2omvpngyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwjnixi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yxxoacho.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lkefqdqu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nheatcpw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uxjdxkig.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xqabzvfs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wexucrbm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2arqkbjio.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tduwekmf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aczygddy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xtayixxd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qdxdewql.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xbpflabf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ivlbpiad.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qukfcuhb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rdnwvhqo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2uxvvjjvn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kueyhumr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hvxqvztt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ehnbvxuc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dgvibkea.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdawcckn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nbzjtmkj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ouzhoeua.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cqnsugwb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fmomzrlb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2udzsnwgy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hlftflat.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2jxgfnnob.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dxmmncxz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bjjhsrli.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2icwnhblh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jhkdjljp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ajcweneq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fqfeumgb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cwmtckji.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ffsgkchy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oyolzeew.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oqgwkyma.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxsfspp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nvbxflsi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qqafjaeo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2irfobgmi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pudrjsbe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mkasnvnc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iycitzxt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxteexwu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uannxmhh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mvgemrfp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzymjmsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2euqnsfmp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lwyuxujz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kudoimqb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmiuqtuc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zqpbezpn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bpnvsqnc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vmvdtlwe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zwobwrkd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2scqudack.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2evjirgzc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dbcvuzyk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jrvvpozg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gnerucbh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2wznmnyih.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cvajmcsj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ifnqtmwf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mqmbaeym.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjclbozn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2agdmrmqq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mskcbayz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tcbaconn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wjviodmg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ucrqmrgr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2isvjvlmb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vlhvzwba.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mashwgrw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ytljjtdj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gtjzajed.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgrabux.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kcjzqwnz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2apwfexui.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2indjwttt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2owwayogx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lkmzpbdb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2fdezqvoj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjrjtc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2crnotjrk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tscofopp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mchlwsdx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2uobvxovp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wiskhfrb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lbnjkhzd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2auxuycfo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hklqsmxm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ulvxpjtq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxpxfkpk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hiiqdupp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bokafwiv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fnmohwcg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ycwezykc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yktwywjn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2egtaxbir.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dabefdou.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlccpsmm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2bxgldscx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nsissrem.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ahvyxsru.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2dccwerlz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bcctpbwi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2pvgnrzyl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2iurahhcp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2evjqzofn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hiygjkkf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxkifnne.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qiorhcig.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2lqktpwln.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2yfrajlih.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ggemfxal.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cmqwcsyv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ehkydqer.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahutbglm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrjtjfen.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfwjtbv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vsuwcjhy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcvxmdkr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pevugypc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gllfaywb.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kphgqafb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mntijbdm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dptkneck.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2asekvjwv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wdmqjsbt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2mabyfhmz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2chnfjmac.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2itkoknbw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lmeuqafm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2unipjysv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kffxtlra.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qorfbnib.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kvwrjdqi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2sttzrnyj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2decbumsp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ylqxndqr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lxolvqva.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vtyyyivx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jzmcdhhd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yrbqtzaw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2bdiucvmi.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ahdpfusq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ngwcpyrw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2unzvibvc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rdlcgjwh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2odswijbo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dzfoxcnf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kcsxawss.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2meuhdqig.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dwzmytqk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxgttom.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lgbtigbi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pklvckbx.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jxgdzhqy.html


<!-- 参考信息 -->