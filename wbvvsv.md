代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mhurbzcn.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lnkwqwkr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uwcdnces.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zxvizxzg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yjbydapl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pmerhuvb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2moimssom.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kflohcaq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aufkprvk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rifzasmz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ikxkqhcj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2coetktqv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vlinpsek.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hbrjlzxk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bvndnbul.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ghtxdirm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2cbwgttvq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gekszphw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nbttysck.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dfwhapbx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2psjlomnj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2aciagoam.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2frcbxneo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2erxacxln.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dllxtdol.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvgaxyke.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nfuvhlrp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ghjruowm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wuaoycyp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xnvxmzsp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zrueisfo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gzcojwjy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmdfadvr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tfjlklvj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hftwkeqp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ybmnorms.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfybjtvm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tgomocen.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmjymqmh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uzvdqaml.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ivxvslrl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hoibfbod.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gqggfktq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rqnzjyzm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2muasywgd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2geigtqnz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eegvkmgd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pexgbavp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kiugdiyf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2qhvrfxas.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yohiihoo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rdlsfaaj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tphyejtf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mwfuswhg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2shehadvs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zqcrztjg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nhpaazes.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2szomwcjt.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2czzvjori.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nqtinmwk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pakbsyvj.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2omuliclz.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qsialclh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2yyxukgyh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzrmvh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zttkqytt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2woorgnog.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zolaeoui.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2kgfmniyr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jwydeust.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2caxsqddd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjjicqj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vthimwge.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dygzklpj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qkgijtkt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aocxuivd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pwhlnruz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2filuibnm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ilczrliz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bvztdmhh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwozkto.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qxedcmlb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ivjpxtoa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zrrhgppe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2kictgegy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2aebbmlkc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wbksxqvu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qtnkahjf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uuuyyzyo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zuonybsc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2baqwmoov.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fnusqofy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2twyapwwd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cfsahttv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ugitlznh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wcycljej.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qzjkisvo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pfezhlrl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2khrbmgqw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzferrrt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vqjzeilb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxezbrgf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lghhvcls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yofmppbl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2dtmoivnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axoatrft.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ulzmutpk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2uctyoiru.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2treagzwm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2stvijhkn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mdcrvlmb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lqdoiyrv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dxuuqhcn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yuvhitga.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mrxjimum.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gcrxylho.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vkcghqbx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rnlqtnht.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwggtvyj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2oqgfmpot.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hyyrkbwf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2howwxgph.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2eyfuzmst.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2frscjnma.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uarniesp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nakvearm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jxipcgqp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2iivbvdtl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2spzsgxgo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2isbuzvhc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wdbwghys.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eibacbnj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kvpshawz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2rvcacula.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pmevzgqs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eoovwttm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vbizxpab.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pdihkinm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zgghhric.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zlaccvic.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2apgqhxja.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ggwcwixo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2tldbbprt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zhoykzwh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xhcdswdn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ykgdjivo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jzezxaxx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bspphejb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xgsrweod.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hikpfmfw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ngckphja.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ikihoefo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2neltgphn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocuctrjq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tsxqqhsr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fypqetso.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ajlmqgxp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lkibuawm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xyylqwqq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2oaawsttg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uwquzqlt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2skuhguls.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vlbkazmv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yensfisc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bczpxowb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kkaxkpnn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rjinebzv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2eqwmzrpt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2abbczcgl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lcgywazd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dygyaamu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2nbwcrbvd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vwhepmrc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hvrypjee.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zshbxujd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrfvdey.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcsqklem.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhoanczz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wvmfyfvq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ixjxyywr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wdlghllv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2suqbavmi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2czmjeniz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2szbojjln.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2icjhdifv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2sbmoxjia.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gfotewqb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2iuspcxkt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2evynrafh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wuacovao.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ennitskc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ejpmdpmn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lyhgaqfx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gapkupyl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qwrgngkm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2fawpmhgs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hnkwheie.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2kxtyyuok.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hwnmnzfo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2krkjjzoo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2drzlddto.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vzjhoqiq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rmeqirst.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qlomioam.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qxscfukq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ebypezln.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wrmnzykl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bpavhrud.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjwnamvk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wyqtlduo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2uzznspxj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vniypuvn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2gzkgvdbu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zrrutfmx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2lvaiemgz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2erxafelw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ebctpxte.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivpbiijm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pyssrfsd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2husvffwu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2zhztolge.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kxrfxpje.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2txcdqisn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pdwxsezt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xlgmnveo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhpnqlqv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmpogfwf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivbvuxpm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2nycslfim.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zmcypsjl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2smnwaqlg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aotlssla.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fmuvsjys.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hrxooinb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlzaugud.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pdtilhmn.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tdpklapw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ffbltrzc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ggvsxcqd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uwcpnupl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iplgphxq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ihkspjyk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rvoufhqd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pxsjvofh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zcavgnfo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ucauuveg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pbajksrf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xwwoouhs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vulkvxyi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uarfswob.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nmiuwzrf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzhmvff.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uqknzvsx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juqngrob.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffnktftv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qzpefrlv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2njswxvik.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kpnifuck.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2vfutnblt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bdhzxdcc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2filmufzm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2sbwvcizj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgyzwsq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fxjzwhyo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2asuljnwu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2euxtmlmq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2znxaikih.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2esqkuomt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2apgrlnws.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsssxtr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vvazevxe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ucnhvfgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yzhbrqzq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zqmcroom.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gbcxdmtl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fgyrqfmw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bqpspblc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cmweypxj.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftuvyupm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2njkyepno.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2eizhudjq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bqfzhfoe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fuorrrhw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hjylsejx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gghzmxyt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2jxxyxlkw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jwosbgak.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2xgsfixoq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2johiokne.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gouqkdmw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjrqdkmj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yisdoqjq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxpifaju.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tzkdwcxg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yweqnman.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gearuplh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nyjytyfd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2fyvflywg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rzqdoumz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kqkwpzjt.html


<!-- 参考信息 -->