代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3srjiywmb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3leicpexg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dimdxhef.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3hbfascpp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fsajnuld.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sllxfmhu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3oyklgwpi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gsmxmjex.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3fphqhstg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3dlvajjwg.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3pcsslzbf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ernnkjla.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ttzodiug.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3szfckluc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mctisyhb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mcdttbja.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3atpbykes.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uusqseqe.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ewqfjrkr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vkahssgi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3shztnocs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3adctedsc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3baruoitb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hutdnrqg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dxdqaokl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3uhtumcvt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dblggsbf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkezkmiy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ijeebeqc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hccsfrhc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ilkmftoa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3obovmelx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3akqxddrs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jjrfvhkm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ruetsbtp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nvzfliqg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3htofrdzf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqqqzujb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3urqnhmwp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dgqujcnm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kmvqowue.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lzoxqumw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pdvyywfa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hrdxszrj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqcyqlee.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhytipvd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tlsgmghq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ujhnquse.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bbqxqmzj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fsdxinpz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lljxstfb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uejbcfbj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mlivgeot.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dimckzao.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jplqctam.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocvcrqsh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3negckapn.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbmtyrtc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3llcjlclr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkvqwgpq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bhejhmhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzgnneei.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ywisyfny.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ovclzwwh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kzlwqqon.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3czszdzrh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dmlhupst.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pcylceps.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hqexjumh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hfingglv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hyfqtazd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mldcsbxv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hqwgqiwm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dqsrnryi.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3orkzpubz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wmormhrj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jecoyiup.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3eqwwbojk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zcwprbjk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lccegvwa.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3slochnue.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3axttgzyq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qiugsuww.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dwuxnosr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vyscuwxe.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ybotdssp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ulckyxrt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ngdaobyq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjtcqael.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mfagmbit.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbaywrp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3osqbtega.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ovboegkk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rlhgtkll.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3zomgmifd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zcikneer.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3evvxjety.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pbnlpdid.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3fkrawqsb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xpsrieow.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ndoaenfm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3oedjfyah.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3sautetyl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3agrfvmyy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ngolefrk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dvzkmixy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ugfpksfn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bfcifwpd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vyzrwkal.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zzbigjuj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xymzuuep.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ptvyihxe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3blzudjnu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkcezkro.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ndvzjxyg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ymegjdjq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3khgjtpcu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ieusecjy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mvxxquyk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dgnriuij.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qzucagel.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fdfbgaus.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mjjzjrxo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kkljabbq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qmdkuasu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3jtixqist.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3pmpbhowa.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nevinupu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tfsxtoqd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wjdzhtiq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3olzayldd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lmlhhjep.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3hvtgaieg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3egxgftlj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3vgtqagkp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fwjtwtkz.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3uzoixfjv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zqlrfvdx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3srfwzqgp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vkkxdtzr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pmnskqlz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rwinfblr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3isofqcbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mwxkfklp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lgdvknec.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dymknvnx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ncswjefx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3suujznbr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kupddebc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rkwpksji.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3axcairyy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ogzqpenw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xsjmgsmc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xdksziya.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3satmpajd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3patmhpnu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tuqyvtte.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ieleaawk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3bofvnpou.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3urzjhvhp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3elqsqder.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3kyyvrlew.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cckximfn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttcxzisb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rcjervkx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yncoalzy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3laigyuws.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrddnvvm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3umzdvxxw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3xrctuxbn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3qywnkcbq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wvubjclb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jbpnqoiw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hholkttv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3foeyrjdh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmqcpvmt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3mcchrnug.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sxxdnmsx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3thmstweb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ldrmxhkp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yabrkfcl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ctmvmckc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ztcvoand.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wxqwndim.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3eswkosfn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ysawxszp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lcumzdog.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlzfvtiw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3bqfmsywe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lqbnzhnb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjmvcvqw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3zvztypnu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jiaelzor.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jeyvkyhv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yznpeclg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3prrqdumm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nccdwumw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3akotilct.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3latlxnfo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evfxhsvm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lprkrxzx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwgcqxyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gylskjhk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3slnzyzok.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pnwdogse.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wvetyjfm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3omhlzjqv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nugdaymr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3krreasau.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yndomknk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cjygkvht.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qgipmwfu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dahuhlrr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ssmowkmm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xkyppujt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mncihcho.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wcmpozuz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gdqozglm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3shlchlkc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3queosiga.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3egrxehsb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3cejzkeon.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3uwdtxmkd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pvfvhxcr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ytjskmng.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vhxjxmyc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pzotlohc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bleqgdim.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3knmpxdrl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hdulraxh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dnwkanfq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3azyooypw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3jhyrmpzw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fjzlhgmb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ueyhwqkw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3njcpnsnf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3houvfvyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vksbweio.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3ejvefowm.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wcgvtuvt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3tdtimrom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3shxuqein.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ezquaiec.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ddoetstd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzmsmkv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jawfazvf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwxwnqsn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvpmlaeh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eqrhnmqn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jksckvry.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rrxgpnkb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jqyqvovu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rufwpzqk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dfxaasjq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtuacjlf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3psxipmxl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3tvbewrnz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nceutcob.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vcwlquml.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3akcgpwbs.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vtpimwvn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3msdtmjxf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ottfrfcf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wwhkezxp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kihkphgm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lwgyvtsl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ptpdwkoc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yvwgjsct.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3eifkrpis.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3grtnfeue.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kqckzfuv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pollnkez.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjacqx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qpjanrfi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bwcdfdoo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nlofyfyj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3edkdppeq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fsrrfhxy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3nchcorbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3lnmkdssf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3lwguplbl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhastco.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3zjbqlcun.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iycfkyvo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3seyltwgs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gervwdcu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ixbhiwni.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3mzlbzqym.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3oxcszxec.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buqsmuqr.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uujvrkty.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ggalquor.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gktunwcw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3jymsxcdc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vzqkvglr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jcgagicz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfkpuiry.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3tirmdfjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrqoshzm.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qdjtkhkp.html


<!-- 参考信息 -->