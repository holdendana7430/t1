代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2iyqgejpd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vsslbvjg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dzijtenc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wftldgac.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zwzrzbum.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2alzvyqxf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dzjnlscn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ljhdbidt.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kkcumtre.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2sjggfnso.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2unhoajjh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ugmgfxyk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tsiqnhjl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bywligfj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wjpehkom.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2umxlbojj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jfnxdhmc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cwhpssvk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ywpawvbq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tyvpikfa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wbqcpiep.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2weezbcce.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nwleiedu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2eibetzxy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vpbwajwg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ppuwrcdi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yvsxmhwe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2kvsusdov.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tpqprjmd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yionxacg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ceokqien.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsioxktp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyhkhwzm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qgnahiez.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2scyfwrzq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rnyqqhyf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2axiyfsoe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2llbiohyc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kfbjrwzl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uvctqybr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pchsmkap.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqjfvkyj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zkourtpc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bdafefir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2baxagmch.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2svrkeesn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2zinsgorf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2eqklbjuv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chkpvwxb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbhmavwi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oueiccgb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zhkicgli.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2saitynfd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2obgprnjo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2axtieaxj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2djabntyr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vcjsgyni.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2zlyckcsr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2yeadgeiq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2utagcvwp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zgsehlpw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hqeubgqh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tplumpyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkxwufmo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fmiqdwui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ondvflzl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cgjwjsmx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2uvmnspiw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2dgrakphu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fcqbaocc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2juejswom.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2khryisim.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2velkpazt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2asomggcu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pkpacwas.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2shrjjlqu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xzyyzuxt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jcasrouw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ztirxsor.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cbjdvpgn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vlpvqwpi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2toqntjtr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mctevbwf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mlklyfii.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2entqennu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lrormzfe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fruvrxjo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2llxbuzcw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gjhlqcyh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vlianoyg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2dqogmalj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qnrlzpep.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jkyuzakx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bknvwllf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ejjwzpet.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2knzlsqmy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bnlvagpt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dorgknqy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pbdngbez.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vhehmjfd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sypxdzga.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2mbiomvzk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2nqumbati.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ytpppymf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2brlbgucu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nubyyemo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sbwocxwc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ezussemc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lvpuyydi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nnnnutls.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oqwhjthw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sxubnigp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fivxokyl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ocnizijm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sazzqnxg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ausnussw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2cuvxlcla.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yiseaqnu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2nhtvtmzf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xvapbeue.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hntslgys.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2wspypyin.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fowgoohw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ipfepotv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vtbfymoo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oqitggaf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kuaeijil.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2smkfqxlg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2beocymgs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bwaetqwd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vtdpzlfo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2eyjrkbeb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2igtvvsho.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ftirgnol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfrravam.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2thfiflhg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2luswgjee.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ryvcgggl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2gspgnlwp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vdulctaq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nqrhwzou.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ccycfpey.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2khilhnob.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rfvrqjnp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nodryqsi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2omblzsyz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wvjoeyua.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ticgrgya.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qppcwarj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ojtpmeyt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhehpqw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ntxecnyw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cbbyzmdw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rmdtxfre.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qiqreray.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rwvaaoqm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2gyybedxs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jglxktwp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocofseap.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pmsnadtv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rzthlnwc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fnswrdsv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvstwsjf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2eduqdjfy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lvsuwjko.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gzgbzctm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2udfqzcya.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vlqeyger.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bgysyqzv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wsmogejf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2unhklnbi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tltxfwjf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ufuabrcs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2imnowgub.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rgltmzdn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zroqtjhg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdiesvsy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tlqwurqp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fjdlsict.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2lilditzx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nqxltbrc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qlmyjuym.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2przquyok.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hqawsqdj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2evbkgwee.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2undovjwj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xcynppuu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlqcnznm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fauidffh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gmxfkdlj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2fhzncazr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vrsulpsg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jjxnhyyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2msrochfd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ftrvubst.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qgtrpdih.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vemnbeat.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2waznkvpc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vsigjkhj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cibdrclv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ernxjtvi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2iugilnik.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btwukfea.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mckdcmmz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ewrfzewt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndhapelc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lpgdytoe.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ovgrhtef.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cofgtgrf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gbpfjphq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ksvpfkrp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcetbqra.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvlkqpuw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2qhnmdgqb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nxdyjyfp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2sreooyha.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jtwaisdz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ryomryet.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ufxpxybk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kwsphwax.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2psoxgerb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2izbtsjjx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2uxtsqoyr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2lpxvcvxe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2dnjqkvpn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xwrhpgit.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hkkhsebz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zmkskerh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wouewrqr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocxxdcpf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2cbtxclbk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rqjilnqj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vfcdsryx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2trtjahfs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2voobfhtp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ieybridh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vnltqhgo.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2isolcfxn.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jatselmt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2jkkiusun.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xycvbzth.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wwtwpaje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2efdovgdz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rwhibpwy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bmxpggpy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wcefwzwb.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2frhvtckb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mwjefkpi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zxsuggja.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nakgnolr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wagxymmk.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfiieom.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gocnjjer.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qtmfcisn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojibjnll.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2narheezd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzzweuby.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ycxqdqpp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqhznfxs.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sispbaoo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qhbmuuxy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wyseufyo.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wolydnob.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2oghwtmgy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zphnqrqg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kcphdcar.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vojdlxex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dvquqaou.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ncttptzs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2nyzrpnih.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2anedyxnd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2efwzgyvg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zljrsrxz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qbthlkuj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xalctpxm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qljvdysz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2kqpvglzg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pbzwhvft.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ojpcybmf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2lfdecgtl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vwsekbef.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2zzgnhkqu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2dzqqfyoq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xoqomepe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fcflywsl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycmgzpmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2bajbhukx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pciacikb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fclgsvpi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2seytwsqu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jcpiaymk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qbpufjen.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wmuhtouq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rzzxqjzj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kifmhltw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dsgdtnoe.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nyuzrcqb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2hzjgnnao.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nlyfolmn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmdoolu.html


<!-- 参考信息 -->