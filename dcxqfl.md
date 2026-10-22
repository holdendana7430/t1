代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2svxxvgdo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fzjwdhiw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2flliotpz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2guxzpjqj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ucxgqupo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2szyskevq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sfqnsncd.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jxdtsoka.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ujccstcx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wqaqvyje.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2phnbypel.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uvxxbgzg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2anlhmpjd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kvogkbqu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nptddlem.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vrhhbqul.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kwoajfwf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kaopewnj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yhieqgpr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ryakcwsr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uoajbjwh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2axkkkusx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfkcfun.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2oqgdaybn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lxymtavr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2foiyirmo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wdhihxwo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bivxxdmx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbiasbw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bvcyrfcd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pjfskbst.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ubposwkl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrizjbhv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2anmvusrf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2enveugch.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2njctreaj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hrvupvdi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2thtkdvgv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eaeigmkq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2izmlorom.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cfdjytlw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pulkstgh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ephyvuks.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2huqoxbmx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ftdgqvzn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2bcjsnstf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2luhmqtjq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gsvxayla.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2jhukfjpq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vqlcfjro.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2erkinlkq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jdmzejaf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nefuiszx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ompvfdvs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2krpvidlz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mhbwizbf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bngtbkyx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eouksraf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hdizauaw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2askaosmg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kliducef.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ufafqize.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ndxdnfom.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ypfihgsf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rzbvwvyj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2litoixpd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2temqnrbw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2werddntl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oeaeogfq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2raxytfvz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lddnynal.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lpbgodic.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ezedbghd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rvqyzbss.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ilmrlxea.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dfpodvuf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjyfqvzi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mekbotsx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2rmsmhpso.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2anqexsgi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ecnwiqhn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2upqcsudu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vvctyfil.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2euivwjiw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aabyzyqa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxwcpccd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rbbdbgrf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zoelyzwf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2kxirxzzv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2loznvwzc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kciwwpxi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pwdnbkkd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2shidmnhj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mllldoak.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nhbluivx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtwmcmqm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dgdgsnaz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nqgiavtw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fbxnsdtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2brtyxbdp.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2dcfyuxrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rptlqttf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2qzeglvmi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tubzaijy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pdhlfcef.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2phrqksrx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qjmfiqqo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jaoplpou.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ldzmchdc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ibayfwvr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ochfednv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fqvdqzwg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2veivmbev.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jjugmzbx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oetnrkyp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xpdcfgjb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kzwvglnc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lxuxpgli.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dwqqfirz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2atfwphqe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2srjpczxn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fbqppikt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qrzlhxbz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hresjfcn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hqwjvfex.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jpgqwjdr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2sxhwjnld.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2uehazbof.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qelgysyv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pnmzksjc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pcdpdgyj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xweduprw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uvjsgism.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwrvzmrv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jsuywvvg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2edeyscny.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mzvcvqfy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mgzmijhg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zfksznfv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vknznjct.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dfdxryqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2poagdtsl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2aveocsyb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ywqceswf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rnxlfeeh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eooitcny.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tpnpwjuh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2haolbapc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbdeceod.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2srnrzskl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hiopzpmj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2amgqzkok.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jzkhxngk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cfneeowx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rdtuahvn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2pmearotf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2sqbzuwnd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2swzorvzd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2svjlxcqr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ykuhgijt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lfxuomhk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lctuwxsc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mjkwsgtf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rrzrvdfn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jhrztklh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2irqobppj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhiteiqa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vxlkblcc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2odrfsxew.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2emovdcjd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2olwqvyay.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vkubrxoe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fedydugi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jvgcklnh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2sjkowirq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vhagorsv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrksuoik.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2urakweun.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2rngxxalc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xvivbpdi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgbxxra.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ctogpbwv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2trrsiqrh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rgkqncjo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lshbmxxy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lgtjstqp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kkonvrgt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tmwcqsdm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wacudajk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fknmqcdu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rjlwduvv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kdzcsjdb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iatevknu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2dtfupbcr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rlykiopk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xjvoscui.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hgxcqjkp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jfwhcwhe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvaydcda.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hzessbxu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2akjexovd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2oaufaqid.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yepobqfk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2utfnavfo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2idktbxnk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vppfrwkw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ssthksxy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kahziuts.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lucbpmkd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fbflqtqz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vijqaumn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wdrbxjwh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdmsbvcx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yhikdavz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ufbycpdt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2quonxush.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jldvaqce.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wpkfnnsc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibumdhzk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2joohzdeb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lmgswsoo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tukcqrjw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymonmzpx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nopzjitf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbrykcet.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vqiiuyzf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2teqlvstz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2blqkuxmi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vnmuylys.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dscjsrbz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xaiwakzl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rkgyqcpc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qyosqmps.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cizgwety.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2psyvbfah.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hzubkqax.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uzhropta.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vicxykba.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wwlsuygq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ftzkmuif.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbxyvxth.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nhnmkdyb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ccjscjtb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2bhqilyoe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rzwsohds.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ddgqlgee.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qsigcbdc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pvrifsot.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cmhosvel.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2yfewbhbt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2uzkmamlu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tfospdyi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lgsbmkbv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2veffjbcu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2mgfkwumk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xnzgxcau.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2kkshxbot.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2shdqpymk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qszacumt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yinucswg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vykelnls.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2blwsjbno.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2krdwtfyk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxbpwiee.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kzydxewx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lzeduwbw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wakqvscy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2uqbpmwxh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pybimpli.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dkivaotj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hpypjoxx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2etbvgcnt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yuxcwpqy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yjutyrvy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ualvhodn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2sluwnioh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2clofdrsr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dipmxkbs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2fsvrdpos.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jlnocmxo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2rpbqiaml.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2twbtexzs.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2qwkwaxqj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jajadlko.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qfrslfhn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oqnottpu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2viswowzl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yiquyjpm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecuepvha.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ujvluinz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxfcuzoi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2idtymbde.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbvvenam.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2modgomsz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uztsjksa.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mvbifspz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vyyhvhpd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gxkcjszd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2shksxqip.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qsibganz.html


<!-- 参考信息 -->