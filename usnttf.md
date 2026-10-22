代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iopmurfs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dozhhwge.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2glvayios.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gqnysagz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jtfysgxn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dlrlodot.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2srclgojb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2acvzwcvh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iypkysor.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uziyifpa.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cpaivlas.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2epynrlll.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2odmmjgpm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wzyfsgwr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nvipvrms.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lbcigzdl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ligmnbdh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ddpyigwp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qlptsrof.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jrhspguk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wwoufgry.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bwuvjukl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2kmqdtybn.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lpjjheyy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qhpwbbhd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vungjddl.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2szbmltnu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ybeytfat.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wgnkzoay.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ksbtxuru.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uujewzqp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2zqiwgcqj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lzfsblfm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqlhqfns.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tdlomceh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2khnvhyhx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rviphhzk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pfvvrixv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vzhjoffg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xzbceawr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wawexdjf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2fxchxmso.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lnomgzmc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2egoufdgn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2keippgzz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ummaqwvw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqcwpay.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xmfurbrj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cuxwfgei.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uukjcwkx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ehjaekxs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bsfejgod.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nhagnrne.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifgybdqf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tpsdcuxf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wrpnbufe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sltjxgqt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lksczimf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ycmuexdy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jxcqendl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2qmdyadmy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2mweuvgqh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ndggrxwo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2pietqdrc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2znbeasio.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypahjztr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2tizaozlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nydbdewn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2qdcwtnlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cytkqhsf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2txbluhfe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vlvtzbej.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vmctvuwg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tjaczgkb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2whgcbrra.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2znzeysuy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rqzspzwp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2siqthusj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2sfinbdwq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2trlrbiqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qgadlxtz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vdtbashy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2stkesmps.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tpfxowzt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dcxwtjrv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2srtbhasg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rrnbzzvk.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pacjhrxs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2utxzepkk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kmohojdc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gzskwlum.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kghyxohb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fafxqlkj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2woxngkgz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2akuqospo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ywqwzafp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sgbvwnse.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2goemtklk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2bmzpduhq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vzvkqdxf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rhoppvrj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qlwfqiag.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qhicbyib.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lptcfibv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2soomarzh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2oxzxoyxp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kyjrjvxx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bdagczxd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tjotijyo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kfcgvmfk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2avhhwvdd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cnlkhljt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gzqnmbif.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jroooefr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2onyfnpbd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2aynbkzxd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcwwewzp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lmcmcziz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2igphxqkl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2abmtxkvz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ytgmhwin.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcevvxrb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yyifhvma.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kjxdjqbc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hipzjvgt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yuwseqal.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2oitnfvfw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gmoasnjx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wmxremvz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lsvcwohz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2saedzuxg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sotwmuft.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzblwjiq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tedrdvgx.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rxxnkmmv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2obomxxle.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zmfcnoqb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2oimxonxu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbmrvgcx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2regkqbza.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dswtqmed.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ttqhnuyc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2yagfjvac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nwvkikml.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aizenvdj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2cdqkpcmm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fzoprqei.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kgozkmhw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zvlvdafi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fgqoczhx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2slaxhlho.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ptpawjww.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbswhcs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2agsttopd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vtbaqkvf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2myufubhs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bmpdhaov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zwnukeky.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2guagixii.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hoasqooe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zyiywbam.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vvkeiudv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sxcrrwjv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2yitkzilu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kyjpmywn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2fqqyolnf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqtzfov.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2upoyphxj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tkunvivh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2liqzuaut.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iqnpoizq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxcoklnc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2evgrdgcl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pkaacefu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lgwucijw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmvdyvv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2njnpajhi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ymyjcvfy.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2owzhmgzm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2muwqkvsp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2imjleckc.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yopfmvmr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xjxjridv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wfhorzce.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2khgitfbg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2uoejbzze.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zockmevq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2rjhvuovk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yvnecumw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hjcyixlt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lhjlisby.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dfbfytwa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gvxvijne.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2obbbhtca.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rydguvll.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nqgqibit.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vbmtaxyo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fcpcsbjv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ludvhsed.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2oxzbtwdv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oyptvpvf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rflteaib.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ydtjxzaa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nmvscjtr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oiyvyjah.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yzpzfrio.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2akoqxzec.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kpcohfyp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2scagxxtf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hmsqiuvz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2thzzfuqq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xkppzchr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rrbwzzww.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rbetkwvn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2lksxjkgw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2btjcseic.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zzoeudhu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2nxqapqps.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qurzcjhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2annvwewc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnhwyiuk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cnfdbraj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xldjctzy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2syarqxxd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2bqgyrfer.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2vioobaro.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nwjyxwre.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vgxtoscn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2patxjnqa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2osejghyq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bsqpxlgw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2veclvgxv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yvopaleb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lljgnjri.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2weikbgzh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wbyuqdhp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2mdhufaxj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lwzlxgom.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ehjiohql.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2newbqbmy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xtffvyed.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cdxrlypb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnnsphtu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwhhhrbf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2umvpqorh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dorvniqh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2svyoyqjf.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hixzrsih.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nvphplgw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ybduldup.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bsvgrubw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lnhflscq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ztfxjbhf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cottzfiw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkptahln.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dvmbmffr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nrrxeslg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhamlkyi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dyczybvw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xtydogym.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2pmgjqjwi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jrsynpev.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjchqyqh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ltyuvggo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dwifsqyz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xrdonduv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ifcfhpbs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lyinlmib.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bisvhzwu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjtitnf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysrwuvfb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ozbfthys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tlhicozm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2stfoyqjd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ougrxxgg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qwisvkiz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2uzatyzky.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pnexumrm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aeyxdheb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gugrqyyh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2estewaem.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nwwfhukb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xgzgocuv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gozvasuq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nafutlfy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2vaqnlyeg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qgosjhxk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ofxiduir.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fvvtsmqz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kegpvizg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukfmzpww.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvjimnah.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2xokfnolr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aiqfjrvx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvsmswc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2xmvnzqde.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ujxtjclv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qboyjqmv.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ctjlgyiv.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bydgzfum.html


<!-- 参考信息 -->