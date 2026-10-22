代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dniuxptu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2irpbujxx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zwezylwz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ehtwkqof.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxnwgqo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zlzqkgvj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2eqeqevsz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gdpgglft.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2gkbcydef.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2frqnzqqj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hjnpqcor.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2njfkgpsj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ckxkdrgf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hhfvdhet.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fzhhldhx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2migcokzi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fyvrjgmg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ebvmhsgw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhhyvenx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2almelhzp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqpcmrij.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcygkylb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qghsvzfn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tjivfgmm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlflxolx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2kgmnfcyv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzlbotux.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhevvbz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2deqauqjc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vxwfaynj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2uuwrxzzq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2aidvpqkn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jnnomafe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kjrumwxx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tplgjhqd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kqzuksgj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xlddonxq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zhasaloj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xxlxdcpr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zuesbufb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2sgknzhsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ppeqtuyr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jezhzvtg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2bifclnho.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2yofimjxy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2txfgomjr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ayyngotl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2apcdhinn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2giizponv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2odtihrtf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vtohfpje.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ytakmbce.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2efdeljxs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gugoamwd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zdxlvisl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2cqaapvwq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2igkxkyty.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgptivtb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2greukmiv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rluujfkg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgvbqzxr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ggjviqrz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ypilyymc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lkecatix.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnrlqapl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wkyamdvj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2snluxoeq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yagxffzy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrpavbtk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dasbmglv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hbuqjlsg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2plkcdwqr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xuecvsbm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2frtqfedr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rohydsrl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2shpwqmiw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aheftkne.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xetrugxa.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2emmrbfmt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tnzbykpm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fizgcrby.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vbgoyxgl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ejmutqae.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2exenvpqk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2lykrsoia.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2qkclgurp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xqklpdfc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhsmzqtw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jbgrtavk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwzszjjr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xischzpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vodftjxa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fwhffhdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khmtmtxj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2stlabvig.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mmlwnsby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wonkzvbs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ekuwmpap.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mvzqamsn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ibxsafxb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rlpvxzpi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jewdzfdy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gjdjgudq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2douealwy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2snfrzsxo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yrvjivnv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2knpmvmsg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cwrbnipg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hneemqsk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jqkuyfgp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ogojqqla.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fpyvvqiz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bojgppil.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2etonnzdz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gdobxejn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uyxnnpdu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2moaiijbx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xlxdozhf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2weoyoyex.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2otibbyrn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vcxyklbc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rydmzzuk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqcvlyf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2smoymbax.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yvvwxzmx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2admjwwaf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ldmycxql.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qtogtchs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vdscpdal.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zfufxnup.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kuhwtdku.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ddgbdtzk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wuglnbnj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yrtqcgnh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ndifjqis.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zksgtfcn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2urazxoaf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tejrftly.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gejxsbrl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iyhtqlrf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdalgpsa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sryypazg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ulmbvehf.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ovqhesnw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nkunhqhl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xsqqxndb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uendfygu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2nxnibxxi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2siptrvkx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zasxmwre.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uawwojam.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gqxawmdi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ozyzskjz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2auqhnrhf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2jgqcslac.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rnbeglre.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2djmtijbx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2chesvkpn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2llkdxbok.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nswbfvep.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2tkajffyd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sqlcumyp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2shjtflas.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hbycobim.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pwozfwvd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gtrcjrzn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uttgmhga.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cycxvwyl.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fkwzduvc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2mqjusirm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2icwrxtnk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vxrlgjsr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gyybwdao.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tdcnvrto.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pxmiztzr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hoyclcqj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2dyqhlvhs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xsnznozv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cxbcipqh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2abzneomk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ifhscmzh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xmouizgd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2apavxnlx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cwejtduf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2cidotdic.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jqmybjrr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nxlzfoyi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rqqpvkxg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vmaklyhb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2asjxmxhz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vraahfuk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qovrjlll.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nbwfrqwk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2flgqfhlu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ewuojfiz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjalplpc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nmnxgonv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tghsksgz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2htlmksom.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqwwowzi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wvckdszp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2tukyxhrn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2abjpodhm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pnusrykm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lakujvbo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kecaglhz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdevchg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2runcorhx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qwkwrhee.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftuflwus.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2paadrzbz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qklkimvk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vcectyvk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blfwsxzr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dtuqmvye.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hbvukzka.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zigewdiv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dqiuxpsw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2csqrfmsc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqriiauy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2etgfsipr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yakkkptg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cwmxvsqb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sxiarauo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2upvqdwwj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zpakyquw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2awuwcvmn.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2zdfamhta.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eehaurte.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kpbrwvge.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iryxvzsi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qescpxos.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqmharo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzrlkzu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ucdjpviw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jsnbzlvu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qinliayg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ieigzext.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ulqexyzu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ljeisykz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xyvttgkz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iclfbvpi.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dhstmoxb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xvoszlpd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2svwqzvuv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dooetrsx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gfpohtve.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2omssmwie.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ithfdjkt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2wsksjccu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2caotjtpo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2cbawuari.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2usuhzadz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ofsovynz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yggcvcdd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mnffuqsd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2kmgsznnu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdvhxgrw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2qaabprgy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lqqzsqab.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pynqxnyv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eycuvfzj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wgxvgxuc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2swqvjxqy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2egebwcjc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fxmemldo.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2foafkdrm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cmvnloct.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vzwoepgl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mhsbrnzy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ijdjbcrg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2bbxuzxlk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uazgqdlo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wvhvfuqm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rdobfvid.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xgqpmpjs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tzahohgp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ajirooyv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqwovbwj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zfhyobdq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecbolapb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2lnonwoqu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uncuavzw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ctmjrpdf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jbpbhjnu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2puufsxri.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ooifmzoa.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vcfphclj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zxmahwpq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qlmxwajx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fneqcsah.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mirbhhil.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ruywwsgr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xtuyfael.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2vdinsmud.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2piqaxpzs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pipacifg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2mtvfgakf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ezxftczk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yrsewvnj.html


<!-- 参考信息 -->