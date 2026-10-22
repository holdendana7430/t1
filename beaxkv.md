代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lazziwju.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfpqemsb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmaabfdn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2tyqokppl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zuqghrcw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pyzpmxgp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2otbldyac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2lutlshqb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xcjyrsym.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vmclpesa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2rblbhtmn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2iudkyawp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hcmtkkzg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wigljnnc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sslhxxxq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ywzdjkus.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nbefckco.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2jvabskxm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iotifndk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wxgehzpj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rbzbtfto.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iifqbmvp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wzpjcogx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zsknovam.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cgemhtsp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tsrrmjbg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2kwtbdsib.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yztsfxuq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vrswbnav.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2avvknvyr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2fydtqujb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dggrkdox.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ljepbzmu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tutfrrpg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2oubtjwcg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybhbgntx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qrurkclk.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dhcpezfj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2orevlrnx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2iszdcrga.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhgrkkh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jrooszar.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2rfxbseql.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hfmbyuxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2swykjxhn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwfveyeo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2leahengo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tdtgihey.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uswdfmfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jcesdqep.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyghfcqt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2dnafyddd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2regxzomv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jrdrzkzx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mbetibzg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ytijizxd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tssshbsk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ceqdifnk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vavjyjfi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bftpimqr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aeltzwid.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2imzvrnva.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uivfefmp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uetfstmx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gfihfqpd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2osflqxok.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nweshrjl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2utsismxm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dwxxznqz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uvfolvmc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wkwjfwtc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qbspelrg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fakjaxqb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hsjfwhyh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2odakjwbg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uoqbhxhn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tttjumtb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qsncuycc.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tjnkrdys.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ngnaqtks.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pdweuxza.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pbhghwcx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wdkawtbp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yqmczumc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2imvitpon.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lugeymnm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2cppwvawo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ryeqrcgx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2revsvyts.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrligdvr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ztawakth.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vgkapqym.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gontpnfu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2knmkbhhl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dmyyqkxa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kvkcciev.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wfcjejla.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2nhbnfhwj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tymxrzrm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2htyeweye.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsrwnawq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2oazimnoc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2sbxoonqd.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nkknkjif.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qhcsjrhc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sumiscwe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kjpbihmx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2sowuvvii.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwjiqkqc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlrbxofk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xqvtwidd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ecgnmojb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qzioslgu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2budaenss.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fthdreas.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2pjjbzpfp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qcnixknz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ghyzcuhv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2reynqyzj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjlxwusc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jtadkheb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qkrrqqlj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lfwotvpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdqllpud.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ljswshmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbybowmr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rsaqcmmk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2quulkteb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nlybwjrv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kugokqfa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2olsqammg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wepdiziy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2flbznxpl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ildnskjp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gjlnappp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yfyvzlms.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2jtyfufpo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rdrtohmx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbffwrc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2luytnqxi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ykhkqgru.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tacnflfp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2iequuikr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jlwfdnno.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wvlynycx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qabyhosf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tunqcnvn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bodvcqcx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uymnnxqc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2otbnista.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2laeeyqll.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jmyybsbf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oazxkhdi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvvvemvl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2adakbars.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2amsedfrq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2sartbfxs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wgcdakmk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nvgknkdn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ntysjdmf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ylhcurwr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ojfwhwqn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bpmppfor.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qfpenrhx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vfahflxy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ddukpeuo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iyikxwgt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xnutothy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mzuxdtyp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vfudxkhj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2peldfhqd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hxlgutgt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cubindch.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fcybtmvu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tlwohoyu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vumadahq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hvzwfabc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ozncucol.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sjykykwy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2apgmrouz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xcwlhapu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vnictxtq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2iatuvyhp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzkulbtd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ygeyifbj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nqsuigxf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ncjetmsv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2txkyxevi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zfcufvnh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cvjuiiyd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jpbtvhgj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rskfofxn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hdfduxox.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ofjmgxds.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhyhfstb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2uyomafxd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhqzype.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iubdvvju.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gbrjsutb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2esciuxht.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2amglezny.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ofgpxkkg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2hwdkcuqd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tsvhavmg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jezdyniq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2riolosys.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qaggcpqd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iuaaonwo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2idjyhbcb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xnsrczrl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ezolyrtq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vocomeoz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nqhuukia.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2rwyibmms.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hamufneg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2abjdravl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xeaseufj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rrvxghqf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vcynppxw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zxzkuahk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dgyvztdg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fwupdltp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wchkxrpm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tomatxxm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2uxyimngf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2pzaaxvna.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hspcanjv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zrfcyffp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rrdgcgws.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yifutdqc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2nmekkamd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tvljjemm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqzasahg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2oxcsioqq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kollvcqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nhixlkjq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ouooauwf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vcfhjagj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hdnpizhx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fptpalpk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xqbotzpq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ckqooinp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbsporcy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2slmyvsvz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2guiztspk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qhpyftbw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jqptjwgh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pxnlggoy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nzwivnhf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lyjzvgio.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhraxpd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdnswzor.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fuoddxrm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rpdghxzk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xmvtejnr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lkjbnown.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2utwchsvf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2enyqxdkx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fpsgfowz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jianwhdr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2acmdqmpd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nqhlmxig.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2czknsbwb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtuydutd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hstsvxpn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2twjssjqy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2oikwbfgz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hhbfawyp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zgnacmlt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nmjezwmu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2srrbqmti.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hojnmhsa.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvfcbonh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xbbsgigv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wohuifga.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jbkzxlhs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjsjsgjq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sjcomhmv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yyopfpxi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2sxlcgddp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zfkgtyof.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gvmfhprb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ovdihxea.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2oemslomp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejkiwohp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wzffwsno.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xlumvhyq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rfrstsce.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2voygyrwa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ajxzauwh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2xorkfzce.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wosecwkw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zdzkjyna.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hzumwfok.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iweviyjf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bawwzcqa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2icaewxng.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2qaeesfuj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gmbybhnd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cjunonec.html


<!-- 参考信息 -->