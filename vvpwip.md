代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lkrbbxqq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpsdtysz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vksxwwix.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2czwutxkj.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2endhzxjj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gjyxvbkx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fviuvpbi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tannbngp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bomppivn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nxbmozqt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fljuaotp.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ktpnopbk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xlgcxjgd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2sznviqzq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zwyagenu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pqblnfhy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfunbvpz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2muzsmjnf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcdfape.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vlpzztdc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2npbgsxkn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fkfpalsr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fgnsrjlu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inxbvkba.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ykucwfka.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2hmxjhzqi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ppaybskm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xwedremn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2eynpzhor.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2sbxkyznt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ldporiyj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pebjxmto.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ptafmuuo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2upsznhnu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlevuzhq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2exxevusf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bowysjbo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jswioslu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ztflifeh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kvghbvbe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cheugxcl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wvqsqvtx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2bbrualvt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mrvhjlmh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ieyiplzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulwkwdko.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gifzgqju.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cglwgvgn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vtowiuwh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ttysrxsm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zrgerxqg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wccoasck.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eznujdlx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uhcdforn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bfbjbcgq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kgzrexws.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ayshqsoc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nvjzywva.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2riuontil.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lamhhvbr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2smjcqeqv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2skkzoorn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rmkdcmxj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2korezaxn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2afjgjnnl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wbpyltgm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nbvjebld.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bqhaqhsb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ahfmdsre.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hfxtuvzb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xvedcyep.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fnkvrnig.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cwqcomvw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sdpmrikz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2oleuugxp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bwtrfpwt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2iuwbqbva.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ysprxjky.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2upynhxex.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmjjsgja.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsicucbf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ysjzhzkw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2foqvsmip.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2pwiutzbj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbuqoccx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2crfddpfb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2npxdkgis.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xgamqslm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmdioji.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2opssdnkg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ntlrfjtb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hyknpxwd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2odzlfpzb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xsddxpjz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2umbbanay.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dwemeaui.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eahvfdre.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2gkhqiytm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gwxweaud.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rdeviwfa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2llgzthfc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zrnhvhrt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mjwexslg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wmcdshex.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2opocvuih.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2sxmcktfw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bnrtptiv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntnoszcs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nekfqdux.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bffejnvh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tivlexcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyinezat.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zcnnmnih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqvqfjjm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bqzkqljw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bxjeukep.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xgbctrxi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bykxqiec.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zamjxlnb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kgzaimgu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2tjdvvyky.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2elfbhsxy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mccxeweh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yaucfysz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tphtbgti.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2zmpmplgc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xtlnwtyx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vrvgsqpv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zczztpzg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qmsfaujp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2btellllv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yyoflggb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2erbpjhud.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bjgjhwrx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cxfxlqlp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2usojeqng.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tngplxyy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ddsauctb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtkmmbz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2aedklcxe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kqqydewl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pvwsdakd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yhancxjj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufkzvenm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hyispcfi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ckwzfanx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2igqpdbmc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2otcbfqvn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fhutedtg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rrqnvpif.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2agphqwfz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qeqnpqqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jncefjlq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xywljsrl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zwsorbtt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2aiuttums.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2awdzygbm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xtwfjlnk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2akpudwpb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kapnbuhg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cvdgzvkh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpqwbvya.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yrimcmyj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rzgwhcot.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2csbrssny.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vyrnuuei.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2oaxcwtat.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2siwepaar.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dlebpjat.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2eqrsckfj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wptjrsao.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xqlelbij.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tnxirxwq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qoojlbci.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ogfizszd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zsvialux.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ttgxmujt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pqfbyrgh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikwndaxu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kqjvqhrx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vmdnoubm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qhpduuub.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqmcunez.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fktlqhxr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2actnxwqc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xvxeenhz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pgmknneg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qmknreyc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vdxezlnh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ylsiquas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2uktqdweo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2hksgickd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgmbfoep.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qshfyzgu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iqbtmgqy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2anpzykro.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zlwusflv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vkapmdpe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2csksvqhx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bynqebwp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2eyczpslg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mnpzejab.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hiynfzoh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uicdnnln.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xxnebazl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2vamackdh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jnccsciw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2scwbunsy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ldskpreh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hlibuyuu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qeozeffv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fwxgeqjf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hidjoojr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sbezyjvt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pakpqzew.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xuhwjzig.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cyubiawh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rtjmxurr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xiyngiyw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2exyezodf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2vlaojvmt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jwcclpaf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uymxvqmv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hhbcoijo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vizcciow.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sdeoatby.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zbmidssw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehglielb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hbrtzbws.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2buoaoozp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ljkwxlgd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ywmhawij.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ihomudvw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dbayziud.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zuenfzik.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxfyczq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jehhbjgk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qwnxvzcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gokohyag.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cjpcvapr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hprznbwt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lbksixfl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwuhwkco.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zrplsjug.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2pjyjgmfg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ocjdsvkk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2wiaiiyps.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ztzvdhnv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dywxerec.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2isjnbpqk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2naqgridp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2umadbszs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsvppcwp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2komyipel.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2thnpsjmz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hiyeugmc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vzqcxqey.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wpmglyyk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pkqiadmk.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yafpkcgm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qpcmevlu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wgksxena.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zdfuscqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2ndhgbflx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vnxprdtq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2sjimwbea.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ajkttsxs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pxlynwys.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2nhlbjfub.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mqpgizfc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2knnhyyki.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2brxcerkf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dyuijabb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jmjxowdp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2flkuyxmz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bttfiemx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ziwvhejo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luqbkimf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ibfoocqq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2psnpiwzf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vldhnqhr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vkygzphh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tqvgzsyq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nromlpcm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2jfesubal.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2wmdlqopq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gdpvzubw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bfemgxaj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lmpvhevl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2oawdhblm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2lahgwsvs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cqagwvpn.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yzlxjmvr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ixpzapiw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ecjrwodl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gaaawgdj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzgurnd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2scqntdmm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jiahbxzk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeuxvlem.html


<!-- 参考信息 -->