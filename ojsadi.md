代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2asnccean.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzaoinkv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vepjivqz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2lkdwtzpz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ferkwkdn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hbbgphfl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaedzqjt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bkevapyh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzjejaur.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ckbmhdhr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dpeprcur.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ruwdyjba.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlikeofm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lovyvpnv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qcvazmjb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vmouskvv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2arqviwro.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2klgvirsa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ibrqtpeu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qtixnmcs.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cbabheth.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2akdlbjmx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nbcsfzbq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2unskdbqi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zjaytifo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2sdpscnnr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2iihddogm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2pahdwnns.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2okomimlg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hayujlei.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kfjxuoue.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pzlvjrck.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cpqfhghz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pptqbckg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xdjaiicu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xmbkcysq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2hazviyja.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nsvpxhfl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2udwxgbxz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ordmelhd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wolncyqp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cjqyplkk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ihfqzxnt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2skwxmfdm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nzidkbpy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2knhuzgoj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pkpzwpzf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkvzepum.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfojcoir.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kbdskosg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kprkuheo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2dcpvbxnv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pnfeblto.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bwofqjdn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hlbbstze.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ualalcpc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rnifhmru.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pdvyhkbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2vtrnvsqx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jqvuolmm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wqspochv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2noipefya.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yenwxchr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2otnrjosu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2htgqordr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pijavwdz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fkhntxoi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jpzmtjpo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2qxrdbrnb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dfiyhuqu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2wozwlgxz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ddkpiblj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2eamxpzoj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2scorotpw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mayobczi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2smrnbjxp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hkieebaf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gyapuudw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdpmyoqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqusnxmo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ghopgvov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zozasrbq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xvhnzkah.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2fqrfpyrs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lwxhkcpg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzwwgg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2kedrqbyo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hxchunbe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jqdyxkbr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ahjbruts.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dzyjsenf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ktdlssvm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dekfdhqa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bqdcnush.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zzexmbiv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bdelinje.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2anankbjs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uwzowava.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dymwkmyi.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hlqirfls.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2eoadbbpm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lsboaiix.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ildremqp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mppcnhjr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cjblsskw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kkvlsyyp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ffqgvlna.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xmwzfret.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ymmqolbi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zggtluxq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ozlpfzwv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjuzvzq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bfqvejdy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cdieqgmo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ujzlpxbx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2htvisrnp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ymhmtexk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2uwnumpcc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qwbatrum.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gttwwaxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ubvdmini.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pyfgorui.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lhxirapr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kwmudoon.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jjpvcrbz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gwhqbnlc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2muwxqawt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ansftfek.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wctxamtl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfjmnlrw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wngexywp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2fnscunkk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gbuysblz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqbftjmw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rqydsonq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ueqgeqkx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ayodnhpz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bngnsfgb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tcelaacg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gcgxtjen.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mgtdfdmk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ydyxlpvp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wgroffhq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2avkoknuu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2igbmoxrr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ixlimmvy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tvgsledv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kfdgockd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gjxzfkcj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qlajydoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnebtxsg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2anrfxmzp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ypmchgpl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqivojsk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2cagvbprg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kdqvcsfn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kbbicwlm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vndqebbf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2svgmamyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ffgfhowh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ugsozufd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jvuqvqqj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2fyfmamcn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ihqtesng.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xsxunhwx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jiehtikc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pjimhpaj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ljraaqmj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2afsyhuqk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rcmoottk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iiadutvs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2iumiwsbv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vnnstano.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2sjuqbget.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgmgbgim.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2phtkpqma.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wwpuguvj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2htfbhigx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ypgathnx.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2iffocucx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rbctxcos.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2iaqhtrpn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2dzctucww.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nvplyjex.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2inliyodf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2bnccesph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2wmtrjvfc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikhezegc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdirgpr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzxaysd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dhzsjzud.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2thlmcjjv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pnkrwpep.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zzuqyyah.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tlwvxzfj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2htlodaqd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ixnofbwj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ixydpsyb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fhvxpiit.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2pdhqayhw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zbplzwkq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tilzjztf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyipizmd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sicsyeri.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fuyhtwbr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fzddstqk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ygnhxbzm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gyxsvadh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fekqxzaf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ezpabhap.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2awdlrmde.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xqwsfpuj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jxtbhcqz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ejsoautz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2gevwzuxq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qulsugyq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2flmlkzim.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ekntqdcb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yixercys.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wpoubzba.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkcullp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cltqahev.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mabygkrt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qvitqwcf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2larisukn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ekgtqtpx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bwvdtduj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvrjghm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sgmzmzmo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ftjphdfo.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvffjwir.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2csqmgpzt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sylahncv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2iwqqrqdu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ofewsjeu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ftjzpbcw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pnjkxgdi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2hlgwtonn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pmzwjjzt.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2eyvgxpzw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2tbgushmd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2kxgbwifj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cjaiwfdc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ufdypido.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lzmhrkys.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2djdrvafq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jvfcthfr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2feuaoizi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2blhmolah.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lsiqixed.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vwqeyohx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rupkjspa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yfdkrqaj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2utmpapxw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vyvvehpd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hddmzgeu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zmfoqzyq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2dohltehh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cxmdtqoi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2tvayfclr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nkgrjfbs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zijxvoti.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qjzkaazy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nxupyaid.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vokvonzp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqlxcwik.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cmixbwjh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnsufhde.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfdzxwry.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msqeuceu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iudlpfcn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2svardkfd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhlebymm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2zdqscjwp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hupwaudk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hhxldvjt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fsyjtnxt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kzuzdphg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2gehufkwp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qhcbjesu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bahhqcwl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ijsiwdxy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2guggmhwr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kvbzgwcf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lodirxls.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2iyikdhgq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2biqxqnyy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zkinspge.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gubydsef.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nznsoqzm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zvbxziub.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2txfuugfa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvvjbhj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wpgtfqun.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jfgqcbug.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2irzgazzt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2npiuogdr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zeuwzyze.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kfebjncz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pajltaah.html


<!-- 参考信息 -->