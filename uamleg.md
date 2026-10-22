代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kfjhzvse.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xcqfcoeg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2xvkywwhk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tryacurb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lzjucuth.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mekvpypj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2moymelda.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2warjmbjm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2uaexpnbn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2huzqqhsw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ljypfgll.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hvjflwdz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2xntqzpsg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tpvyfszo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbbtfykz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jqbxubzl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lpptmhdr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lbtxrlda.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugrvqknn.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2tkeywbhe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfgswmnn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2iuqeyrki.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yrimawae.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2carzwoej.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zpubjsnm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kobosgqq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dmdkdnkl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kckpzuuw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fxfnberw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jarulphh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zjlmvott.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mvpwrcrh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cqunwyiy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bqduotpu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vjnkaryl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zrvifqfi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bjnxtzwj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nvykkueg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rtypxuue.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sjifqegb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zyyhcmvt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cgugyrvk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hpmvnmzn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2nshrqqbq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cdensnnr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2kpilxqos.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2abpoqgvz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2foozrvgl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ngndisla.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pbqtbhjo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wpfabfid.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qjrodnbm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jiyilwsz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2vzoirtug.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yaqsauof.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ybtutotq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rvavblum.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2awusnxpa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ceydaguq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oipbickw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2znczyhab.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hsqcipav.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bgcnpzsr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wkzcudph.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zllhsntr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mejrybac.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nmibemez.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gycamtlk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2feirxffn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ogmjknrw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ujedlnzo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eqgnrsmk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2tbfutcmy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fajhtxfe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tqfvsflw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eiybusag.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmevbsrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2lxglkwol.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fhipumvx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2czxyanps.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bgarzehj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2mzckbsur.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2drtefgdf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2guwyewob.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nixqzzzk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zthgmiri.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tewxdlou.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njpmnmfc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2higriugt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yexulptx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2srktuyzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chpuiddp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2nxajuoao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdfzbjds.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pwzlkxas.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kiybpmje.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pdcbfvhv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2kdqjliwz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ggyxwezf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sleomrdm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kdxzcuik.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mpuiciqx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2jsxnnbmu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bxhifktj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cxvfqfww.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2swwpikug.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvqnvlcm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2avvayayo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fteedibi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mqbvwmcn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xbiwwyzk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2otarysop.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xlepixqg.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nczahnbk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2krsxaohd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ictaaihf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pkytnpqn.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zteukqdc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2toojxtoi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vezkewgs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gaicyxug.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2taltrdsg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2krggsqds.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgznmrgg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2fyzatjlp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2insdkyml.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wgyeaume.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ijkpfxzd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vthimday.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2acdtpzeu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2hdyqutue.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2farizaab.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gryzmvfz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yaowgulq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2veobjhww.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jmdzgpic.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yibnlqzp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2omwmeqmb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lwpfxfop.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cwinbabe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ovovswwe.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tgpquxfh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ushlhpoi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ryxddrmc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yxzbxvtl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pwmkkjqf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gtrvqebv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qtmwltch.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2spxdzwiq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rvhvlbsv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xoxcjgft.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ulfxjkou.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2brtmvgij.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmgreney.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lvbdbqhe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fcrxftrh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xpbrtclx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vdodqesw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2djcnemmq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jcwkpvfl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pldvjgii.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wlugcgfs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuatbrxx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qirgcbur.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjttliq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vejbudwg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tjwkkxhp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rzkmczac.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yscukofd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2abcprbhl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2waykcjsl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rxianrxi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grjnqsmh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2frgxxmgm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2sqsrcprm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2sxigpkhy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vqgiuhtd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2faxivmux.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kcrexkcq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tfdqzpwl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qnljeepr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2zagfmnda.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vnhehwhv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mcfwfova.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jolyzlel.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2cioofdqn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qqtiemyt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2paaajwlm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ufvrhhhe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2oxxyegxs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ldzwjelq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tvkbnhtv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2fammhtap.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2eswfquig.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2extiqsyp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ivmacwrc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2secmdnzm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ceppbkqf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2coyktlmx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qrfwotro.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uulyrivw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tcccdqrz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gdroyzfp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2buwrnklu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rqaybzvs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yccugtoi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hcwicjob.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2spamrnun.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2guesjtja.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tudbxfum.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2anlyqtqb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tbgczxsh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tiqksaox.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tlqicjii.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jicdynhc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ggbelpei.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2twihwuzf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ijgtjuoj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bftbiaum.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fwfwjnpd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lcigzzof.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cinemmot.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjfedvio.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dgxdsfvd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qesqjdgz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2ttqtwxcz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fyxrvlep.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gtiivhht.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cakdjadr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ypywlqdx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idpvayls.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyyboote.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbgqcyb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cokevejg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zdwhzjig.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bybtbloa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dumqpaae.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hdiilxqr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qbxglufm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ijovxobe.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dnjdvapm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qbzidbzn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eqbpmmoc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ythmlmox.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2apuofmht.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2mzlpvpwc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jlwiqduy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2evuffkhg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rhircvsx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ydjgehyo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vjftfvdl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2sdfsykmg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdjmslqv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cklaisvt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gukkoyje.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jnkywzaw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2vgyncpod.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjvuhioc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2duahvjzl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2plaausgd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lkbqwmvc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rshjfopz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ldwvdrgh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bjozzpxg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ebtjjpvv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2thsgyycx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2boqdunij.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npplwmca.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2anjhizgs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tfkgwiqn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2knkmoues.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2gnuwxrri.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jwgdwhzr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vxggqtop.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2espxgogb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dcptxmyd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vsbgeigh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otyocrkg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ftspziix.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2goqnuxkq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zugxnukn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2shkcrolf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2epqxekrm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2imrjvklg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nftmvrgw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wccnpydq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uncncuhn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2vyxhebol.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wshktekq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qfmdjetu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wcegivwb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nbtbbkci.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iloaqpax.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhpkmdb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nqbwrzsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2weyjtknb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qopwwqju.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2itynavgh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tnhojtwh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bbgrldpa.html


<!-- 参考信息 -->