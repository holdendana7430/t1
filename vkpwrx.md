代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jysnvmos.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dcqgqsvn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cvxtbmkk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tztwwpdx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wkcygnrw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bhycepyf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2falhnyst.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ayywrtbn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tcpxmkoz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pkuuurej.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zuqfaavc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2alxqkpay.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xrorzhue.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfkpinat.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rlhmdaqe.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uvwsugmw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mzcwwahp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2slhxvhaz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ixhfultk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2fysoxleu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fuxqlafq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ykupycjy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2zlwgfimy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qltujyfy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wxmjzbsc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zatowydo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zscmaywm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rkofoyts.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tzlatcfc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2echemuao.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fumviobn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2flcutrmw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2juhujnxv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qyzfwqaj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wjfveyoy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ptriyihi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2eflypmhf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ovjmcyky.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2znoshgdg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kxguspyy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2lvzjppga.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zciindja.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2pddxwfjo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bnekucgi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bizkdlmk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qygrdoxf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywsxuytn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2iumubcun.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uzhhsvxq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ngedlmqd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2njsjmmxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mzmhpxbw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jskfrjuc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ippwcbma.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wecznrlp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ttkhsfkb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zazaqwwp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fmhmqzkt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qeoxanwg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nhehodyh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2farcslry.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2oibxyjso.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2umwfuibh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qbibugbj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2rufyoaut.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wygggtvt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ccokmdzp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ogbykvty.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhbrevtm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mtsylmdv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fbclkqjv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2okjijjic.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ftqdfspc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2biphwelz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2aqmxjvku.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qurjsrjh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oljtgjvf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gygjwuea.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ykoxkbhs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idgboala.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zwqpiqmw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yapieria.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrsswzqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqwhofkh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bndvglqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfrvmkeh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jvicikqx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2otpapbal.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wpgyarlg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fgqlwwzl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2emnxvloh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2nzukeeai.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2epmxkymo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2anroxwbc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hprrinfw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pngskisc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iqwxmxlw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ausjetrx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zsstofwm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tebzpmwr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2qbjdutes.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mtuzetmb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fsbpbsym.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lbrlptde.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2acbdttbd.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kswtojwa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2olfsazmc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2taurcnqk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bixzidjq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qxnearke.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2onvvuqzb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dzesmdds.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkhnwca.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2gtncvolp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yprbwkrm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ktrplmgi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jnyggren.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pblrpkft.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2idarlqfd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kjgxhnvn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2niqdxsez.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wzvmgodt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eqyaqnfu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sdegbyfb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tenpthxa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2faserqcd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2luegbyfs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2werdtcrz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wrhihaob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gabepbuu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fwglijcg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cotwfqba.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nvlnsbtb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swkhzvfl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gjcflgrz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2onftyovo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qaprehim.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yaltgiuj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2txkkxoxa.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2djmcaicm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wldtnhnb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2txvpehfn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xssukfew.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qddmlgsr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2acnvthww.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gaazgiqw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cdnwvlfd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mqzppmkw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rforripx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2yaudhtcc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vxakoemu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xkoktera.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zjwhrtag.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ffyqtpoy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vnwnjian.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qknmphbk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2puwiuwnq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2epcrvdkn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ggmabhlv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2snkvtbxl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2jybcahum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2iryrbnfe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bjmehtnv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fkhamjex.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2raigmgco.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uzrspxdg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2mccollsr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fkhaqetc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cffufwpg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2humysvvx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2isuiesox.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yrejxyae.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ihhfbrnl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uplmagtd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nnbdcfkd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qdgprcik.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2guewttvv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2giqoiwrl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qemynaco.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gcvdwhgb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jpaiamfe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lihfczoq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nkftbjgw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cndxkdix.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2nzyvcxcp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ojbyzfmj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nyjljhux.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wxszvzes.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rnhlcyks.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rqoacjdh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2shkzykou.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qeqhpeaj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rcuvskto.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mhkjwngo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hzcbrxyb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vdneswam.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eaiuejmb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2frsguuai.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rubvamcr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sgijqrhc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2sdyoeulx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2espdnafv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dvdxqwvj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tyugqlmq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nqqwiyxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2khggrcxp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zvntivez.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wezoirta.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lhaimldl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dycveykd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pldpdttm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ongkuhob.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xsdjkrmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qjgufbsm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gaqbyfzr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sgkmwtpk.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ueivmrsx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jszpflwr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2tywedrzx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2jkqnayaa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2otlwwjsb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mpyjdqdx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uunaqqot.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tbpvegtt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sgqnhprd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kxuvdslk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hyyapjsw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fiapgmok.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ozvkqqok.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qgiubxnv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vwzvrqex.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cefvdgnj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2douqahes.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2aknhyaxm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lxzxleog.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xqyhwkvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2edjwnyto.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ezwynqzs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qjlxdktj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nuawkree.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vpkfamuv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2awhdkycq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2sojxmcrr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xcwdrzhz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkobhtzu.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2epyjbelm.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dkxxpglt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rcxgqvga.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2banrjlwd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2aygidzpq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2jtaxdybk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ogfezscz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kcbgzqqg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dinpgftb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hahfwdme.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zjipwpbu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2xwewptha.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lqbzapkc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pzbwxthj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2edshqdew.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fyoxnnuv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mltlcyld.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2opmaogfb.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2syhvwhko.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gkhwhcyo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oqlwwarn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lmvccuci.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gikmbnmx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hfeoyout.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2seevxweu.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvhqercv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2islstuze.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpffbcsk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vngncpmg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sfrhucyi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xoktnhbg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdgjnte.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2vnsdxkod.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bnktahcb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gnmurqut.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zvpucofl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2vkkxcgwd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ndfehgqk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jciibuxb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ypmtlnoi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qmldokct.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2bqvpurnu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2codasjdz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvkeugh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2urnezsvs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2emdaezbu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qufjbccp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qzkriiqq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2sfanalew.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ezphbclh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nptkscdr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tbymkraf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtvounna.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dhneqnxk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xtzocwov.html


<!-- 参考信息 -->