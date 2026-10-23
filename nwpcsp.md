代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ivojrjjr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3sumnbokz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3bkfdshoy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3bglcmrhz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ixpvdrrc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyerhyvs.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3krxjmrcb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3drixdvvl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3oxkvukqj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3tieufowu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3llnreorn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzybycg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ekojryro.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dbfrxkag.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3knxbpyjb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yzkwplaw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ntjhpwdt.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gapuuzxv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oesmqick.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3crbaxdhb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rodmivrm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tpawnalx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fidpjerw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tjqivjak.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3unnuexgl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lwaqwrde.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vrhjcgab.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3veiyckld.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ytiqofji.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3naapwlih.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ergaxpvu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jaltqlmw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3diwxzxgd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rmbmlgsw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lorusbub.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xjcotanj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yudqimkw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ljufsgsg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rpsaesfw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kslsdckw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3fuloexay.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxvacus.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3rktydmbj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nnoltytx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ihejqkoo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ybtlobvf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zorztnjq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rwcrvpnt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3uiyphtnz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwoobiiu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mupgkvki.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ilpvlnfd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hhkipyqt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3enruyhrp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zodvtdjt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gxbpajlp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dvawizdb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uilsccpa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lkdefdfd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xisalums.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjyteiyo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ydhunmdv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fttpgnrc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mfvpsfrl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xfiazmqn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3okvyymbc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vlzpwhbn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pwohjujr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3uavognmk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3icoxvnww.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3usnrngyo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3whatlfae.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qkmnyqpj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3hrrkxynk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3qawtffam.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cxxievpw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ppivcodm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bcgbchbv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vxpwburs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3offsmzbe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mxuofrix.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sdrtwtky.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3wigxhlvz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3htfbejhb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vllifxoi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3uenvevyt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3isursnys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dzrfjfpf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3galllviw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3koyvenao.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqkeexie.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3riwjkhll.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3utpqnlwt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxqdqkyi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3golnwqgm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lmfmnzco.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfytazci.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fnbaufyu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bmhkmuih.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3uabmjoll.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzhorfsk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pxrkbmar.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fvyxpgve.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3haoqaadc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekrtwtvq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jgfpotfa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hffcwjyx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3giwnsbrf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3aguexvih.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ftcrqyvp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3raiosxwt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cemgeqvi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ohyhhgyu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhvkeajj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vaurqyvv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pkjuwxmh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dehcfagb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hhcwarwo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3qsybbkiw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3knsupryx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ymxkvkhb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mstpltsz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zofrbitk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwugfecr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rmhktlrt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sapmumvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjywbttn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwuthlay.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pyubpdpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwpafvin.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qmczxpof.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3navdswfj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gefjzjhk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zafcmuzk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mitncmvi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wslrzodo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3btilwgyz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ynkwlmnv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xupzvyho.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3tbhghgsh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pscibwlq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mggtrcgm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3oohknslm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lviltbrz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3tjwyxgbi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xkrlvcpg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxczmcf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cvwgmheb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gfewbxws.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqhdwprs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvzdbac.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rezbdppm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rjrlahax.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nufiesjc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ixrvtctw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eizfzaxi.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wrkdeuvx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3stdtpdqc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qhonjpyt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fxvbweqv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3wuuezygw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3drptywtk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ohagxnay.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dzfnpabx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gknrmjko.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pusdkqrg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktbhnqpk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pzhlourv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wxghoybs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nixaebmi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dbutvvro.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wphdppeh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tuxqqqwk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rcnwgxdb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lruottsu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rzhchiuq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3voryrulc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fquuyyev.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3onlvgjcn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3byjvxqlj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ufhsttlk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhfvgntm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bjxjuoyq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qrcmugsn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3isoqojzh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eluhpzmo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwzzwkrs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3onuxahen.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iwvwfymk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mkmhdwpv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rrkmiaua.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vmmamojo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qvamrpro.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3owljsinh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lyorcdgi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3pitefqmr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3osbwpwai.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hvhcsupc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3koxaxycj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qeutjeev.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zcmjzelf.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ertnphyv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3olyktsxy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zfcinyqf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtrpzimi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3oknqsdyg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3bzdyauyq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vdsdrshw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tdqmrija.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bbrukgvg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3xkxptbzc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cmuhembi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxlvusz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vxnywsxo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3izpkwtat.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3fgqesebw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3nepqrvfn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3yvmephrz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gmfzgbjr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pcdainbb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ntmnrnrl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3necjspro.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjyvjtnv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3tvymfyko.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3uocohryg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3airwmahk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlkrsbyv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cqafwpyr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ggrcvhdl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pjxttoaa.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3oonfwueq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hovamgrq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3josdqyxk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3horxrnky.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3fxrxfsmj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3abkkkxjl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3vknfbvls.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yuxzxvox.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zwrbbrmk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3xyurnfuf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uxrktolf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hwfvakde.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dajsmdlz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwxucpte.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vjjfhyvd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3cliiwkzp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ixofbtrp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3swubvqsa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xeclnbqu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ultdjryw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jktjdffo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adeoorak.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vpzavpih.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lfeaptjw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mkouhotq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hpsgvcru.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kvpiunvo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ldjpbrjy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jgdpvjuy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hdknosag.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ugpdbxoz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xezgaejg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yiyuxxde.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3szwvoysp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zvsvoawb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gqzngxit.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ublkjrvr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rwxlqzdz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jncuowow.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ydqkggrz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kzqbavxk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3oehrinbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hprhwzuk.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3tgscttka.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wxpfhjse.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3obogrjdd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ifvmorkt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3vwmbewnt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cguzucut.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3guteougu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rhhbtqlm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3xfcdoews.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zhtimhpa.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kmwrrrzb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3kilwymtd.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pvypfihu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdknpy.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ticihiih.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oeybhczp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tbxcaolm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3shjlkbct.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pneyhtuk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wqgroqoa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yrunnlnm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qcnxynkx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3evhgrera.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zpuzczvv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3otqiilqs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3geiletrq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3zqpnotgv.html


<!-- 参考信息 -->