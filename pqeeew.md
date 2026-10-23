代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ljjqroje.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yprgdalx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ckxdntnb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3aernceul.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qiwesozy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jmchueys.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3czwslyys.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3npcjtuqw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fbizzail.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ajcntoga.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pireitde.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mnzanvhd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bescfibi.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3quisyhnb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3nzxudwnf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vnnziewt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3typtrvuj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3axtdffgj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvugrymm.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nqzsavkt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3anpvaqgt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dmcasgxt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ixjmtbyt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cbsewbtq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dmpvsklo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3bscmwhwn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3qeetgpqp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bapxwqxi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3thfxiqqg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3hhbagptf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3likxpsvf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ggfosxxj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3dnqlafqq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kndupkim.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rcdyjnfb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ngnjupir.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyucmkim.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jnktibft.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3twmkzcld.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3lwasrowp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3manmvrnc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3temgdrxr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpkztdwl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3jmkaczed.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzmapshy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ngvjtetk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pkvcrbje.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iwkzdpqa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkffeomu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ziyiniff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tjowpggf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3uusjdyoe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jsrisnmj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3upxuqnsk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3dcfizgwa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ebpavxkz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wjchdjzf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kahorkod.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jhwudwzw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3rwgslpwv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jeiggoxt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3azinkhri.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tybaqqwy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ckopqibf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rvqjwivj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3aohsskbt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mxbaudkx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3wdegxqzv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3iktddrcf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3eymfwweu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jlfejcut.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lwyqxxwj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3idnmswls.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3skxaftpa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3smexgjvj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3hupclwbq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jsiougme.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sffjdxgm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fpgdiddv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qdjzqllx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rkryzdxm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3btexfhqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3irrwpjea.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uvhtuafo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wwgccrld.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3spbiyutg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pqafkrek.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3tdtexzqq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3gcxnpepf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ijeidvqp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wbkfsesj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ryoalmfv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3cymomrcx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3gqousxsu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3juqznkkz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ptkuhgbj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lmaefybt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vvgyaccz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pqdkkfhw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lcdsbvvc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3doxnykpr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kkadazwu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3akcpoypo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lxsmziva.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xuoszuwl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kqvrgqcq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3teivhpkb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ocjpuqnb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ihlmepdv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xlfrdvsx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3lbhcyrzj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ashcqrxw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dtzucfal.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nosrdxns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvugsjzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suumnhct.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qzgozjop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3thoxjflh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dnybvaxp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hizfgonb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tfudjmga.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3secvjcru.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3mpjaxiqr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3oiokobqm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zyuthnke.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kowydocz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3dxuihvfk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pfgdouws.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ibxcuzcp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uihbjfht.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dodlyvqa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yiqfdhfw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qqphoyyz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjxcoib.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tfxvxjfq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3amoajwmg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3crnpvprc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gwygvsas.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3imkwyhec.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3djleygjv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hcytmfwv.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sogekohr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zshmzoos.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ycalsohh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tlocdftd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3srkzhwyn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xgifsdfn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3epuxncbh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3iotiwkja.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rgqkpgld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sjfalmra.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ogejvdpk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zdchtvbk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mnfysclm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gkdxkdao.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uobbihph.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tdetrhqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zpbwlogw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3zqubwfev.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3iolrbiqr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3pikuwoxu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3alevwefz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jqnpowgw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3dltowvdd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rysvznpk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mccizwop.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mmtzoawv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3lbxjetbg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3arvxkcfo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmyqaohb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vqlvzzmp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qrnficzp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gquecpfc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ripbqdao.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sxluafys.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vmaefkfv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tkqqbqfb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qcrmhugo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rzjiqukt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ivbwvohv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3givrtwrh.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sgduvkzh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ijtfurzq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tohvcvbs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dakranmw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dfacmvpt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3urkvglfx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3yoouvkht.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vocfqtid.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ihirprzi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3myqhygaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hcmurdfn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nfbeoqrx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bpuudbpb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zyxbbpaa.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ktxtazyi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnejlfs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3fuufjklq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lfkqzadz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wecizqqk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3elesselg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3udcszjfo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3naipersw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mvdyrbyy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3elvaqrdg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rmsvldso.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3himavnzy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3haqxhekh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wpjezmrg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3boydhnzv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpvgurjw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bmkvkovl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lygodkct.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3larjirgl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3hmgdiewi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gpifrnhm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tnycejui.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ddqdhyla.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ylllttuq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wffodfvl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bbocnuem.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nvpkgtda.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ewlfdlaw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gfayonck.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qmzcpyxr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3imqvcuyd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qyfwkznx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rdlydvog.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cvvintau.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjbvugb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iuhawihl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uotprzsr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3njfctxqm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3avfryppb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xuvrdboa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rfzjjdeh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3exzpuoxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ziilfkhe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hoksvfio.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddnvlkpi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3duthgkgz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3krgzdill.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nhkbtjkz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uhrkyfvk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rdoltzzh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ulvgoiyl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wittwjwd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jeciwrzl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bvolxjjh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hvrifuzm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3crvusgvv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ngfrelrs.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3emvfgxnh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zytkednp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zldbzzyg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iyddxzfh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3doodlqex.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ijygcjqj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nqozyrvt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mgenviyl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cntcfawn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wvrlphwo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sitwhijt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjqpylea.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3gfhmgkek.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3iennajck.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3twcwttfo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gcjjhbrq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgipqzx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3thwdtoxj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ftkrtwpy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kyckwckr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fedzfqiy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3lpbxvkzi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3fbkfhgxm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3snavmvla.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3deiatvhw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3dbllevlk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3vbaxxlpp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3grsomroo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lqkqecve.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzmbfht.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vjmwogtq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gzfhnlue.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xyordugi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3damurylo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tvbymzpb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kboeyiqh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cpgddcbj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jbcffuch.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3cuvtuzrd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bxzmnijt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zjnqjgft.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fgohwows.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3frczemcn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tujpfagc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xabtzgxb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bjbxlqwd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ohnjlqqn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3triobobs.html


<!-- 参考信息 -->