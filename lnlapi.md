代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ponrexcc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3msqbfxly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbaymbkm.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghfexvbz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vfbngkaf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3imhtcdaj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jonrwztf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vgyaedcw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpgdpjtj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3okewaqfb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yyiwuvqo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tminimej.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qcuwjlrv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3cthwymbr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqjjetdy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxoowher.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwxqyryi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rjzjblnz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3swyqyptm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bwdfcezu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3juyodtlp.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nycnkqje.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dbptdflg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3edzorcpe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfjpubkz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcqyjaoy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xpwaodlb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fotljbjr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcblutds.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bsfescjp.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3wjkothwj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3eljgwcgj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ntwlkges.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyvqdaul.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jzfhpkfb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3zxihbndk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zioklnmm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbvhbotn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ujxjprxu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ndawgaag.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ypmuuxeh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wyohrqdl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gilkjnaa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tqzhlnwc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3oxhasqkb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3injnqvcz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ygrhgnld.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pocmkite.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jnkdwjxj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3glrlkkox.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3uzniwjvs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jgqnkceu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mdtkgzwr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gkzxpslu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3oeluutdq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lkmiekvz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tgoqubst.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qncuamlc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tiiisvki.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3soumqqbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vsliazhx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3bhvrdzyq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3onysvwxn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3malejywp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gsxmfzqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wtbjznkx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cmbqdsaj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tzizhfmy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhogqkcq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3knqtehgc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsecarlj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3acnzneec.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qtmkvojp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcpxxrez.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nxogdehm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3rdgpdrnp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3biunkdnq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqmjndyj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xqcbjben.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ldtwskqb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fbjiclig.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bhrywocx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mpzunawn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bcqnuink.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wdejvmix.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3upunbmxn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3veokphmw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gyijfguc.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vxzcuxbi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uwkykaxh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jbtgusqg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ifasgtgq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wluzahgy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cfwnwopc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hbkygfgx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhrqryd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3scdxwpqs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bwhebiio.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ymgwusyi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3eampbwko.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nvqrodxq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3teqqqmco.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dglkcysv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3zdbrajmf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3euhugipc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qzsincad.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bemhpodl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vxadotzv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hyazoxwy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3unbomiys.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dozczrff.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3smcokgsv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3glnsrnhs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbsusmjk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3pchmvnkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hqorkvol.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzhflggz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ajbagaxb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yfiggdsy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3syjedduy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbgatdge.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vnjfglmt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sepkurye.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mqmpyjgx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ltfqmgcd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnanxubl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eibekhbq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gmnzkrag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nabdvnjf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hnrrkowg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3etdowpxp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qoejbfae.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rlieygtz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ncwqmgot.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3raknkgxn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ntdvtugx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rnkalcay.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qpgwsjwy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3azwnjkhi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3haajyszm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3djphpelk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ejmskzon.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3zgfsbqjq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3chnchjca.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kbwhgmrt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3hzhcgmmq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyraenhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgjzhtpl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fbwszxyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofiqdklw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ltvdlhiu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3shyeswbo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fezyterm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lqrunhto.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wvhunlyi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vkqxtihy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ndukqxky.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3tqpytbko.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jmyghjdo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dynultyv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jxutqqoh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mtwalfxu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ogthiuho.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpmzqevh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xqstjful.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jkdhkrbi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xlaxgxbd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rymycdsf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3yidseoxj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tpabrspd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wxemvnrl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wwnfptsj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ppmzzimu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sbrgesll.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3usnkcnav.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ycfrmjye.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ngufotzp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3dxkuulmn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rroymqls.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sfpndbfj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sappbdbn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3brjhgzau.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qbtxmyxl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xenfpoda.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ixauzwxz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3aowmjrpg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3mpixqqje.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cdxocfod.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qubzsrbi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vzqfvtjv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3acskxkeo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3bbuyorsn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vcrkotsp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3joxvtkra.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jwljmfwn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3yerwknvo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ulgijdms.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3oolwafkd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3juhkkylx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ewpqmwel.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3owhvsesu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ktvcuhea.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cxamdfiu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nofpjzam.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3bvdmicfe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3pnxuawlg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yeirfiyk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fccmvclh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xzuvaqjr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tktwcsyk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mmcbzjqv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3gxyczbzj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uwuhtmnl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3essnxglp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bphtjclk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jkowajja.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ojntvwak.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3xgglmfgy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hathcbca.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xcojlbdm.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xkxqtyty.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nywzjvun.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gleaknai.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3inrwaerg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwijsel.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3invejkxx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wguhkhiy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3aolgwryr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3giovhpdw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wzyriapc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3pdvbpvya.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3umupfkfa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3iwdtusmq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sptnwqig.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3snsbmzjp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3skfmbvec.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3znsufjdq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uoqrnjkm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3aqxlnznd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3sbyjptju.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3iqynofxs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3frezybkd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zckkiedu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ljjmeosm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nnumncfl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vhrperux.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxzosnsd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jyeprkce.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xbpqlizm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3aoqvtocs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wyhstjsg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3esnrnxkd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtexenlj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yyqexkvm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jfnvyuzx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oeapkfup.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3csmrrjuw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zppsguqk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3uhjkzeck.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zrftqgra.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wexnwndo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3omjujhlg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3taoccdkk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcfruvij.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rhdfswhh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3grsejpei.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fqybnnup.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qdzoyjbv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zreajovn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyyrytmj.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eeyflqdw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jsgcwwgf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lijdgbru.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zjetpmoj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kzxstslx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tuiejdfb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yxdhwrlr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xupceczq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zxfclmms.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xeudckdd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mvpcqezm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pmhrcxpg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3rtzwrhtx.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vtcioelt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ovyjphbt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mvzrmvdu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hywafmlc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wjzcmrpc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cjstfkhh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tsxmnntr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ctfrzaeh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hdrrfjtg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zopdaadx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dhmsbtlf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nukkqcub.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3czdzwynk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3etjvdcyu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmslpum.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3sjvnnduj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3swamelmu.html


<!-- 参考信息 -->