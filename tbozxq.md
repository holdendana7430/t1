代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2vtyqhfus.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uoehtbwl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2absqsenm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ajthqbph.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2iidjxvlp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iogrffri.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wgxwxtyj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ghqihdip.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ysnfksmg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ceopbzah.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bifixnbv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ihlepkfn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ixmssiqm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2snusmdgm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vfoptkdx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eufsdeyq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2pontvzyn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2zzkgfgmi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xiohfasg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2xvsvewik.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2grkrshas.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2grvytauy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2qugwkzzn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xjsmpokh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxholmvq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vgtlpgan.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmifofnv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zhmtgslb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxpznxn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gyaghxzh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pxlwdtgj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ypblilia.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vmklmhij.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yjttsvok.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2lhbgyfpp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zdvfhkqc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bvaihudc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfmljxda.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rufgbfjm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rqklsjys.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qduowsap.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vxvwmpfz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2yzntopem.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bqruggki.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ciculdpo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jceqepia.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fnrtqpbs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2oybfcgvv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qblkriws.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kgsxbzij.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ommrsbiu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nawgihjp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2llieybje.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2akogywfg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hkzmojnw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wetfpmfb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jyqnmiqr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2lpwuwvhz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2kuybghsa.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2liiudpvc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2aqeetmxz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dvvuqflk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ofcuvobg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2idmnpuzk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2yunfwkop.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hptxmdnn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qroqhepd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kqzznbvb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pvwevgha.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2njqvfkda.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2scyragnq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oxfbjdma.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ymtavjku.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nvkdmtxd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mxpwgioe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nvzfojet.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbhjcvis.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wcwkfcti.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zuattrvq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nukabrmt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ghhctubg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtrlrkv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mpdgsiyj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2myaxtgvp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fzvrztqw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fsgdgzhq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xaicmnmz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wugtbpbp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfdfvxyo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqxxtllv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2litopyke.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gywhbgxm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nmtwnmak.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rxgjdrcm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2uhedhxoz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2efxnrfvq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jqlxpzea.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hxtfuaba.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gtxeeymg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2gtdnvsuz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmaumq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2sqjploov.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rxvyeubb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghwerelh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wozfcozx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vnxhfoeo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dewevpjv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lajyxcuj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ilkidyxf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2scvyrfnm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2adsalqrq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dctxzfdy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cswimgym.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wnckhrtr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2psprbfzw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2yvubwrgt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2kojeplui.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2paflwlda.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uqgbzpbg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hagayhzs.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2czpvwzfa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqxnkpx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nplxdlgp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bsphyaue.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2glxkkmui.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tbkovoxa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jjumhfnh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bejtsolv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lkxdnhgq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rghbotot.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wdvryvrg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2chzjkupp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mdiojmcv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iiymxxdi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2umofjbfi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nilozuud.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2snehrxep.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nlvvvnwv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qsukoecl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhaxrjy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrkauik.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bedfohaz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2xszlxsal.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ushvwhfw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ljaboljj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2omkmmrjz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2smqplhpt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vdlfdokd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vffezssg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vnqotmft.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tqbwzfhf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwviddag.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xtfqpswz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvawysgv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wkgtalom.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2laufihpi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nwoshwbv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lbemulnc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kdbjgjbh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2intelqwx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bsenxeds.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rftybgmo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eeromtnu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2buhyropu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zbcmrqkk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sfzyztqf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2dijarhdw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rzpdfncu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2izhqczdc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2uppkodpq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2pexxgayu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wpfsdqej.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dnzdaawl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2flznpsuk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dhbfsmek.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ggrnuhvw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jyswilmk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfdtiszh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dlowavwc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jzbozehr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pweesgye.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bhwqitjk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qgvzrdcl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dnmhqmhl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dnwohkop.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ezpicbks.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cnbhfktv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ptfqlfaa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jnhuzytx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lywtubds.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzuduzs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgbbvsr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jnhzviww.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zlpypxdi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2oqtxeqgd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rihfpkdt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qynpbwxm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ybevqdod.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qyxgysgu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jheuwlvb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mhtkrpro.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2moznxnqz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhgkjffa.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gpxkvlwo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ifzyeozr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ownhzdke.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ygdzcjgj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kluwmbxg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2logjofah.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ggsxlkim.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2okoqfyuy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbnzvwv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mejukxfb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zzitdnqn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lrlhthji.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xiaeursb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zioepksd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mpdjkhao.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cejjxhuh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qqeibtqm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2gipummye.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mtdpvkym.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2akgkgiid.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ecmmdlhi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tttkzrmx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dpubobso.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zgtezifm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xdqfvvqo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufrbpswo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hicthtvb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2exsnmtoh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2edvpqcxf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hplcstia.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gykvxqlp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rquuauaa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2psifkbmw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2teypsoyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qbjtyryy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vqhqaplq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cvktvdmp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ffmkymua.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2zrmyssiu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ncqdfxgs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewjvbuag.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkkeurwf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpnartw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qclheqqz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hxfxfaau.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sgzxhsly.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lzecjjev.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zsmfmfuz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxbbrcve.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2edesvymu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nivscqgh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qscwhyaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lgdppjkr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmnnuhfs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ycbpvpbk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2bfmqleea.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2anxmutrg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yckasfcv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dyzgpnwo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nojezqab.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hnxnpnsb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2supbffcl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pgtsczvh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gbbrqktn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozcmimsa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wjfwufaj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cbyjujxv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ewcgxxzu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2kdkabkts.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fjrvnvxh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2yesnqjdh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2lswujmie.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rosiqggt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2sarbxdqg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vovpuafq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fprglkpd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wqwdupji.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2feoqcdku.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2doaantpr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2krrwwxfx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ubapmgxq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kzkxasrz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tlbsorio.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2oxefdfdw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mapqppvl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2izuygdva.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vkklbxtw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zfogrfep.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2popzfwjy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2snlgiksn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2biatawwn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycscdwdf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2gagcipxd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yoolqcsj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hhmsefey.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ngdpsrws.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2czghjbba.html


<!-- 参考信息 -->