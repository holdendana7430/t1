代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3teaksnkv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lwiwanus.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fxlarzju.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3wuyepbej.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kroxtmxa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3goccclbf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yfzddkqf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3klqbblyj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3xxyrnafj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3uxrwwkxv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpzcaexb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3gcykrdir.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lgotuzwq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3akjsdqye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3irstxmuo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yryouxxs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3itahlmrz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wwmitcuc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3weezniob.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dzmxhgzb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ggjpqkch.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3imxtfqbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3rpwryvoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eitnkuzx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ygkddzdv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hrpznaox.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nxobpmrc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xwdehwpg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jmadqpcb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qmjfmbup.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qohitllo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ogowpmwz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ndtqikik.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zbvathur.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3mcwnphmw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mxmwpepr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3reyamglv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dqinxvqf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pbtlesds.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mpebeugv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3aivdgtdc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dsltlapn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mshynlpw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3obnqazii.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3opxodges.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3etwvdgcy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3knmxqqvu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mnvnmoio.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hxfkifli.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxqivxac.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3iwhywkdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgxhjk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkpoifzf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3juxivksw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rdmetkkc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3uvzfermk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3aueixpks.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3sawkpbje.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3afktcpxu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dptjmdeo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzufzyuz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqmoblpb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ahinwxhs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3huprrykf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sgppzyoq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zsoxxrna.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xwywqxcl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hyibdoyz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3drrctlha.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wvwnuhbf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ugfzvntj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3grbwghpy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zfsyiqby.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3vorbnnrt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jhzvfdzw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hcngykjp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jxwyopyx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hbzufvvz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nombvyya.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3anwhvgqm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3igxgunol.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3urxaibhn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ezigldzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuvelfmm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zbbrihcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owdngnas.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uqpmeqvf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ndxugrzk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tpiksqwl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3noqzzlyv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ibuyrptn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gphqohmx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3wsfdpcmx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wvjushql.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rpcrqmoz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3fxmeufok.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fxcgpdsc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hdplzetx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kbgxevkx.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3muxxshga.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bwjbnaef.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtnmzuu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vdgplrrq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3phytdnfi.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kkitodnv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rcparvqo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3exbwpxiq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hvstjllu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ocxiwmgq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3czkmgxet.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sbznmcwe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hnazuoye.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qiwiqsrp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zjjvuuow.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3weplhqok.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3loqqbrzo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3esctuizh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3offykcca.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jdvsrvii.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ututigim.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgilsmxp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pxdhhnnc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fqvbxzkq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zfpehcpv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3htrjfnyb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jhraahqo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jfafcuqn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gsbtnerm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ijjtjmho.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aqryfcqv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xfgpixeo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3epvkhcpr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qeiuddxw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mubcyptq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3psphkika.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ywtszhpe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fuceyysz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbjbhdv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fprmhztn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3clactihj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fygrcuvk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3cvyxyibu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqrssltq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3owtizpvt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3slktkcuz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3greebcbi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3likuvsfs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qomgukxt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ewvuyiou.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3skougonk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3buylduey.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rukyyzfl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3nbztjieq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3czozofdw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3roujozvv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wuqryvhp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3jlqlmnpo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ybvjigft.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gtkgaruq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pilstyyq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3grtxcfjg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mefssfhm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ilwnywml.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3redveepd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyukxoae.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wigurjia.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xyyjiryl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3elwcsveo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxdmomp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kgugpcah.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lygiojfl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iwmdkrnu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ymidcqjk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mfxwwsea.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vwwnkfxb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jzrroxkp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pwucpvlp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3fcgqckpp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3msakagnw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fptfrcky.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ogshitgu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3stdtwkmf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlxpmdqa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wndbnqnb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vpdknbcd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nyjkwrfz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iwejqsut.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sutzeaoq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sgoozteu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qiidlseu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gcbwmfeu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3woihiwid.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tuqgftdr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3evcgedyj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3xnfqvpgj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tspdrwwd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3clzsnheb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3umacuctl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmnxkpen.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnolbwjj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3haxhdjoy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tddjitzy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3elucczsh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3dfapnszq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jplczejh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3byumebnt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gtnzlwng.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3juophkuw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3yydiupcu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rzwmajge.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrabqlac.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ktikpzsm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wbpwnchk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vjxbufxj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vwwjzbbb.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3voqgywmm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mkdjmqjt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3galfungo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ueqioszy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3wdxurmto.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xwswxbod.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bovgkazu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbzjzzbo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qnkkcsoi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qyqheykn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kxuowuws.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3acuarzae.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vzfsedel.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tehtjwnz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3izrmnvng.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3hdqlsttr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3exefrzdw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncfndrnv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzcqgho.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3kzdfbkkt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3prrducvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eskbkeau.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3icasyjqq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jikyiqbx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3danzowln.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3jbywhcpr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfapegt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mnjagcde.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3akhlzytj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lebqobww.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hwpzivhz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hetabvnw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ztiitbou.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yrrwhahc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3colgeedv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3kilojnul.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3mymufmzh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3aispanec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ysxbqgab.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bstcdodz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3mldbvofa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3vlqhcgxn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3efjfjxpl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiqseqjq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tzxvqzot.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3axrrgjid.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3twntixqk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eowxkxxf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rehnzrch.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ajaqkkfn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vulrzkvn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3mzpnymmg.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rbnyhxee.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kxyamatd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkvkgog.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hycqozzg.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oomdirge.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mdejfevm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvvdqrsl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjfwezq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qkvomacz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tjpaiyan.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3lpugalyl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3tfejfece.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ovlwlmyd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gzpzpust.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bqpsatsy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3yiopvuox.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3sbegwrqs.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vnokbhxz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qmhiwwip.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xchkkahs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yahwqwiy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uwbmwmji.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lkbkkusp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pnqyjlil.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3inncqoqc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3shhmahtm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3duslcuwh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rsygvxhm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ztwbywty.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vdupohdk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tyiipohi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jxofyiyt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3sbapomhk.html


<!-- 参考信息 -->