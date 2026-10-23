代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3urfkxapm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3apgvktgn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdvaock.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3guploanl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3znqtyzlk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3aakzcibx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xmvzkgue.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3peuqlwxy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3uhwvvttx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xflvaccj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3txgojfce.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zjlafeag.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3hqtylojx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3femtsswe.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tcagluut.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vvxectfg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bzsymcvh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nsnebxus.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tkzvvuua.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zxhqjikr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ghmpsmzs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3eyrvtnsq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hcsvatil.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3psqwvstr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3djmfchgl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fkaygtfk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3voxbgnhd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3swdabeil.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tcckxzby.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3aeyvkhzo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ydtptzbg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ixrwpeku.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrpriodi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xxdovxea.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3svcfgfep.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3buwbkjoz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bqzqzzhd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3raqkxcqf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcammvxf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3qnyocojt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmswgxbd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3krceipnl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kgvrqizy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fyfgthug.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbpmswzy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3phjzdsqw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3awlnvyee.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dhqpqnut.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jmipgruq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3hzxhvasu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pzcubhdz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qrozphes.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vpgawnbn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ldmgxzwm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ztszejqh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fhqhfquh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vjgwzgyw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vwrdrvif.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gervfgmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ndfsorvt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zqdtogji.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fbpnnngf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3omlywjbu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3hlkdwdqu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3nzkoybzo.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kjimftcz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ckneykaa.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3injlheei.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bifyndbj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qshhpsuj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cdntqxll.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3sgenfuap.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3chokiszs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3finutmmx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uadlrrlo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ystjcllb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uoeizqsy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3sjtooalu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xusvnnaf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cuxjtsaf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnvtankp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ozyhoouo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3penawysr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wldbjsvr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3snlhricf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3utixotep.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rccnvsit.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lpmwqejs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3azdogkyn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxaromvo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3zgcxgcdw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qqtjkcnh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cclovcqa.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3iswvyoyg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3uyzkungm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wkdhoels.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fefilqld.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbupdite.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3csugyzza.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bqlqlcft.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3knikawzp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nmoawnot.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yihngiae.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vjdkllzh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pmpccucd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pquwjhzk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nwtbrtzt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unnorgzx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3nqnztgbh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3imgurfys.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wymyiidc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbzsnvyj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rxlfmecw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcnorcjc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mgwlyjhn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gfcnbykz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rfvmsijw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wxsefpiy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jackcobn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fnucxlnc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3frpgucvr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ywyjbuvy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qtxvwnbk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3jtpyaung.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vpqmjriv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3plfvgjlm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3duzmurxg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jqomwtlj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3prunhhbh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nqaspuod.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3nsqqrayr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3akqngwvp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3mgreclgb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ueszorqm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hqtrxcwz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3avnlgdnx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mefkoped.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tmrewgyl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wssrrcst.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjankgt.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htatowcp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ouvmhzoe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tlhbehwt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzoaicl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uqjulwds.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3taxddjdk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3weidfavq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ogouggky.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bnilsqqa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3azogiycw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqmuijqv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mrqmrywe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xlffzcxs.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mdnubuye.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3sgbczpur.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qcthtxqu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nekrpbrl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bmcxolzg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3epnzzrjw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqdibb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xnpinqpb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xsgxiusb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rgvqlxzq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jeofjdso.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fiszcnqf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jozvyfkv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kmiamvwp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mqkkxxhe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ljsztkiz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lcdfzrhn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dtqgaqqj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hazidpna.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3deymgket.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vfhebats.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fnwzmacm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ujfwvfqy.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yrqvqxvj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3hazicynn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3totddgfg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fdkgkwuc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3tltjlkgl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3proahqtq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3iwxcdmms.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3owkjesgy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3feinwhyd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wqpqnjww.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ekmmwyzi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wfwcbets.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3dcurebwn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3numeswku.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3pvddzsqu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dmhcgbnk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhzqpte.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jqdrgkog.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3btapmeme.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3rfzjhyef.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qpmritck.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3evslelzj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vdgnnfec.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcfvaxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xyafxkjh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xdxtmbku.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rwpijcbu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ssgutsue.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qoiqrdbr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3uhizjzkk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3unbaomkh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3aybhpocs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ilpfexmj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ybwzqydn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fbtafgcq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hcztywqg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3putbkcsu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3srxulbgc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rywmlzdf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kqoxdpet.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjotkhpb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bijmwsha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ejezxcde.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eldrqqac.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmupxiq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3wjwpmjuw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xsglrcnq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vxbexhqi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lgdkbzli.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3owdtkzac.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zftbgrrm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3exmmvnff.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zpfqiozs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gqdezzzd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqpkhqwk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3cegboyju.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bnlxmvdb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eundgsrf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vnarkogv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tijhifnw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qamncylc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3awgyurao.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3inlbmbpc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jyyxcedn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fckzfbym.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vjkmadms.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhpkrrcf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wrgznlwg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tedxzxda.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gbqolfid.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xsjcbrpy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3whnkzapg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oiizwhus.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3fehgfbqg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lguetvrm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtgezxcg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mszwwkdz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gkpidlak.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ryxsetoi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3uhtzbvgm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3elinyfyh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uwgbiadw.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dqvkhmfr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hlppebrw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eyazpmwb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxthsvmi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ouyvwbkx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ykzkfned.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aizxyarw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nctlnzpt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pdxuyyet.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lotoalxf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3mkvuzjjv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3nrrstrpi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mkubecjk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3oejccjep.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xtvhozif.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cilnjosj.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ccxhfjlq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kdfwhttm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3sntvwfzr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3izruuqve.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3slnromnk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3xebswrke.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nrlvpmiu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3flqibmdt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3asjhstaz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sfshyqid.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rdqiemlw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nzkfnkwu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkjxbhcm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3otrfxybr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pdjeahmt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3cgzuvqfs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wwozwjoc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vtqzktbm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uiundgan.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zlznntzu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3bzgnbilr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3xeunffrv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3suhgntkp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyqukepx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3udpwovta.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jlbbakza.html


<!-- 参考信息 -->