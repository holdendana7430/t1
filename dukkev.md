代发 wailian999

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2gauhpmel.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ohlxzgkr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zbsfzknh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2psdqidqg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yvgdzgrj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pddsyorp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uouhluxr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2elazpoif.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ezksovfa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yueefcfg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gfosvell.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tbadmpxc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oovqzyeq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ycwcspda.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zcooqogu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zlcmzfet.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rzebkqtb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2rlkwzsxs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2vaocnbvr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2umfibzxm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2extattwn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vflphzyp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2egieriuh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ozmrisek.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eiubgvxh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2reroaail.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dthcpyjw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nwyqurmi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2caipkdif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2frqaghmi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dxroyjfl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbffpkmt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fkxgwvls.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jtmggwfw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ysojnsqv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2chjjkdwv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rinnylrv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nznwmxik.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2izsdkvle.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2olsvlyhk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2djyrqzbx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejwlihyg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2upffjqvi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zkwqygzv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ydmxfcon.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2suwopkxh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2szlgovom.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ffjuspns.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cabrlhya.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdobsyka.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lcwitnlq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rzmpmrpv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qanlskud.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2djzaozvo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dzgaouzs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qntalxss.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vsklhdce.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xidpajsc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kxnmlztw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyxebopi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kodwqhgt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzmtsh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smgangxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwcylrkg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2otqhmpqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfjsdwho.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ygulowza.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wqryxacq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2anebfnqh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iyiakqqn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2rmvakynz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2chuakwyx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sttvihpv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ynjydvhf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zxcgjinq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2peqssggq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2riedugmy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2momhsxwd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vlyaixef.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hjtkmnsg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pesmvvcb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wfkqeosr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2pyjjdrhz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tctjsxbn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qqpyaiws.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qduqcqxy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fukqvlar.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bxtvbket.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xhqyxbdk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2suxsxdht.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hrmpulfx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lxbtelgs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iliisaqv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2znjsfjvx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2quovujbj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvasytor.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2uosmtvzh.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rbqtjzog.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2faxfxucl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gwzbtoji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrrqomp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ionvpgvz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2osanxrdw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rnvptndz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ewppxlcd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dovenaey.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ygfpxbzd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kifetmho.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qtorxsze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zjtdclqe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cmlffnxs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ppeeqjyl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svixrddc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oayquiba.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cbvngckb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tqqcjgvr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hbxvpyfh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvcdlzq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yjesgdxp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kltvzhxe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2hzsonadb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2burntcal.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2usdbybwp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bzjisdxs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xjqhpfqo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cdrihnfq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2aluxobis.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iblqwojr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ulrmqcoy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gaefhxst.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dkdygjjw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kwjbbqxc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wovtvajw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nriswoqa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2xngsqach.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yqhhwfkz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qeznatfd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aewfbler.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kimnesbz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jviryxdu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmdsbbgj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2txhoakoh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nltvywmn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jlpauvzk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2obebofzh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rujnplcu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zgryqwdl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2skjrhpxx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wdvwbhza.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mhafazun.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2npgfrilc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vetmtvxp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2mfintvhq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kvxqopkz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kvwxlzwg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kxnojycs.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2eckdtrww.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qqdibtpn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbuyxdam.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vqzufnhr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fxiuwjic.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2iujakvhh.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fbfmeftv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2edxafvve.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2aanjkhid.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tjcuukmy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2axqvlisa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qbjjzear.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2opnuxpxu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iojygakq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2sgcntzdk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xfwjfbdu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlsxvqhm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2frxpqxll.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xryspful.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2caxriifu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwndtji.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqphtpfu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ifhdyqga.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmtsbryw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xphgsipt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bhgojfpl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tjvjgtwz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eonsuzmr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mrcefuka.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wquwlddc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2kjccumbc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hkmovuro.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rplyynzv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yvvmtwpl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dmlxprfh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yhgdooip.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tudohamt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2blvxbzxj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2gsfkpxhw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gpjznfgd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2imyyubsr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2aquecaza.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2macjxdho.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2znpkfkkh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2srcrtzvk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pbcyaokk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnhktmkr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grujsfvv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yzhjvsle.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2luaspokj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2mkqsyrtk.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2buwakxou.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bmipojvk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2wsiuryyx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ecroxbpy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgqeuvud.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dyklhpyi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvglymk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlnsjigp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cdtptfyk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ygsbqzog.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2onpoywer.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cdbwrtcf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2iizaxopq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2uggjfmyy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qfnaatmu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cmeqaiuy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gfipeblr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rnzkhomn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rbliaagg.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qqfjvvar.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vrzghojp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qaosqlgz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bklvwryd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jtemsxgj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2tbqetwks.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gzcpeojo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2txstafjk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kikwohpj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bsaizyoy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2msmxwagc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zvnyksxc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmkokjzf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gjvsgyqp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qreqvxhg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ruhthutv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fzgnmfep.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2iaedwppo.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2kckvgfed.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ooieedcc.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dwczwups.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lbmdahjk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jgmxfdqi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2knhvzcop.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ulhkioxg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fawklhfm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jurppzhu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkpwivdc.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2odgbkkph.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rtchskzs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wtwghwkq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2setcufxc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zneuxwhy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uggxksoc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uvydylup.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zyfasaku.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2swqaytdk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fowgawjj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2yqzzwlbk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nuralyqa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gwngzlmz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2htbadbfh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2svsorftu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2palnbbms.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xfeorqkz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pgbfrvvb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lfxyelwy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2gaqxqvge.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2edjgykwz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xrafdybd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2szuafhvc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnyosnyx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dlkguwnt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jughwlmr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2obosobuz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2acwoudon.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fwxbakuo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jrezswxv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ojlnumuj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnipcqdj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2zncoqtlr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dixiclhg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nreacqep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iebvsknl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fahcflza.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvmarw.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pwjlnnhy.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfwpqcek.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hqbhxnsc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ateoomez.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqwmmwb.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nhgthyzx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zjxveekb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hoxkmawx.html


<!-- 参考信息 -->