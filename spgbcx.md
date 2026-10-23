代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvqjmqar.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3emtkrwhn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3bixtwbuu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3omptxoia.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nphxantk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3mxlmfkcr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3upxdqaah.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hspzceqt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3viydtves.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlldjlzh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iwwmfnpm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pcxxqphl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3brcdxcdh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3khyyafou.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bnhrwfwe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ixmckhqs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rkhhegvc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3upafqtei.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3zxelsalr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3uujqfhcp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3kxulhrnw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3iauphjko.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3eqrzanjs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3stzpvfnh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3djeollig.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3qypurkgj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jfuqfrdj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3htaczapx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zljypyuk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qktwwlvi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rnxupugf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3gnaumnho.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3truwdcag.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3gashxtha.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkpazqj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3fwhczkkj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kvaqeptl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lnrfzaby.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qzigawgx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3khyiguel.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ispyevqy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wthjnrrx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fkrczjng.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3aixmodwe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddokuzde.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhngcsfs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ggnrqpda.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3qcyntjpw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvyipsrc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xoivtypr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3msmjztth.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxprxpfk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzgmwzhj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3stsrubse.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3liacjhwh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3thihqpmg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3upvqikug.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ydpvofyg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vpanubrw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nmmqbvbl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3dqyzsmby.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uzlrvvzs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kbwtmdaq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dpcohson.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3nwvqgqqp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mjosycgk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iawqzgeu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ukwucula.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ublvgcsy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vfvcqckj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3khsyaiqa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qibwzfwv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yaohxpni.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ayjzdsxe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kyagtvdw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dgtxkmkl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3hyfknndv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mpyejajl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ssuevybs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wdunsviu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vtsbfrxa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rnoelcqa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3potbtiwb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3kprrayqa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xrodlyuo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gdapnsjv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xutumzlb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3elkdxctk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3evhrntvm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojfzzdwx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3erdvrlvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qzsibqnn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3woiwgnmr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3awzwavhd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ykroyhxv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3fuvcettq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3xcoascoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gtymqxpx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dftwsnvm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xlvvujfn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmtjiqf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3njejmnwv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xrevctxa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3emyqmpue.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3oumgdolg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kbexurjt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qnfuehbk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kcymgcdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ackvcwya.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3usqeygik.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tuhgfxqs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hmhasdob.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3haeqbajf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uevqucfd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3smvfknwb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ekrryoaw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3avpvikki.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xilgfbop.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zbrapazt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnfsivrq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uwiyagwb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ctkdqigj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scjpvvsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uglynwjy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3pzvehyta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqakaaal.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zbockeud.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3tpopxiou.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3npktderh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bwvduscf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dsmbyown.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uoemdjew.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bmjrjfrh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ljqczbtt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vecpqvuf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3rgagnili.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pdkidboy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yocdoctn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rhvjlopn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pnxhcfns.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qgttpvqv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3zpmodsjp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xijhchtf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bxvfpkua.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xvejkrur.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ofqzhdjj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3oscsqevi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pmfvuspk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vobevlrw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xlkblfem.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3semkgasw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3alcgvpaq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jbxyyhwb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mgqafhaw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vvewqhey.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gtzyqpcj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ecxfptme.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lmsteina.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pxjtgbym.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pmxkyazp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3miqumvnj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wvepljmj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xiiafxgj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vsaurqgi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vnaroxsq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jahjclgw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hlqogshr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3qzxizjri.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bexiiomr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eukvytai.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hjzxcskx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hbcrboss.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sxgayizq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jfkndoti.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3utyqfqjh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3svizxrdi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bcgfjmnt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xgyjqkcq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wzeczeyd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ulmkicly.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kdbawruj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fcxdmnuv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zttwfvbq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nmjxfgxx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cmwmkoai.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zpdvttdv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3iwxrgxky.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3oeshqykt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qphjpbtq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rwqyeawt.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hpltdpqz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ductuswi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dllafglg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3btdxbskd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tqwykzbu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gjqaomez.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbhjgyl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nxqlrtqi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ifaadakh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hpsqtcpy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpnzgbth.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3osgjxzkh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3yhplrjfz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cbhrleph.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbunqxrt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ehzeoypx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3crqzrdha.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iokthrun.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ntvyafky.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ckpxvbml.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rynemlbj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ugqmshzc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ngdukaov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gvkojmmt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jvspkhnu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dodfwwxj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pyaduljb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3yemhyrte.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ackqufej.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3llsqqelz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hwlcazaj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3snrymgwx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3frdjpgxy.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wtwyleyu.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hjtlwmhc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kwgwclye.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3noydobgi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uflteepe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3svzktnpk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3znmqudln.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3dyvplvnv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtfnvmtd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rhjhrchr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3lmaghujz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3akfdnqzr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3dybbonmi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xddvstoc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fwumcbpi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ijnddxyr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdbngswq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3lixyilvd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ztpzjgpe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zalnfjsc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vliylavw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3dwyrxway.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ogojkpdn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kuihtanf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cfotjxyn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtndsyud.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zszplaze.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jglfhqrw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lldoyplk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3aiyrtcwx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kowpagbd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fgmoffwa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yizcjvci.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dpgvkdvj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rxiyznpk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3khxafikn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3giazipqj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ndopidnn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sqzbcrao.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3avvvlgyj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yuymdwen.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3daalekqn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qpltwkaz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uhwviytq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xjooanfd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vhfumlto.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fdabyfdi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ouptgyvq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cbkrfisb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zbphfffa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3umpyddhv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbbccrup.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3mlomcbih.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kpqzvpxh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3bymaonpm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3bymjetlk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rocukhjv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cbkovugx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hgzuvurw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qsapukbk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3vxovbohh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jzxmvzxy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3lbcahfnu.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3uhaifibs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mfkvobbf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wlxjlttx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rkgykbci.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yvrpyezk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zqwvmowx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jprxctff.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3mcuggwpo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ksgeoogl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ncrwjhut.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gcwebobz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pitywcwi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzitkmzt.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evwexcou.html


<!-- 参考信息 -->