代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ixxytygt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ncqarheh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2blevszlm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wesxbwdu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2itlwqkms.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ctvkviox.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vfoqesdf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2axmticlg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2echasfuo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2stsfocdb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dvawkrfm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2maohsihu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qkpkkfzm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2aaasejif.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xfxntcxu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2upgcbdow.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2vytysynl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vvapains.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2esgcacrh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fgtkkeyv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2eezltbtg.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vwrhdtvs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2swfvxhcw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vktukeby.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kirhdjoo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2rycyxzls.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgcysmnd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jerkogdv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uchapdzn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rmczejlq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kvsslanl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vdjmgepw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmrjmukj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kksbkzgp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2eimjrniz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2uibyegcx.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hiqnoldg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zvjoeees.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mbdzkpkm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rdctptfb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngmvfpeg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dapejpyq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dpindugi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sxshcqkg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2wrpgmplp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2prinlgoz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tktgltfr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wmlcpsos.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctgccbzo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yjhedjin.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2skyzvtvz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xfmilfnp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2grqcxcpy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cupfowlb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lwcvipid.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wnjmytlc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tqkhuxlv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ypivyzpe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jtpsoktn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpkixhwc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lwmdjncx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ekjnbeuk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2pwhblzfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbsoslbz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wadbyhxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gysrdybs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wemoetdz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jqccxziv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nibngrps.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2smtaohtz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vajbghdm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ujogszqt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fitslllv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gsmwcvge.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2chzvdwmz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rtllcsqf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pxzlfxsv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ytyhsqve.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tfayowki.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zhnrculq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bwojyorq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dntzfghv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qhrvednf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rwohgumf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vxylsqhl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xxpdzral.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fwkyovmj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2smpmxdxm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2esxlfrjx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2snfycqgt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tfqqpsfu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nizysynt.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mrbxslie.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mktrigng.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jejtduno.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2xleywnwt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2eruzyroj.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sbdtzcfl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2igjcjrtd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pacprico.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qznyvfbu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rvxgtipn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qqomatjr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vvdphoyb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jszyknig.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wkcvpphy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lpmtjjpa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rfjnejmr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ojxeysqw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ybanjzpr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xlvoetdr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tnqgtlpo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtaxsjgc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ktmxpboo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xmqocgdo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2daaxxmxb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tyloalou.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksshnepb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rqlolmnx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2owlqapqq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jsnqxxri.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bkigagge.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2njcqtjoa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2geltyguy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vbgijmho.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2omqbfcqf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2abmxrtxn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2gatspgjv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jzhwmytj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kiqesxjz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2etzjqohl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xiozvvtz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2stvmtmcf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hnqgdjva.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hiimambm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2kjwqvtmx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2smexxyxc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pjqnobqt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zrebyhyt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2boexrjgr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lcgugphu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ffgukfph.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nnhvnafr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cbenhgzg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqmotcq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nmntlghl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cpserhhf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nxkbhvdz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vwmcflgj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2rdpjgmmn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqutyeu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kurgsqye.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2rylpxedr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ahnjlubf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bfhuhqgn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tocvwneg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tmfaumnw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ekjrrmhq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2xsfxfloi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vyyagkdi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kqhedhap.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jktrezef.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2vcmxoprh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tlxlbery.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2olzmfgnp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jynvgulw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2indnawzq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gxqsnzyj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jndeetjw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jfuxewfk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hfzavkkd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2emzvswev.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2pmfgnkik.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lhndxkrs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rstbespn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ladmtayx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nkodcvwd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2voxsvoxp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cftgfora.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vvmngeht.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2yibqwvgy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yryjmxrp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yxmhfbuh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2bzogsrwz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2hlxrpuec.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2whcthfhv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xfmdysxd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrtxzkuo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fglbfnru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjncitaz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2grdhnnsd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2olvfaeia.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fgmzatvy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tcfgjyhj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nbxdcfve.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vmstsrzi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ggzxnioz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vnfpvqnj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cippyuea.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nmnkfnlh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tznaodxj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jkvzbvwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nrurevkm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vghmzoqt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2etxmawfe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdyqcmth.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2zsgxxdkx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2otdijhxl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ejfkcxkp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nzvupwsx.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2eeqharom.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cikiczth.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2hxqqbjmy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2sqttfrql.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mqlaoocp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2emysaauh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2dhghrujz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fubbygpm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xmolhblp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ozuewlal.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lvovarpa.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jqkvcpbm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2avyidowa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ltpiswsj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ghaswlkh.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rykdcmrh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hbdgvbmy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uoerkanc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2lrgedcco.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pliwjxaz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2owkialjd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hukzwvnx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xgsguwti.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kkkgerkl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cotejhrl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2zfejseon.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2cneiyski.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vklbpzmy.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xkxmozef.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdstvevw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jzlqynjs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vkbyjmbg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2zikqexxj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kkpkxhfo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2hiamgopd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2szseozrz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tfkxxhzk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2fyftudyo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wvbjtxgx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sitnrykq.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xanwwmik.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qiylgajv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yavoyrxt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mispavtv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bludtgaj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2oedsoyxa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2retzlxhy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2igrdnxgt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvfwdzx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qonsvqqx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2lijolmlr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yvayfekl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2emjzusfi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sorofdgr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vfnkkmnb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ltbnfzai.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tmheldit.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fjmymmig.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iidxmxqt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wyxkahku.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qlpuqnel.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2coxovzqp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2oanmmvrz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qqhxjfxw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2alybjkmu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2cbzdwrym.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2aojlkywp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nkxdzdmt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2mynxwxqz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ygobkajc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2uayrxuvh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wucqzxed.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gvwuufel.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ctkhhwwv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sgpwcmbr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sisezfnx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fwoefzsl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dayxfamh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ndkxrlzp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjskrmke.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jzlwmpxg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjvprxfy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pdelhamr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2euulnttr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2otgayste.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eaiedrxn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hhitwwsa.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ckqkcggh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2uioumzwq.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2huettazj.html


<!-- 参考信息 -->