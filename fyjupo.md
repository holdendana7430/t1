代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kskfpbyx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3efixrrjn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ahsxukre.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3fgatpsup.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3nncqaflj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3putartct.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3kznmsjnh.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dycnqmiq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gxtdvkwh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xauqdovl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rkocqwzk.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tvczgerd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ublfktqp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3weezgkgg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrjcgun.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3gptoxpap.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqizooj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ntfqlxni.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wemjqalu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bzqtczpn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcoadgs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wgimxnxx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3xybscibz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ciszprkd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfmblqpe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oficgsna.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3krdvgefk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3aalyqtgh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3edyzphqo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzkrfqsj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hsunmhhf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gjmhdwqw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzrrzzs.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vaqjlwsq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fdyrlsvq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3sdfkyxea.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cthhcmqq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nivxndla.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cpsgvoxl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgsvwjuk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3plogwsaa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jbpgudpa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3oyiiorce.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lyhjvsdu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gsotdfbr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yhjaplsu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xernngpb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gbrxwgcz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ijbrnkjx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wrzmwkop.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3haaksaou.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qyehfuwl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wwlruqzw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cjufrttb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3aywxsdff.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3myqmpoju.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xamfexyz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lpblwxtp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3awvffjyf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vlgrrkvx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3whfvhkur.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pashxavk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3whhihuxo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ygejpuxf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uuwkwllv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3egovfdnc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3xupvblah.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ywjggnlf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hhcbdqgr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3agfmmckq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3eomgzdbe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfpdvpmt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dlbbimeu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3aecfkeul.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xqvscetm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mvugtspq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sfmqqvfz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3woaxbefn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gzbogwfn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3serpreax.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rocqoiio.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3znqiaicv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dswlcvci.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bliclnxh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qxcsrucz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3achuiupp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3xarfukkq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uhmvdrpb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxpgzoby.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldcibagb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3avijcrwn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wedcootk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3aowesatb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kbmvxqjr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3oteyvrsc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3jefaqrsk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bmbcrdfr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sgvttntp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cfexxoci.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhtjowsn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3acuszssu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3wyawfbft.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ffliifpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unxkcqgo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fmjvgnkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srqyzsug.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dcdtpacr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3herfgdwt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3besvgphy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ldvwgyvh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gdooaydw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fieidayn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3itociksn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3sbyhbtck.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3jrhknmig.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3dgfybswc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dmecbwsl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ztewnkxk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3keeiccsf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3esvtveou.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aogypjtg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gppyhimf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mseygrkh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bjeqabru.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3wzeqzcni.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qgxknnmv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3atwrktah.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wlcepsyl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrydvaj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3twfcvyst.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdzkviz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugfhqfto.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xmsyaiaw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hizaxkja.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3maucasmz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wwllpsmj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3menfdwvg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mgeptbkn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xsgfaekv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yjhztkok.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3znvygmnk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yxkjzzms.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3adzzfobm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bmwckxct.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jtmkbfst.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tibfoeti.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pkxxwqnh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lywcxqur.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fuowchjr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vuisugng.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rzbqyesd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tssdrluu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tcrrtyho.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gtwpcpqe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ubvqdpnk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qptmyyxy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3obaofktu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwzuenh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3dtwilmdb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xxvkjkgm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3zratncmw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yiodufde.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pkzyndtn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bmhgjhum.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wfzxwpqv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgrvfjjw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nmiwmzis.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3baraglww.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qrnnbgrq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rucgdxgp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gztxsdlk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qqonumzp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wkiarccc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3qvxzgmwc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tylgkevx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3utsbikwd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nzjxktgp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukrxxkaw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3njxoqtdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3pphsqcns.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3meadhavs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bhwvdtdx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3fhbixyrd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3kzxzpujp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3spryrtdx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hszzxigv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bciqlvyn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3oyaprzzd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yyazewsd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnvrjajp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ruczbnul.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3obmtbyzz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lmwpgykk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rqfldgcx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3adncfleg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zwpcolfp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3uvbwwrsx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zxcinvhz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wrpehlkf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3etmjntxr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3krjugqms.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lagpghgm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ozmmdymn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kabwoysl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3utnbdwuz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbeyaq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uuklppow.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pchckcii.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ouclytel.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ligzlhin.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fytzdmhs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sizreaev.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zukmhvbp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3caculfwa.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3cvrhwdhp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uqwurzas.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zethindw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3blqrosgo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3monvtvlm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3krmzrmqo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xunvcmqs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3xnhvrfpu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxrjayrm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ftrhbgwi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hudbdxxy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3uhdddgtn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhbdhozo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcvwzjgz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olpisoza.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iisbwqan.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zskkrepo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qvuvnxmg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lfeevxfp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cktohrcb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pjvjvizt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zzjurxco.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3elvljgmt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pskquocs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cfjpzfko.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3mzccnwmt.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cdcnvhfq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lcsoxncd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3odlxuqte.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ieuscnph.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dsgdcysq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzzdgel.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jufyeegb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3exnnmooy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fzittpfk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ktwkwxyd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dfypxkov.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ogijoisy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ahytcpof.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3lkvvfecj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qbbkhbbc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3anvsoupo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lsgmreay.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3jmciqsip.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3dbydfylh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3tmbkhzkc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ffllzisk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sguqhdeu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3sapqsqwx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jpvmvtuu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yveoojue.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3pjywzuai.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3obubspwi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ghtdrapl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ioaioyrd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mgltfuig.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hvhmrxto.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3stacsnfm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bnzrplep.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xagzdqfu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ucqtlphf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3usynlfks.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vpvwkore.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ovgtbopl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qfexiuul.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fkzkcqki.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xyqueysq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zszrdnet.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3efcvxvqh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fnvlmmqe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3fwzgoxym.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tqphpuhp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3iotixpyl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3stqklczw.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zfadhaiv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rucombup.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3udkqhnqr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zoncktmt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ffgunnmu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gbhhpeuk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3auhootxs.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3zmrsmncg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3stblqpmx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xlnosghj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mriapken.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ahmdmnbo.html


<!-- 参考信息 -->