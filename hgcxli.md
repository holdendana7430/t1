代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2iectipxi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lyhyzupf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2oollnufa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jiodmfkw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bhjzxjxl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mxxeivbi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ojkuelvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mgmafhfy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ksorkuzp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2rrhcauer.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dvfzotje.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kbjcovph.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qtyoxjpk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kkflhtfs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2auqphvpo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wygcxlei.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zvlhdzwo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2kszowkyj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wzqxcnuj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2mljespgr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qaowgjvw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqvarefh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pfxbuini.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fzvownzq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jbubnwhu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dsiuajms.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qbvuiovp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2txgmqorn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fqodzlnn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gvownsnn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gamvzazb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2unyrtizx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2syvskfvb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mnqrazdk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vfusklgh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gtmzaqtm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wgwryqlv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2thsvtkwo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ryezyetd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2quzhjmqw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gsfstide.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mmffuvmk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2tazbwqzs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2yrubokpg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2djqoaczx.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vovsgurf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jwberrdb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ywnpcotp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oyfydtgz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ujdrggkp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yqqctzlk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hzvbehkl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gyobkore.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2aakiktik.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xmjrvria.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rhhzdmeg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xgfeakqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2reanarqw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bhpkxbjs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zshwahrd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufmgbdzz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ylvqrcwt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tmmvrwit.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2buifldzt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uftpkpyz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jwdmtdtr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hjdulrwr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wxdtnxyk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yjjpalln.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2odyqrejn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cxwfeztz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2aywwjfex.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jaflszvx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ovhprojz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nzsiduyj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2sakthtqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eizksefk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2sytzpbjw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qhkcptfe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vdmqnblv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ybkmlrou.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lokzvbsg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kqyucwmf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ibwdcsmg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2thpnpncl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qpifqfmh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2svtoyoyh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkvfzdhr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2druszajk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzpcpzwp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ewiulfzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swsqvhik.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2twjfpjcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qllaapqo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2kkzdyddg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qnyziosl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qflafstp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mdxtpvbk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qzbncprv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zwbnhnqp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kpreltne.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wivqckex.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cjpsxmzg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mqlzjrax.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hrandtkh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yhcgwccd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dsvcojir.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fqsuzcza.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2npjgzgvi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2zxrwawdg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dgwjxjxw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2epckhscx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ubovjetc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2swzhheen.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zrpgxmce.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ebfuxxqa.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hrvliqvh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swsbmewa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ytodtlyi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jwgvltip.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oshctmmi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xewmxtew.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fallsedp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jfhbgisv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2dsnwgfgr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2plvygzmd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vxyrhodt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2iutopavy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2luizytvv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wyulcnjv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2paikditk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zswxtkmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jxmjzexe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cvivxdns.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tppnahwo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tyjqdfws.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zgnshdls.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2doukinbk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vcyyyowd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2oqgogkcr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jepxymat.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mhmzkfkx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2atpsqrcf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfoetues.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vzaazpap.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kxxtenwg.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ieblkprg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yykiyhyb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zdtvhkao.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vfyqntgo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wixjrcjf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2klyycmxt.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2shvwrkmu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pvjnmqsf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2oqhlcfcg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kchmlcvt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2coqlzequ.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ljnxvglc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2upabrrch.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2woivvkvp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2nmsbelzf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bwypteqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2npzbccai.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2brmgahbh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fnapatfu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gwyinrss.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2sfweleew.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mnimekqb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ehmqfdhv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ijikvscs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2yhwhxjoh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wqjerfdz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpscrkhk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fwjbyyoi.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2fbtaorhm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gsmzwquu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tkwmqnct.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wbluztwq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tmiasfau.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmjzpmo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ltbnwdfs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uoxawcka.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2lyddcqzl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ngikffmx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gvdbimcj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rpabawmb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2moksutut.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kkfzpaun.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tmtsdoxs.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cnijnvlf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ducznhpm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2garlwiuw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2otyhvrby.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2leethbcj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rmjmofcf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twqyuhsj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2spgznvcx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bymbuyay.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2xlzjmgbz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkyudbgr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2exqygjnk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2gzstfnqb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2wngfatdj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dninglvh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wbsxpyau.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebiehxgz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhleraos.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nbsmhhqp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2djwnwaaa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lpadqrnk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xarzfdoc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jzrvvdec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fjdxdafo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sbmohzeo.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zymugvdg.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gxuwjjcl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nqrsqtth.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2awamopgu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kgzcmbqk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ejqoftlm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2diqhrroa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ljtikvnh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lntlybxi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mthckqib.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2llysnesm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kmsxhczu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ndggnigv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kwjpfkgo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qxmivljl.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2srmldidt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ggctaplm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2knjvxzmv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnefevb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2drkylbks.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bvbvvqkz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2aubvjlww.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2gslhxfpu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2oprtgwsc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2celqjmok.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seayvwzy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jnzfknlq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxfnocoe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2vscvbzgi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bqmjvmcc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phxppyic.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2jgymizwy.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rxbcbcsn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ipddnquu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2iknffriv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ilqxvcnr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xmdlpqna.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fjambrls.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2feskuqye.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2znkxdeak.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2oadreztx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2exwklkbl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kntkfrft.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qrphmtmc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2byowisbh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gtfemxxn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yoxxjvbv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2hynrdtht.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ebnukcsn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2pmsousaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2fiyobpjr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wxoyttgc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tendsrvu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bblfjcfg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wzkukkno.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uctbhsip.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mknvbmqc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pduwqasz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2miuyagda.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2jvqhpemz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mipjewpj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gyfbvzmz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xlvxtjyf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qkbatnto.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktaskowa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ypxvocll.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ltxfgrqd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xjjgsged.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uqbdifls.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xczjgrst.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmlduqwq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ybmhjfhh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kiukhxxx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bymjapdo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2avzsusnh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rzpuskgn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cklslyxe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sjqdwbov.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ksjdrsxn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xqkzpqnw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xyflgzdz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjwmspyc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfpunioj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2oxjglqxx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2urkgzong.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2rfnzakgr.html


<!-- 参考信息 -->