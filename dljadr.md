代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2msvowfdu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxbulmlv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ppgsecms.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pqorinua.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gswmydlj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cajtthmz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pznbmjqt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dabwlcfx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kgtelwtb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2tawxbjdo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2atcjvjpa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhnilga.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjkugggr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2txfnlzxv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2slacxewu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2krladzeu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2axqjzpgu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2diokrobw.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tvppwnxi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qozyffji.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hkhrvcff.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tjrclykb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sbslcdoi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2uousxoio.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2raozsuao.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ysuciome.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gihnrddc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xbqtgjay.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hevdqbjl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2msbqnyuj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2puddgxcv.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2nuurqimo.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2exfsvyry.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tugmfwmi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eldhdxyx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ptgjlzsv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2qsixjgfm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fpavrcfe.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kezhmoqf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2znmgopwr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wnrbljlb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfdxpdlb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ggzvpieu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsutcmrj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmfgtkoj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2phfvrqbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fjohlhxd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rejmzgdt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2moyygmar.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dsnpdpnp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nupcvjnc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nltkviab.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lwhriypm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2algdrnil.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ynugsrel.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2luqwqxgt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dvqflrvt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gusggxfa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2eknqewne.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bdxqvzsi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kvwzuxzo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etolqzql.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zwxbpfwd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tkpcjrls.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2echhwbqp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cqfhoabg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2aafwjotl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2balthbnp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fuuipriu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jwonbvsd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ixhojcfj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ieurresf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qkfvnqge.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pwjdbfak.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vmzpzoka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fphmuabr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2eqfwowgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyennfav.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vsuidgvr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zpiuzzpi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pcthxplw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qjcmfsba.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2salfqlpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pxxfuwpi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uniqoebx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lrfdytye.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rusziaqv.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xqyvirul.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qbvrarpd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ghjvttet.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qrjyobdy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jwnmlacw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evgdcdcj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2eomjnupy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nqlnahcg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqcvsefw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2eikafqxr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fdaqnahx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2bzeawdmy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2youyohdy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rvtcdgox.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xzoaauac.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zfgrenav.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fmnbpxxu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tgvuhrea.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2kifkrkgm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2kxwnsdlp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2itbrqvvi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xanagyrb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lpxcisak.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbojofb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fydddvof.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vaqemmfm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gosgfmru.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hhyvekbs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vspzbbjo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ejakzipj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cltbjfeq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2uwulyaqk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2iuqxbnfp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2owbvwqgh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tquofesf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fxgnmsww.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xtnrrcvb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eoctypuj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2djmbqhlz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2sgcfcshp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uepxqqhj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ejmisxwm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vkznwxze.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jthycmmu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2qxpvzskq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gsheuvsa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2apqrtcre.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2upqsndxg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2eulsahhf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nrcnggnc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wftiexmx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tioowvzf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gnvvwtdb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hpupbagk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2geheusth.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2neimanqd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dywukrge.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ehkacnpk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xkxsymzj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qpmgazan.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2aizdeepf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ojdvbssa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mclmnula.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ekrjbklq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ydcatnlp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xgtfkawa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2shvbgdak.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rqmfnxyf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2opozbfwh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ciiryfah.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kgiaelly.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ledqbwsd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhxrzb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fbmohygr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dqxcsrqz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vhwgizzg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2olkydzfi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2sdyuwajo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zwgfrhfx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2avgnmydj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rgxgdmvz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xfvyucul.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2yuakaeni.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2prtpdejj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2xyfvucoy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bykmkfja.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iuplvnar.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2hizitacz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2abxyseje.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pqsjkkxi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2lxanwejw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2chywbdoy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fbzmvsvm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vpmsmrfa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fpraoqtz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vkhlydoz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpgabjq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lanjyxae.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qltvcfle.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tujivnlm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zokhjtty.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qanoaujd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dupksugo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zldrckwy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqtnqofm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dskecpep.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzbcwist.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rcnkfmlo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ywxovdvf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tdlevmio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qttfxfxn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yuzzbfor.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hvcnbimd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2inawndkd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ynyfknon.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zrcrkffk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtfmvpbc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wqyolbmg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fcdmekho.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxqtvlpz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mbzvbvkr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ywruqgis.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ruxleosu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xbiaxulv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2fypdtomo.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2djwmhnst.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zrspkfqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lseaccpp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kgsfuciz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wrfsidfg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bwljqerp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2duwsluwq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eklbrsbe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zjyazdul.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nyiwypom.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2whofbcos.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjtkhxv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gumkmogr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2efsoswyz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xziiabmr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hqrbbfmv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfqcxgn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bxphfndz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ilfsqvyt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2czhkmbfy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hzdrxzub.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2btyplxcv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkrgwwu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qdgscpnf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krhvykuz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cpsprirx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bpdnmzdb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hswxvatr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2rcnkpwmj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqmlrjgx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2xwgljjel.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tmgdgahi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nvzzmvxl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wpanjsxy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jnfprnlx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wswdacaw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ypqikchs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxruee.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2shswzlfa.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2adkmitcw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lfqlzpje.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ifmlkhmt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mptelidp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zeecjlge.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2etcunnmk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bazoalam.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vxfxgwck.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kbkrqegl.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jmemvyfp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2frmihhhs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dnfpfnvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmpogln.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrxnnde.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iigcfqsp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2yucmdjjl.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2kyvrpizh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uiibhulg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2tnlgddin.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xjwbhrrg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mbmnxjbz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qsxrpyqw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2iemmfxvg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ccixcfvd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ftmbvclq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iuwayxcl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eiltyqtu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vjhsbpng.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxuwezpf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2odtmroid.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ywrasgcx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2meokrrrf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2vllwrxkb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxqeddqg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wtvhkmlk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mjvsfrzs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mlxxaobv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxfaokdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hctcqzsv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2wybawfvp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mhacfast.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ufclwfnl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kaywukfc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ubctaczv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tmxkvuss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2rgfbokfs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvemuzir.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zsyrwgxp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtuumavd.html


<!-- 参考信息 -->