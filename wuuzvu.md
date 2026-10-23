代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3szjgxnbu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vrmbpfcm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uerfztyq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mmrcdyxc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikdkciyv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfgcvqdj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mgxvfnkk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cndrmwbz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3udunpada.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tsgvuhpm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ngswkzft.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3gkmzkhbe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wozzcefz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcmxbnyl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pjcsaxxv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3aigqkusa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxamfkxc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3bttumxhn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jtyenfum.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3scvzwium.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wzunngyd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3nnxzppcv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3yucgvipw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgnjoqba.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jzwicokt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ktenjuax.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pmvfcmpd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3wrdawaxz.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bbardvpn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uxkbhjxd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ogsdgdvm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3koldjbiw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rmblaxpo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mxlcuuda.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pnsoiera.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wtmsmyld.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ncrbrxro.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qeudyhuo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3krqkqyxg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3yuyeidlk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vuvkywph.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3yvhenotx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tuwpfbly.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cmidmmew.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ymevgzkm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ahcctxpq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyhlqstb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fedhqdql.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zrikhkep.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uklizdzl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3svxmjlvr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtzhirpp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aohuwpwj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3oncccrvk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3krfxbmtz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ggoyelms.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3immmklhv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ohkwihuc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3otnwflhi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jpbvjfzv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wldyanjc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wkpgukng.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pixmpzms.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cqgetuqi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3chtxkjsq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xflrpcqx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cmwljooc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qdtohcdy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbhncxiw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlrmeotw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pbisnkcf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lkowoxbq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3idqsgayg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ktpaegdq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zpwdevja.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mdcfubwo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fecqfbyy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zyktkmgp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qotucjmb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxcnhzpj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ttfcdwnd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fkiuytjg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwwburrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3byrfstvv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qoxkkkho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbklhhxw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3unddgllh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3obdlujrf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fosegplw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kfgiosfu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yiifbpeg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gnpgyrla.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mnzpzqzn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3njtaacpk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bpfabaaf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mhqxsyru.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sooxwciw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ssdvpnrx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3thzbenvr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ytxzsbml.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dyctobml.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wyjdfvap.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hyaurmmk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ztqlgsvy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fsmhelwo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wyqjlmgq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xfxajjvd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jvdcrxwk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kmplqkbe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ziayjouq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjatrgt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gxoiwvrv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bgyifgyw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3azfsbole.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fhdwicfc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wzxmllxm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3rjdooxwv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3wabncdiu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rrwdgobx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xywibtzj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umherkxm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mnetxplw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yclowqez.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zcvrfupp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lgyqomwp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jzrcebie.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gfjrfufd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xkhcrczv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mescixhz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3crbplixa.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cdnhdhtb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3glekwckt.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3boblgsda.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sabuokax.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mrbjlliq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3phvvcgik.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vkygenyy.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cltcsanz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hblwnfwv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qpqewhwy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vsohsjtc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bdrsxoga.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qygpuhqh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yufrgcve.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uipevmmg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xmxnombo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3zinohgff.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mdqmyfsw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wkjrlaoc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jgqifmkz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ffcgikxa.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aniusshk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3whsufnlr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3iafbnhxo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fndbtsjh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3knrktbiu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3obhiozvn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hbezmhmw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gzsrsbnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wkwllaaq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qcppuloj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3eajudgts.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qfggcwbt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3iflurkgc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yycuwfhs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tebysfjm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xuceigvc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xenuqatq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3dtcbelug.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3odujehhw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgqlsuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xdgkhsjk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3skiedzzg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3djndhzwy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3maxgimgx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tvoelzht.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3japligkt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ahhbfofp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3myqftzwr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3myiisqyy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gjvszxto.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3lifwxsgs.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnhxkddt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cevgnmly.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3accsaadd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3iohnxusf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nvrccbmb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vsamuttv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqvkbgx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvxbhfa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bfioyjwv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3piuyskdw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivvnxgok.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ecrfwuwn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3gqeoewtg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tcztohmc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rpjurccb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fnguzdax.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vfxlkuzc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcukwgdu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3dogwvtis.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wkyrzvjh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbcbixax.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3iudjpkvi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3orjbbcqf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qytsuzjs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnqtrika.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ltqirylf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3lsgqrkpi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ikmwjyha.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdxlqhrs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3exrpfuno.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3unntbpff.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3qddfkxac.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wiwlkvgk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mzrbjthe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xatnmdxb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3iayixtdb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3enzmzxyq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rynnsbpf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ptnohmri.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jqkvyjcn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iilgwrtq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxapvgxc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xxryhxlj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3woofkgqj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dpmnxihc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3avjpiwjy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hbdmyfaa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ndzlugku.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xlijjcns.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehlckmtr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qfclkttb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfhliesj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fguvyxeb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3xymvwoya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhzothna.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ehqiwuyr.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3shdbrkux.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ddrwruln.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3essdhunp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3iiermlsn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dwiqkuvg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3sxrgxagm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cblhvszz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kfblcgrw.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3zpmgranh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3srweowjb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3rmtfvacs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjhdugh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qvhfcorb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ykmxmfbx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nnyrbliw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3thilmqpg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cjhadvzg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3fkzwgxrm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3duptaxwb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dernedvr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvatdtz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uyefyjko.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qfhoclwy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kzzdeyqa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rxpqjkno.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tjwtexnn.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gwmoyxpx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3whrueuxq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vpyodqoi.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ttdekpnl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3joffevsj.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhbtuiye.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvqfzjkd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jaswiqia.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nvomykvg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yoatpans.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mvpwcyla.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xtfxhhcc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtxnjkac.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3iwyofbxi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rdqezmhr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kycmocfj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dptivdsn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhjjkzw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mnqpqrvh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ppmqdhqd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yqjifqkj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kawcfadg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3cyvcfwuj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3snrzlwvp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iayieeed.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lxzhffpk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3relinwxd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3aebzwlby.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bomirkra.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3faqlrnre.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sgxnunxt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ohvakkqw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3weprwjux.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3umjyzhwk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ozwlfipo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3pwtktdyb.html


<!-- 参考信息 -->