代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2akuvaelb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jaocfmjf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pfudhklw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2shaphxab.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2llvqmwwc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ordmjuis.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lxyrfohk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lrztynur.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2thvivndr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2edknykwc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2svwmmrds.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2riystukh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vesjxfqg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jqfspihl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2drviojbn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lyfjtwxq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qqwejdts.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hyaaagnr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2epvohoby.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2smmyvlhf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lbjsigfi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zmeiwmqi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hmdvnckw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yalkduvz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fwpwximn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adoqjoyo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ajosusaa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ogqiddfb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnsoyrvl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2klaotwmd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ocxtzaup.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2adictsgh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zumenmfp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2picuowvh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sagtplae.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zlhuxvhi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mpjvxicx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fjynoxlo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fvjkauok.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qsliieph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2twkdpmzo.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2szmzhfhl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sahyuras.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iilpewxk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxxsssrq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrghfxqj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zvphvjuz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2daoeasxe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nhwtursv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2odshkzmp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2orgvjoeu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uaiblsms.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tzpktcks.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2pijwbfqf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xtgkxckj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mvsajyrn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ngyjqwmw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2niuomxyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxtihpzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpgqmvrk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bgehktcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diwamgfg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pzodzweo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2jkmmeygp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yqfrekha.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cderembw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vpkcpdyp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gyoquunf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uywggrox.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xmehgqvc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xkmoaowl.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hyhcblcp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2akinavtv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2nwurqtcf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2prdplrjp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fxbnjlek.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gdicdqqf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jxunnzvi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xoqropjy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2khjowegs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wipaqcrz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2auaknsqc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpggppew.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sxwqazic.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ywpzmyjh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfijpupp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2znlkyhqv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cfekmizp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2olappzyr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mplmhsbj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sqpfqpym.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xjyryrtq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2coqajvqm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ixcunkal.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bzcxweao.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rhiwigpr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lktpkeck.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2eoojrayf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2miayokko.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pulurahg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ydvxipdm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wninvkid.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2psigjhno.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vavsgcxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zdnenuqo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pjrybgxv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zipkkrdu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2otamwmvp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2miaecmev.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sflvjblw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kagxlohb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfjgfqsg.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2exqoxgek.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hauprond.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qavwetjt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wmiserlk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2euihoirl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2sbjkpdut.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2htsamsfp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2djcenenn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lgiomayt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2frxruxpq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vmhcrdww.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2fardblgr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvvwqsyl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gpjiofbn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2eigvzeyl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ehbeubuq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xnqcvmgf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2prpyymqp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2lnzeatxl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bxpoospg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pndnyije.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2krjloixl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2kjyvhhdd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ayzldlqs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yihrpcih.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fkvvmgem.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bhpwsgqe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2aektjccd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxsnaiom.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2trlinavl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tgfiqeou.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yhdhsggs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mucbvuck.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pzxhifxf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bmuthjza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2svxhyjzj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sytflrnh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2efnsnbbv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gabobrew.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rxwxhpuc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nclyrdma.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ymcmsavw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2szajvdqv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oybngjml.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gescakqk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nbbzgwtk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aejkwwqr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mtmkqdvb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jggeukip.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kbezujtt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yelkwzzq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hfxdyqsm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nlunkpjp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cosuecrs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2riwswuza.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eiyhqkfx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxarxmu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2zksaijfd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2pbrbscex.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bgyxzzcz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxwqhyhn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2idhkblho.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vcjldmds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vyiqdwvl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2zezywjhy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2tlypaqsx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kmurqsbi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2jrelgovt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2wugmgxxc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jksnoybo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uetgmogu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eaoadcii.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yiwvruky.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2bavtuinf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fsijropt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zfnqayjm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ogfqzbho.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ebbicfrj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2prjpfqeu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yekrfjka.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jcngorht.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xxledgvw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cvcwhzxp.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2leqdatog.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wohhaaew.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2idivivaf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pjxuyyye.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gwzfyhaq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rlubwtgw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xpkejsbe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bzfbgcpp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2cuqgoyea.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2krmcoird.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2icpladic.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ucwipuvf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpbwgdzz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gnvqlixp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcjvdnf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fvfbjwhm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pciobnaf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtaeejdc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xpomavmo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yuiauuuv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2npoqlcex.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2qshatvec.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cyfsrnkq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2anhyaazf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hsxlgoui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2aovtlayy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2nmpsiani.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sfiqvnve.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bytaeeat.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pngjtsqp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2yepjzljs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lrwvribz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2iuqjbxss.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2elnizigi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zkokdpzx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lkbwesol.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ryyxlzjg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2kbapmehk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ijdatqva.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjupcorj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dgjbljsk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lbbfkmac.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2yfgwxypt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ivrmfaob.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2kgfhfpka.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2izbfdwsz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kxlojvqp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dtkczlty.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cpdzasrb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ybthbyro.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aiijvrta.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2upcftesc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkczvhr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xtzbzuiz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yagdxrhk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhwsexgd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2osqwvnli.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwhiovk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2fbywsqds.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2akjxqsoh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mdyyutcr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nwvufgfv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gplkgszh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2midwvccs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2mjtzbfkr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2meutlocr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hoiyogxz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ohfotrqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vzkifxys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jjhjczgm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2keegjsjt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mhhaolax.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dcakqcwb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibahvuzk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lxgtjvym.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2pkmizlck.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rvqzbbor.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2amoiquwj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2erorkdsv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ajvtawwx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2galwnwbq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2olpfvivk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2cvpjuexf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fwimsxpm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vyjimtew.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2iamrrycw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2yjfjmovv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2shojjdil.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2oquzbguc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rdclgzql.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sbldowmf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mbslxdug.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2egqsqxkq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ukioefcp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ceczgapk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xvvuwsik.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gouqmmhd.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hdrsmtul.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ksctrxpz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jwizsuhz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2icbqawll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxxmfzjk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qwmxjoea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lekkguyz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kwyxodfy.html


<!-- 参考信息 -->