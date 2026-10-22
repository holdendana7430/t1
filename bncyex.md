代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2myxhgzki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wuwkcbci.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhnsifki.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xnhfcqcr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2scpjaswv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypdsxeih.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tdywclnj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2voqzzbsn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyinzvbg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oyfwvwcl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouzqbokw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sfxpxpjo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjlyjftp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zlpqeqjz.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2cmcdidbd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zxviavda.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2enmqrmhp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdnllxcc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zjznrdkh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zeztvnkh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hdpmyhpy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2awtnffhg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2maarqywm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hdmxostp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xvvjpxxi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vqmwawmg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xvdtttbz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2sjcbrnic.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jinzruix.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2khchxxis.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bzsicyyp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tudtejse.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cuzasmjb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2kcslbafr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ctvhnopy.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2poeounrz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mfnsulqe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pdetlngi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2dpynrzeo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ouhcarod.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kbtkbafb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wkceejwp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2bsohavpx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfgxpjkn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bxvexaqo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2oexqqhrj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2emkhjhhp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pxlpjakh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sowpnsvw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nstcjqbc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qptzrlml.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xzsebxgg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejrzhcjw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbzcqmmb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cpogazbl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2uibhhdnc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxojnpvv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2frtkeumg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vvujhqas.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xyqdzhmn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zfjsdftl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmufvsby.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yieestin.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zgokpzbi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihywyapg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zimvomxf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ujtrtvwt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qrzitmmh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2aspdubhu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mdnykleu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wjpuipaz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2urlbkbmf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ptqkefes.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jdsnqxhr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rhztywvg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ussoxwqy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vcstzlwr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nfmyyvrz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nufwrqdh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2btmwouqg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rnxqliae.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xeplhswc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2lzfeuurj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ytuxmlah.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2qifynmqt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fxycqbak.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nhpqtfzn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qkbkidfo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2atewbirn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2npacjegi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nqezmeve.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mksstuho.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2jfrgxqty.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ffkoskqk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfeypvfl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lmuiisva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qwoampzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjbtyeby.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2quzhgydm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lscefjav.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oiqhelej.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mzfkzxjt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2volsdybk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2wqmmjuuc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fbzsmool.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mijhsptz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ujubcdnm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ayvexbyx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ldcdnryz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkcxjjxo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnulcfx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qbwnwkhe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lzamrqiu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ihgdqudc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rynzsjjc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zwebykeb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etlyncfa.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nntclprt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aqqaujpp.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kzncfjiv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mhmktxaz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pdeezhiz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2sbvueoon.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qunpshox.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2foejzrtb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dltxomen.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2upwycvtz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2maghoala.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fpjqccdy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jwuwhchn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntzzbgba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhxdvdof.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gsytpqfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efnlritc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ewxfcofq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xcqrdypc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zvfcvbdl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aayctmlr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ribocwdq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2umohsnyo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rduwnzkq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ehybrnuo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dnobgguu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rvjbmxva.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xttdsxkq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oybcndeq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sqapcpcc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ixepfcrp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ualmzufw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ehxlxsck.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqukzrt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2xjwhwcbj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ctcnseco.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ocxrxgvp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zqqkhgbv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2xkyypvgp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wkziajvp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kghmzpte.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xfbchgtk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2oafkdoui.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2knigtfav.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sbzhhtin.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nowvouyi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2oiicovez.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2brfzwaml.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2anictpah.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ahyvpqpk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pzzblhks.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wxocjkuk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wsypmmcx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jchtszvw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2msexghmu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ozmfwjpd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hckotbdd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kmuejlzr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fxeotmgs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eqckjeoa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iuyogeix.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ukufjhvd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kridunzg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkcgcfit.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tmiveanx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zlhckowb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uyrexdpt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dwhervvc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ouklpzqe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2afokmgnd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2uuuecalh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2cvksquyi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ufcsyesa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sftbfpab.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2shxcingw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2thwjibmw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkzbzmqk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vpbgcrnw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lwxiewhr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mludwmek.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2hirgdquc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mqgayqoa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vqdhzyfy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ylhucfdw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2nxuuahwo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2inemrgxc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hqhveopn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zcrxzqzc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mikdnmtt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2swdwjhmb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nphgbwvl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2olvzjlma.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lafwdnxd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mxounudt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2goipowck.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyscsqqr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gurfughf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bvbgkjdg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jhmjsxig.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmbfbcf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ceyftluj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fubiulpi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2glhkrstn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rcckkawi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ehfrfiiw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qweqwytd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2gtzepnmv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cokgaqbc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yjtwoigj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oacyvmrh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yzgllhfz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jvsnkedq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2yynkdrtx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fcimiujr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zusevtlb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xzoaihbe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ayzevuzj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lsrrrlgk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlwwqhtg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mskqbngt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fpomvwrq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2taboeqbz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpjoblta.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gkfmweti.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2vvpeegxo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nxzwvtrf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lddwswvr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pirmtqwm.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lcdcqfjw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lljinsfc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wtlvzeca.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jawvtrhk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mttyotaw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tofmzhsu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kjyhzkjj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ebjjjtso.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjrltapq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eodshbia.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjxrjkan.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uspcmfvi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pgpzvioh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yttvdlwu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lcethbao.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fcprsdzk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pmfsacch.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhjbelhq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dqtumddu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sfhslfom.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jeubmjui.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vmoerypo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2laegkvdt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vuvqnuqw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2upqnuerx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hnfnacos.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uasbqcvy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pmdjoshv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jdkbrpqj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hzsxruhu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2dorxzyng.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fsgokjie.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ntcvxjxo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hebuhojp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bzrxwyqh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2zidaseiw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chnooksm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2wmxvbpzf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vhwtoxjl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2lgpkujni.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2dgztrofv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qhbvktwk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2iyapnjwb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2opwoitce.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2plxwuxjh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2uljmgfrk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wykjpzeq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qhpwlnbd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jbqzlwqs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kewpqlbp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xfoaunss.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2itsaevwx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxvkyso.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lbqzrtxl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yvwpurkf.html


<!-- 参考信息 -->