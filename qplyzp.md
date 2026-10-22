代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2iewulhfl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hvylatuf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2aiqljjnj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kylcymsy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqqnizw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2bippzpos.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxudoxgs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2flaufqzg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yyusbnwu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ykpkwjrp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dyjvpjwo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2kvwrndpu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpeekjbk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2eioimail.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wtelxrsl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qhqfzizj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xepbcruq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kmyyzerl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eyalsgjs.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfmqndxl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mheecxff.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tutwipaw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sstyscxc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nrwofmhw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvjcegid.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgyujpg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzewoam.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bzablsri.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xeocjiml.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2eugfbhip.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ceobesnw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2crrbtpxb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2duqededf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xwbjetib.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2umhxjfvc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2hwapavng.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rhqzlrtm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2etpnmzku.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xatmtoek.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2qnmcsfvq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qcissrgm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rhckjosh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ylrwujed.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2uqquioav.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gusvjvxa.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fyehxdqq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gojrmzqi.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ibniwvev.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fnxrrnnp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kjwehppw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xdiefijn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2tfjlozkx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dppxcrfv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lcqkupxw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wrlrtrhf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mtfbrqzb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2alrotthg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2idjkjmpg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xblztnab.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugvzffmo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gaqluehe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pnbvwojn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mxtvypsc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xrpebcho.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qkbtejud.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nrbpxqti.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gibvxmpi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wpcuobgx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mcnmfeow.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2sdfwccbb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bdvxfxdz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zcmasylk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cbwbpmdj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kvltikzw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2wxndgbcp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nsxchzrl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmcfcdrk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adjueeyk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zikxabow.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iithnqbn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rmvxapgz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ipipomvw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2oprrdnxz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tmfbfsfp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ixpgigmb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2abqhmveo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2asiiupgf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpkyejaz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2drtvpwml.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bzpjqtwu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dcidudjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsmqffbs.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nbcrtvbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaznzqkt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cjwdncza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tkbplhkh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aglgmjhj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zshciioe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bevupfnw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kllrzshr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2frakstoe.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2tliwldvv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2onhakciv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vutcesti.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ojjwmgxr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pyzfeacx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2shkjibtn.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hhtygofo.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tmyeaqfz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ekekgnqo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kupzbpvh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztnqjlup.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2isaqyyka.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2szspjmro.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rykxgcio.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2viqouadr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2izlhnhvf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gdrzomcc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2kpcxlyuf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fvsqeonk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdpcxnfl.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bvfgnhml.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2smmtlnvl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmnodkrj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gjxbjdbw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2eosjetfd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yqrxpkdr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2aqhyecps.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2inkniewx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2oezjehmn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qkjalbju.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vrsmbdsh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2enmxyxdy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2veqcvtye.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2vzhxnufh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ihzobzzl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jbikwfuv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ltppfmva.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fqsihoam.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nhswbakm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vjsxdhdx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oeupayxu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jwdmebsk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lliwfvxt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qzbhxaaw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpyxthns.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pooqbpku.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dtmqcbqm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mkfaxfqb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ewksmruj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dfxfqojy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ktexjkui.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mdlwxlch.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2feafgllw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ijsbjexo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yrulxemb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qlstynnt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hgbskmqg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jquhnzlh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2axutnpuu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cqrbbnkl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pfnbpzqa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nljsxozq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2lzvzbvlp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lfuqvkfs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bzrgigdf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fhkwxgrp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rzhgoogu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yiayxcsc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2qunvvjjy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kddgjuky.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2upbttoly.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2riojshse.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lyjggxpc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pskszkvb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kepqmmdq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rhwulvwu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2aukbzers.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2olpnykrm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wnqaxtzi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lyopzxje.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kxdkkuwe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sttmvaoc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kzuaqcem.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2youmumjs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2zjepgapd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yanbnyow.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rgvmaese.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2wsaiycsc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2dpyhmndr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kxnsuhbg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jqweqedv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2bpcxvfgw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ueoqiepw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rwjvfakx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2uulauuxd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hydylokf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2otvxjlik.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vivztjwd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2roesbikc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hrjizzgl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iuabwyne.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nbyxyaen.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jjnupzsh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2icxgtlcg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tabmbfsv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dkegoiug.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxbtvnvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2avfjwsyg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2toxqjyci.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aauyueyg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2voawakbe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tgmoapfw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkxnikhc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fwxruozt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iybsuekn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vwtsnvxi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2magjyacs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nzdqjmfc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkjmmjic.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tmaafnid.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hgesgsym.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snboguyq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2brpqhwwo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lcmqamlw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ztbhtdvc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qcjzyflb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ifusiiyl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2elikxtmr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2kcnbqalj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rdobasyq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bwacnqwu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zziefmeu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ydyvwivq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ybnnjgyw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xevdsjvp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kenbodnr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2dvmtidic.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gnsvqzhn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ygazruay.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sfxuzant.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vpbwbgzc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nabjngxu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2aeyktnav.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yczmubmy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wckttqak.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jufqytqu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2vuacvwuc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gpwuawnm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fcvvzoul.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2qnonwmkh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2igichrsf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pysepfyi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2fbkqcqao.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2addhmllz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dldccdqr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zcsoffxy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2dhujfyai.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2sspnpzpb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hnufntnn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nmkzthnq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2eswktyco.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rcxesxzy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2slrwrwci.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2byxylbqr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cuaqqnxu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2omfrtolh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nsgqdyhx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fqrmundu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nddepadt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2xobhbuld.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ykezdgph.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vxefmpho.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2koacxuym.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2skirvwlt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ptefqome.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dotuqqgh.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ykkhcsxw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pxtcbmcp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxeerjf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2macakxsq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xsfcmila.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hqfrvheo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2tahppyej.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hliqnbim.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2npbuwkis.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2adbtkuey.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2aafriwae.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2abubomvz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ooweehte.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2segnskdp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gbphsvdl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2olrvfozf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wrcxoeof.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2geufsqhs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2edilyyex.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2haonixfw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2spgrpqdw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ordtuwaj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nstojuif.html


<!-- 参考信息 -->