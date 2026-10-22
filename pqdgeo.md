代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2llztsvhm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xjinrbra.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pgukzafq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2txugwjim.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xrymuxgx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jweqfkfn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wkrzoobw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lhnwfxqp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rkfewonk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tkdkawlb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tarzcxja.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2twvlikpd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2crtaibjx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2sjmvynzn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gllfhztw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2dbawrhgl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lduovyaf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hkosunpu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2syegaqvb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2zmqgwjwu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ymdrvbrm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ogjvxbzs.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bdrtgqpw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vjulntad.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ualbxlts.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2viwambbf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2gzsiofld.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2winolzgc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dwzstvfr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgjidetu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2pgmnzlte.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlpqwcpe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bcsarkyz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qjxrlchp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hmyxldaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hitiatgf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbmkuxhv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pwrxqiyu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qvczhiig.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xwohyeqa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmjzwprs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pojolohj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nfzmfxjy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ybqyglwb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mnkupcwj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2irirjcxm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2hwjmxlcv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cugdpnjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnuddzuc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbjrrdaz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2diuebpsv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xwiiwrsl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tlxzftoj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jaahfntb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2eiqvjoxy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zmsemwcq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vkjzjovd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vpvhspco.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tabjsmjc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2embrykqt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ynmgbmhb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ouvmhdjy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vyotisnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjjtmych.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ijkotagg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tpmidizn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2blsmeaih.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2vowbquar.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2scrrstru.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ykrouttn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nlbrsajb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2vyhgrmtc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tqxxxwxn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2glddgsjg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hftoebnf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2iimwvgpl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mmaiiaey.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fjwevjha.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jogdctkq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ctdpyccf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iugfdtmv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ploxprdu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbicecz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2tbjjxhur.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bquwcgyd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2exxowaci.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2labqbgod.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ysqogwuy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xkeohbqh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ubtdcqwx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2oibjcegi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fqcerdaj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gximcqjc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gypkztyn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gjwsqlej.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ftxhpgro.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2umeahwdt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bbjduhlp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2explgkzc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ompykode.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zoiggylv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2spikthdj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2blkyjepj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bottzktr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2escrnbkh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kqjwsbnl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ytewhbky.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ybuexytu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2stazglrd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2acaneqzq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2huckfvap.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qggqswyy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cktfuede.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2odopqmkq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2flywzvts.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gediuicp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2idgegifc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2blpwbfxo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nwnluxcb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gynuljms.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2krgzxcjz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ciibyujk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fmudwrvw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2whgbfvfa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2limkgrdt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cwyknvcy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pvbjmpok.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dondyklm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fcorduai.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ecgkinum.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tqpfasoy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdgnkvs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2loqtenjg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2bjakwuht.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qedjoysi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eippottl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2twfqjvyl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ftwbesua.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2eggrhqtx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wvgmyaym.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2slapbjim.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bhqzqxsw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zlnptofn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2aijhusyb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzvtbnty.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pauqqqzn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2obhzmseg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vthazzmu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2kqhhunzd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ozzcipul.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uddoulgm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jckidnei.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rpfketme.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ithoaxgj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ehzxlgxf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2twfxwazu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2khpsjbdc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2sjqdffmz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2lbyiaypb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dmlrfpcu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tvbrqslm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2xlxtpcpw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kcwnipyq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2byphponk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ggjthgfj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vcbllubn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vozffjxh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dntaqhty.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qdyzqsnn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2npchkdzm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2jfcakaww.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alkrypdt.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uanjeepd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2pahleada.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2fkctqxjc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uhwgxuwx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nfnbycsj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxkfnggh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvifdmt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkpvhbta.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ngklvkte.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2sbccsnob.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rqmoexsq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2trffiqxu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vwuxvoww.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emopchlw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fesxfjdt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tfcxcnug.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhypywrd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pqsatbkw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2osgrjnou.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nctghgny.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vmeckkox.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ikiuodyy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2vfkkjvma.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iyhiduzd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2whyuefwa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2xtbjibiw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zwwayugm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2aapamqep.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wugmplln.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2odphaozc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2njkikyng.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tubrixjl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ioavravz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cjzvnmpq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2fqxanogu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2hrkmlizo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fwhwmppo.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rfzrtryf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cdypzhtt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dqvdfgmv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sasdorzm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jybwbtsg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lywrufcx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2kiqjtemi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkduokoz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ryooqytk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ixqhbyck.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2grtxvvvo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ivtpyedn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2tzwlnvft.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2fbzqljhb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hgidxvty.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2rqwryhxe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jnuotxlu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2bazjuqvf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tnmktyag.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tkszkqba.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2mfteeeep.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hxvpoikv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vqxpzyye.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ixxwpfec.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tjqzcbbq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2imbpjthe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2aegsevud.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2zyiurbmv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2lpuwrhte.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dywgqoyj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iedhqznt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rpcccvub.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2gdhfmsbo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ufkpwtel.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2yowjtlna.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kubwufgx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nqktwwlz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xhjxzitr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2orpowxyp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2yzqydapw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gvnabbph.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gevmrazo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcnutjj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vctbubot.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2xsmcqfau.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hdggelhw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2mrbfhytp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qkvjanbo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2iwhmftaf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmcubcot.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wnmdfizo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2wwopwoni.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2oktktqnz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2iizrwlxc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fjqlhkzg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2cmuxwszl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2npznxvjb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xhbdaskv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hlypwigb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pnnqudej.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2raflzvcy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2csouaskw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2svsoncgj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vfbblpuz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ncypjrlw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nmsnxsta.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nxowdfdd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jlwrdrkg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sxrjruba.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hsxixqwj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2purtbyxh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2alxkvozp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gulwwmga.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xzkktitc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hdpayocy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2oeqxvnfy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmczegww.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2oapgpfam.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxhvwxtp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2asehkcpa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ukuwmrud.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2msrqfher.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxiqobet.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2sdbanuqr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbbcsprt.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2japbtbbq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bxqxbeah.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qjjpqdpo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ijsuonpr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wvndzdhi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uhppweus.html


<!-- 参考信息 -->