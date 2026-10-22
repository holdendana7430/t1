代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pexjwoeb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lazgrcbc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2qmikrgrs.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fftgdsts.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2eyauydzh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gvstddox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yqxgsxrc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2glwdbfpk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ovmfldin.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ewbljhpx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2feawkgiu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2rzmmfzgh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zkosylnh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2klenijop.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnqwkdvl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2skmbdmfk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lgcqplaq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cymavbyx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yygscucg.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ngesxajj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sctxqmcw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ocfwytxy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rpqccdgg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2qgrxlngq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sflsaxdv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2tfkpmwhk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrtkxgz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rfbykhzp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ddhpwhdh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qxrvbflu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xfbxqesx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ghzeeulr.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ylpluusq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nhiqmdih.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mffpwlid.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2meyurjoo.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rwkmdelu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vlixvkwl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qvbpbkyk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2baowwqvl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hbqzgepv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ctisktrk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zdemmbed.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kdiszuzd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2onqxwlth.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hxnejzue.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xhpnidav.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tyrffpct.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2bmmmdgsz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ioqghhjq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2exuflzpk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2oreyxffq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xmysqxjz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2mkluyqvd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mspyfykm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nnjnofgk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vwldyrbz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrodkomk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bnnrqyhl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vxeqgxnw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zowhbzue.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nuvtgaiz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kgtexgxr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ajomhpmy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2sdlrcicm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2srmtidab.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2veibncyj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vbofhxar.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtpujvfp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gmvfkpfa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ucsazmka.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oqqnzzgk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2eiwaihib.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mtiexyxq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2megxehrm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2brgbryps.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ozhpvkwb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnaectta.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vhbghchm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pygemqwg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rkydfdpb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2abynjoqc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ltrvcdjm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mrvpdtxj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ovmdqnid.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ezrxigxw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2omepqkrv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtjsplgx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2etikigqe.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2avcizdha.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxvxaesj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hevmvlyo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hbqaufdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elcghrds.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pqnamrkm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cliwzppx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kmfzfplv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pzpfmwip.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ivhdpqum.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nfmwznwf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2lnnaogkv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wlsgqbps.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hewrdhyw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gokeyjes.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2uduemihe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2vypntoht.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cbbctokk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cqiscyot.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2feqhcuxq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dqzxvohe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nlgxcjaf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rrdijxxf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2sotkzzgy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zubvangk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ljktwcqo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rcmrqpvz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cefvhoxr.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ewosdyua.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2shisqdip.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gjhjfvsf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kkqsgfch.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wajhifwu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2aqmkzcuu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpbtkudo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ffjjxnmb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2feqequkq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ywmmhggy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2envplsbm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fjmxgifb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qaclkime.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wzjyolrk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uitepmwy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2itsrsdwx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eliikcmx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2aoriftfy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wdntpjew.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tvghqzor.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hhvocbcv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ocvvlpew.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zixccnya.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yuxsrokc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sqihkllb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2irokzmju.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rwuypnpv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jysjjbwi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oekkybtf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2poxmlxoj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2aquyhkun.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2thnweyuv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tzaksnje.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2szmjknqx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2enoowuey.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zjlgsgfb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pjvdwasy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xsyxpfhm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jmgwacxt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2apgykyii.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dfikzvue.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2poxawcxn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vxbpgixn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2myquauod.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2djlvdvzg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnrvjgoj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2crxrfnwl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tjplsdcm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xoqpfeuz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zipxnplv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bzlzmgic.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2buffukzb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2uxmqvmgr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2puhjvkqu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2xuwzmfsu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqslgotj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tzefkocl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2huxylisa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2isogulzc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jktztosr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2skhtlrxd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2enwsrpkz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mpamuggh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fbbuocij.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2wsicivet.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2agaoggxu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qdwpeztt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2aevhjnme.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2sumevqkj.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fcdctztr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zgnpitij.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2rjavwnbf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hnwcepsl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkaflrt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gfhjcfoy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qgjaheme.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2wqibbydw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lkbhdnwl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzjwpbns.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2awhkompr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmhpzhbi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2aedllwik.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mziziiee.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atfnhbwi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uskzqrzd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uyqkqtjp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vanmkdld.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ghgcgewn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ydatzgik.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nuhbjkzh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2geqrfdui.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cdcnbheg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2icjiniaj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mveaujcf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ufooquta.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nzsjzjyv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgeymawf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2feyjzalv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kylfcgql.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kpyepfgr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2puvqhzhz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pciqoxfw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2juuthtnf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wqfumcas.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xpghsjcw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjyavhwd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uttvqdsw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ypflvhpx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2grwxkkvp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kpnhgpau.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2fhctlgsd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qtbyamhm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lpbzlmlf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2famzbmau.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mvkvbshx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2argayqai.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdjdzcv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lnkpavyd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzyujr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lsjkqwim.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ryqufgfx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ippuibvt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xruxuozz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2soiodxrv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btykdjfm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oaoxurnt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sihylsjo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pkjdcgym.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2oelohuoa.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qhqaszns.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2bcwdnmws.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2sxlgxnyl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2dpmxgcoq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwfqjpc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2xzcupvhh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2titthxwt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ttrivgcs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rugeepcu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rynzgacl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vzihpfoi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hfqsiwon.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2bshoinki.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2cgngvciw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jxiytyxv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qpxlncva.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2nhqwkhpg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kljsvzkx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2qlozlfui.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ovyjsrmy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itooxnbf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wzeamfdh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bhcqhbjc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2aawkenfw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2cufwuune.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2wejiyeck.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2femrtaoq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ypowmqtf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vjjpxlsh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bkhlxcmi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pydgkqss.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kjghildk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhftfyp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2asjahpxw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2peeafaur.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whcvdjuz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdhijeh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lpwholox.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gncchiet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2byxdnfhq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iqzmmepv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2utpkpuwh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vnnprdnv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfkbagx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2nlsqvxlh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uowdjony.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hcbarxpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojfjcgni.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hmmumnxd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2safaueuz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sfwrbilt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wgtharth.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pnfmiwsx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2ivplbqxa.html


<!-- 参考信息 -->