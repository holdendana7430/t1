代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2wrytkrje.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtipueih.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2mzaskuld.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2oekoqjiy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lnnckopb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pezjofno.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2scjscywo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ypqxxwbb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2psldidum.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2drkbpojm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fygpzoyc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bkchhuka.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2yblsauns.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pdajaofg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dpspebxu.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bcxmhkpr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hqwayoqg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hcbuikyh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ihhiyflm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vsywbiqh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mwgrirwb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2pwfxivgj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2nqstsdfk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oyyddyfu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2lanvizga.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ngiyiosp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfeimqzj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2yhxuvqwn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2yerawlqc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cepadlup.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kgbjjsba.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fnkqooxu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ocjbnmbx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jmleqekz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccejfllr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2fyoahptn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pqwcpmra.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2obfncfuq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsunmqql.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ujmopmfz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xwcpupsv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2vuyroyjz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tznmlvmv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ahrpjjzf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2csdswqoy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2eyhiecso.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2spltgkqr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2phfivesa.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2aczyivax.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gkisqoip.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mtbnkddd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mjomqvku.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xyawlkal.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lgnpbvjy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pfjmrskj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dertsqbu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kzanzxci.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2yjzitbqa.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2shxmvhcj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zszmwrdd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2inzcyope.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lspsdtll.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2oqxxufwy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bftqjfbc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ogozmudq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ieaeutls.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rebawrdc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qdgrlqui.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gjjvrved.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qbhvpofd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2svepbbpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bhskimwn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2tebncfdr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2buoibioy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbkfemyf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xwjldntm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2shhijqjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgvuyycg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yyggobej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifvjlums.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2swxqyvlb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2beqixtmg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2dtspusui.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yjtuhdhm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbktlvmz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zkqcssyc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nvaqbicw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qisynjjv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lugxregs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ainhxdkm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvexxsa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rcujgrzh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zjzfwwva.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rdanvhbq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mhiyywdh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cyeopkhp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ojnfrioi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jthrywjd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vjrqpjbw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qnipfqbu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xoorunxf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uxenyfvo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qrvtjjgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cilvwiiu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2owkdreac.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hajemuws.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sgfaeyvr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myhagwdk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pleprjsn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2iileuuff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2domwclnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgvtqzgl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2uprbqxiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewpzdixg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dxwpikxm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lheizita.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gcmhbcqh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mzibkoci.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sghmkmnm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2qrzkcyed.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lilhlyug.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ytguvatw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tdjnvtfv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2toxiwwwu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ekskwfqr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqjojpu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2erwkrzqr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cohxwrmj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ktucizwc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcukqfh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zhjaykfd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yaxjtvwr.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2znktxyml.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2brpdbltw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2miiqzujl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dyervaey.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qzkivpra.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tudnpsgx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lmmvsuic.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdraofnl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gjxgvhaq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kyapnusv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2srdgzwof.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dchsdmuy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2peuaogvu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2meblchao.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qwfzrupr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2pbasgtav.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xhaozjxg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2xhwvubvg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zhrxdvmw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zpiwtvbt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2arvmqird.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tqvqpebe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gboitsex.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zmzmnutl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wxhpmmvt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2deltwkhq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hxlzvrbn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zgyamkac.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2csvcukqq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxvuiflu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2blhdqlvb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dmjxrcxs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hpmktsfh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2unkjqlpb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wivcosop.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2shxamkuu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zgrtfhgb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kagrelkp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vkbmpnuq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2moffencr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hpbacwml.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oevyfzde.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2egocczgb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cpjrippc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kpnzsbwx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hrznnvyq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qhhgzirg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2scyngpoj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2amhfahsf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2icjjkbyd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xgzrxrrj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2klpwqprv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2mthazlmx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aascdagt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hbcdszfy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2egvoivrm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlfhwpah.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zddtihxy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bejcuyte.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fkjqwpbg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2icxbxied.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lpjddkuz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nphpvtvf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2sylgfbkd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2licykxtm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bodugemt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zodsrpfw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dspxzsis.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pvzajuvl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lrvgjgip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vpdjubfi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2olsdgftc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wdhkjpvd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pplkpvyo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rfhuwoqv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fnzapzor.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yaxfdofz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2laumvciz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jghqljhv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2esmiddbv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2brsqgctp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rinfluit.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2elpoxmyo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqrnhnxy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xhkrujpd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nfemxqzh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ycqffztr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mrtljlns.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwlimmo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xrkcgksw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jlakghcj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qkqvhaiu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ehedvena.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2djkwquxf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ynqkjqcf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qigtpsid.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2oxpjksdx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kcqomhfw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cnlzftee.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2eubthefa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tvvzhnjb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2canusgbz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwsuvjem.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fezjufnx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zvlckmnl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dsbxkhze.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2upyumlat.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tznmjjmd.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qedgfgyw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qmmtihon.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nebcctsd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tfznlkyp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cucboylh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2lfyapgpm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2twfyuftm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ptsknhju.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmrwgiik.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nduqkgmv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgpszvgq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ukjweyfw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpqfnp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bckzxvka.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2shdxzqpk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2flytcjzm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mnttkohp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rpojwyyg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tqubgxqg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ohvmzrqi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xszvncad.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vlhwnuhx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yaiyavlt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ynttyuad.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sopkowbk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ffrhtgyn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zkhqmpig.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wspgawet.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xlaoghcg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2sfhykqlq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zcywrche.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2brajhkzp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2enwdqqyf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vlwppvzn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gbyajher.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kuqitdpt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nluorvjv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2klplhxzo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2eknpbbkf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aozrnyhb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2eoiobgut.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2srxtqiji.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hqwfpuzp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2brdnfexw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zyvgidhc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mqdycxeh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofarxiyz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2keykkvhc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qzjgftei.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qfgcrneh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dkxnhkel.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hbdvwojf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jiuvxkey.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2efkckcum.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jdyrrxql.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pputygvd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fnlotlbz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fqbpaitx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvwkysl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vjfrotgm.html


<!-- 参考信息 -->