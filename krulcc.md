代发 wailian999

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lzjyrzhj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ihuqshja.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qunijddc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2whllrqui.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qezujtim.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zigqbtla.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gbzlgnfc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2srwbvqcv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2aackcoty.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2itldxzfu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bhygqgze.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2bxlrzird.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xdzonsvx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2antnvpwc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xedprjyb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2angtozag.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2egrhtovp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2slkcjwhh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ufhmfixf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ukzsxhrj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ofeipxiy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gkvngtrs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wtdwvlwo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qidneeqs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjqcxjmz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xvybqbun.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2euratfxl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xjzctkzp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nxmbitrh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kqenmuzm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ljgphfll.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mefphvcd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2kyzkicqo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jatbfgyh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eaulbwdo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dxiubong.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zndvoppb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eoeyntsh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hdwolmsn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fdqbsqtv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bthvqnyg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2qwafrjjr.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2prjamebr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qzilzhtc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ghiufrog.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pffyetmi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rioeidea.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2elkmnics.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cyyyitok.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vmkfrmbb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cgtttrpi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfhiwhsp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2expzmqgp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kngvckwn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lesuvdvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipumgpzh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lddnrhvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erkizvsb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yrigyqmr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qhcnvqjk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yrkafswc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eohfzpqh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qdmnnhac.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rjqubsbr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2whqhxqju.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2snmuhucs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2iihadggm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2dhaltjcx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2okpstxbo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uaowgdob.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2smempsrt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dmtjwckz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ilmhaodw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2swvtuuwl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fybopupe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ndcjbwvw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ojzoeowg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bjveshna.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ahuyjuey.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aenbxwxm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wivnlcld.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xjpotfdv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2peolzpwe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hzsnifoz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gemvnszk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jysjvhll.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cvrkfcxu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2exicnauh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xivouutn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bbfyskkc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gccutabz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2plgrblqj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oqbkdzvl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2slgxlwdx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2euwtyddb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nojxmplb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jvchncad.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fkuhzetp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bkvmeype.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2fefbpiux.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fouspnnw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yqoyxstd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wrtdssyw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tmwsycok.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qgokmpmv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhowtfqw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ldyagtgv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bxxnqhft.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bbbjffot.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uxcabisj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aojakbdq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wnjtwarc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2xkiqhdzs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2giuewoow.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tfgdtokc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2imbtobvq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rotphcbx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2inklnlla.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2mrhfphof.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jksaeosm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2svofuktr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xrisfkhn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2isfzccuc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2idmfmibz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2whrnpvyb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2eolzyqmo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2segnrgzk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2flwcuwwn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fynttiwo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gcyrldgl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rvewxoda.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ljebpwno.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2aqucqusu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2xzpavauu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dsxdwsin.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2etwvhxnv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvipruqv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ebsgadmf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uzyafdoh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wwsgbkus.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2iwvqrcdr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dqdxpanf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2voptujqi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uslxrtar.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jwiyqqdk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pyqjzjot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hsemvtut.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dixegmlx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2syvhpsqb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mglpsizz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lgsunsqe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ndzxster.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ivontsml.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gokkoflq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drgqpkxw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2auzxcxgf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mqqhzhhn.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2djvqmxlz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lncerwff.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gjvchbdg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eyhrtysj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2djnjiggq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2uaoiyxvi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohmprpqu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zknhxgsy.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2xfspluwh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ptcxzqxs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wqfnffnr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hetwgdoy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fkekmgwa.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vppqbpwr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rlfhgltu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2umxkclyg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2meuoykxz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ofunkbuq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qvqoztyq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uktpgdys.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmgtozxs.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2frxbylsd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wayeyuzj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2sbwuekjz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fgoogaxh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2idnftxfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2trjocdly.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qhovuceq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ryhajzkd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tjmcukgz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2redrvbrf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mrrhjpxf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2okyobiow.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jnsilazg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2cmlqxlwq.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybklrswk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lfcydovn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iasvbelo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2slqhlgoa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2zstbtuap.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cyfstpga.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vichipsl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2gxtdrlky.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wdtrlivj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yodfsaww.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jcqcelzv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zworbhhy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eokimctg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2reyjjxnm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grfzvcje.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wxrddpya.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzvtfqjf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2drnluevn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cgwexyrv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wqvfgclb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sfggbhep.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yxxogszj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ujmfjqjh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ehjusjxj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cqsttlbs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2tkacultg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2xaubtcco.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ggnxkidf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hwjcbdwk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwnpbalj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2goumlvan.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tubrgczv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ebryumse.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2emphswva.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nvvzbmbm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qtluljvj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nyfkjjbg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pjznnwjn.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2dozfqtdj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hzpxumle.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jvbjflmk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uqewcywo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rwjgsdub.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2huwmcchc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2dxplneeg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2frvtjtux.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wnwiwxvg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2yshbjyco.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2juexidhh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2opdffxku.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ftjkvfsn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fdfinrhz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqhgbtsd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tgrhodzg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2btbhzdcn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xsgpwaak.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2edscgemj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hblziyrq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2txdkhhdm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2alsktcej.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gfkzhipb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ipztjdyd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2brmwpzia.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ywoggfrk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bsgiidgz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjevzuvi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lvxuycxo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvosftxi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqwitaei.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wvsvhbhq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ymvminrx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2romvdhoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dghlaegk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2sblvdbnu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vzkpzndg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2arhhhvvi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qacphmmn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lpdbhlvk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2twksbxwf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xcvepeqa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2gojodrcd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ujwtjbjs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dllcckxe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jmmyvhsf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tcfjdhae.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilojzbsd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2djpjduho.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2zznkgffv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ilipyucb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2waljkdyn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mycfrsok.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ojpkigbf.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iybucwdq.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fcxxxmcw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fwitdkkp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qcfofjzf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ecjbnorz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ectzqrnt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2adaaqigt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xfakbelt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uocwhieg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fogqrtkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edyyhbib.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hkdsvaen.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zkhdujof.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kdbwwjjk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2grpkfwvz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qxyvldnx.html


<!-- 参考信息 -->