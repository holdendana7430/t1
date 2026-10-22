代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sgdgyfvh.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vhznntry.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tixnhruz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wnnpcstq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tycbhksw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2wpjbzwzw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2xuacpnxx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2goecnlnc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mhbbclwu.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fkmgonlv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2beliorpe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2gfpvqxch.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2lekhbruz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iexrvalt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jdffxqhc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2njihbtce.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zjulqbut.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tgteshhh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2bcjdpuxz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nmcssrpr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2skgyhanj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jofblccz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2idwiylxn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdfqfipv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmeiykaf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xudkdcoz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2vwacoaeh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2aiwbpaew.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vniidccn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2dlrikigu.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uhukvspb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vdwyxmsj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yankevge.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2juxkjbru.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ksoixgbt.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2llhctgay.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2keejbjsg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2pgzcwtwn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ztfsnwsc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2onmtdbep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wfmtptwj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uvicvccq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fjkbwwyi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hgkfsafo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2yoyouxbl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wlesmmtq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zyebwhvq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2flhxcvgt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gegfphpm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vrgvncex.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rmnafull.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzqwsomj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ajkoufhf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jhzybzqr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlvfjmiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2flyysjud.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kpozjcqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laghmixw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dorbcmfy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ohndwvsz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2exlfrytd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sfwfhwga.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2sacknhek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ydpmdaco.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qzqpwocb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xsmiwoib.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nqwkkaaf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2elplgjda.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2zqsjjifc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2epmossdy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lvctbfjr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tikwjzow.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xvxgtvrr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2liychrwy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2syoorrzw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzirpgnl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kofmtqlc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdcfkcgq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jpmpsfsf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gymzjfqf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ffefjsdb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fsaujqgf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2azbrsahh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xeholiuc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vbygjipu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2wtsffzss.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnlgholx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2afkslwbt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2nmxtufqg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iaedmptu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dglowcwp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyirbdq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pasgjcfx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yyqmpvar.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2eyrircuo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ljmizboz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jibpjvbe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wmcuftgk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zeahvzje.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2afzqjqnk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qpageoxa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fxfraanf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tlzckixm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pujedmlh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2asaotdgi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvcxrseh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ckcnxoil.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pvnskzao.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2igzehxoc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbhlrci.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qplbuwlh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yjvstvll.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2efnauiib.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mldrogqu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxelizim.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sdiyybpi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2toguunoc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dkzaszyh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2hszbgpir.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ehxxiemx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xefceyda.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lrcklpjp.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oyizwvrm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jlkrlwoa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2bvmptmmr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pvzeieuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mzxbtqmr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xnzngxko.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iszppiup.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oypxrsif.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mqfmjybm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ydzyqkgh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zpghgfpi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vgwvyzug.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2axfpglfu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2msrgchzk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odkkphkj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zvglaclc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2abqlypeo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zpzllrcd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xchqkxhq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yiirfqqe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lbhsrope.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sggvqmuf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gpodjrgi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2falpgbmj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2cintbalq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2dywqgozd.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2weasbscj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nqpuhkis.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ebyieohm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rpasumjz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2atzhfamj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ufofajcw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2neosqiln.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ifejxjfw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cjiajavt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tlppgwbn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kgziwfgz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jyncrtrv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gastcnzz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lzdzvsvq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wqwvfswu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfnauzbx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2meurrftt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bbwhryzk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ljawybgn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yuuvsojl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yayidsbx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jisqvikn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qdwmegyu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nvdqcrdv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2adyvgjcz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xgjwahpq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kctcxtpn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lpfjjgtr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nzrjdtkp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2krrmdatt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jmpvulys.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2clcmjcza.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lthonrui.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2knbqcoon.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uztlneom.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fjlbqmpj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2trofpfey.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2gldycaxk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wltqlbby.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fdptixcr.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qgeebaax.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zxdskppy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2csvucsns.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hqvrbovm.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2zxkcvipu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2tecqgjuv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jifrxtcr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nehafkxz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2llppzwgr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2upyexxwg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xzyasgcf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2smfpxhis.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tojpjfbs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ufbszdrq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2cqtinmnc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhevmkp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2syoylgsa.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2njjaqhob.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2asbesmiw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tjjomjml.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyxvbumb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2xiqdcxlu.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2iabziqnx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mjtliznh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vtcckrtv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2duohkovs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yqczgnoe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ajidybag.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cmzrigbn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2yerwbtum.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lzsfeimc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cohayban.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jydprdbj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtyscqel.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2okusdqcp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rilejnub.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2fuxtshtw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ycaihqry.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2rgfijoir.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2smowxtjx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2evnqiude.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hvpnnzos.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwexfveu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jimbibsu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2idudhuug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nmksrpyy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ofghornh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2evfkftte.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2uklyshhf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2upxfxsup.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jczemeag.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jwzswjzo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jqqpwwoc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyctlpgt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbmzadql.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjqftrk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwbwnbvb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vlmcokzc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkrhxqcn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2twxfvqbf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnioyhi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2cmvyqust.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2vqmwebbg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yegrcwkg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xgdjiggl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2hkoackvb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lhnapprv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ztbrxyry.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2blcrmsqo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ycnpbwdi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vpfxkyei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qxfhvxfo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vdhsobdg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2recnuxpl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eqnfqohk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dzwhbjue.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mclfnyuu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tzaprnfe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zdvigntq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2lvmldiol.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vhternov.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dwsxbwwz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ibpshnbe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2oxzifrec.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oakywcsn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kueiauxp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2drlluoat.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2xvnewkjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2lfolbzef.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pikamhge.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fyxigtdx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmbwwgt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2znkxxbha.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqvebcxo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fietzpcd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nffcoknm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yprpicqk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2hpdwtmww.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ygrwltxs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nmornqeu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rjlydjle.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sbheqvyh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rdzmlxfj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2umcmhiax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynhtxirb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2fmzhfeki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyypuezz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lppooqyj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wehnukxp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qfrphbwu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dhhtfxsy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2csvyvfri.html


<!-- 参考信息 -->