代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2whxbmeld.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2distbqxk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uphgyjcf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cccbwcwn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ucgxjvds.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2whzlbcor.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bdilxrdw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2iskqxyan.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yjainncd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2quxlcckf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2unovlnwz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zxksrzmb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpudobpl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2jgfirmhz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcpurvhh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vyrevttb.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2rkiojwqx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xuubdaeb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kinjifgk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nxeqsswg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2fxyhbgdd.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fbguqjua.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2avdvibxv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mfavqowm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nqrmfvqc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xlivhkqe.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jjytnzap.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2gvvajuws.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2pdtsdodi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gwoeinwi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2xzjjpndn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2uopnsjqj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cevnbvor.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2axeeejav.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cbwspctc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2susnijej.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xokrcgzu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jaecvexr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cnvivthq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tvtqitqt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2tvsyslta.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cklcmrib.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hemiqafi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2fzwsqnso.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jqmqrtcu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhevjrwa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2fpetlvlt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zgqitpgs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgcwexsx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vaihixny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zvibbkml.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2zsmdarha.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcbtdzku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xiujbedn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rtwpqdxq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wcemfutn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cimwkpxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2siyncgtw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vukawpbx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2joyzzxsx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2djtrnskq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ialenext.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ghnhwgqd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ojuplluv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2leaifocb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtkieuak.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qlczhxly.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ggzayqbb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mwdiltil.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yjfvzqyk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2deyhllgr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2cpvliryr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ohvhkkht.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2feausjwk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oxupdlxy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2eftlktir.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xwczulhx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2icfqmxzp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zknogkyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axxihumu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2guycgvjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmkqnrie.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nvgdurih.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2epvcmjzc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2viptbjyi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2biahzspb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nkduykpx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gtnuhvcx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2jdstsesq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bbcnpduj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2axnrwzgr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ktoesuof.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bdpbtdau.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2evfddsij.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jrqamcon.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uzanrhsh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tqssuolg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2banuqkka.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hgqwwcvu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ucvfoama.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gsnrfrso.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nhyjghhi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2eitgobgu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2maslokeo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2maaxrcjj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fbauitcp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2vmtgmanf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wdteulak.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yulfdjnk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qcfasvpi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2axusnqnq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iwjmicbh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vghgfjvf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zkhhmsnw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fyosspwc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uayuyhiq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tcsrjgox.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqcuzrdp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ghvlklri.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fukefhek.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ydtuqifd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gzrqwyow.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fuzvmyjl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qxldihkr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nywdygwt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2muolnpul.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rpsvzase.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qchmjdzu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2idmmspgz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kivttvwz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xeqgwakc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2lezcwwbs.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vkiijyhd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyrylnwt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fkmixlmf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ezfpgcsm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nuldgdki.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2intwgxea.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2onglgmnd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2btdhpswu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2epkyiedk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tfooccqv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2myyczzfj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2srxjzouj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cesipbjj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wuxircnv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2txovdsaz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vnesytvs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2cjtdjpjv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2yqdiksra.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wmkjjube.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nnykjili.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2tfuxcjpy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qusqvldq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oxnkndxk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xxoxqgur.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ivkqgfxq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2prgaxtbs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fjzsdgkg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tylkcuye.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ukzgiikn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2rhhsdytn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hemuwgbz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kiadpxqx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2czccghoz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zwjbkive.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hapkssxg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rsxmdikr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fgnzskqs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2npcnfyfc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jxadnqko.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2prxdhhwb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ulygsmyb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2eeqpvstx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2rkodjnyk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vztslcrg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cmounzcp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rractcfk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlzamfw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kxdjzqbl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2keljmpbl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2gvfuwirc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zglshbpt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eywpsgvh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vmpnydxf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mebdgrei.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dxikeroq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfkwbdjx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2xlxpacma.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vzmwgmdb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2aawzrcdr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nfwyoydm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wactbixe.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmefpur.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmavzint.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hlsgjuzk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lsowctvf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ufariowr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pjpgodhu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2brnkdoot.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rzalxhxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2svrukrgq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zvqkhyzn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ngubtyur.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xgdkaxcd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hnxctqnv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2joyizsel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdqalszc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ykgkjpmw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xhptcycb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qidofwhu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rqeelttw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ljrnanxm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fzeoitnn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2watdbwoi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ciodbwey.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2woxubbqn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2kblddzef.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pcvwizmg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2anpjdxdl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2spbmpvcm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sxnzyzhg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rbzpfhun.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yhaduufu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fkullqbr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mqoonzst.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2okdvzojb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwydfmsg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nhukfohh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2buzaeivl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gjppeeol.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bvflfgpd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmckyia.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kujvsmml.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2kadorjty.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cvupqhmg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2abwkqrng.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ncxklogh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ddjfrcuj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2apvfobhy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvqznrxw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hsujxook.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fvtmjryn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mcewnsbv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fhygabnh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gxzesddz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2whorcpid.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2apaxedpm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2swqroyem.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ijhebxvc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2rdwbjemk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dgsngixu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2awxltgxw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ffqdlziv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hfdgpoml.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2blbtbxcw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2suoipvtm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ovxuddzo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2exjpajqc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wbumxncr.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gaoqrpif.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zybjoykr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gabklvye.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2krueqtfb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2juckvxwc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbvhzaw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cpnloyqc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2erirfaxo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkksfxdz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtygfkqh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjilgvgz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ddeawxpe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2emchahek.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bwdxubnr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fefixgjn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lyuzwuxk.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ujduokvt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2snxmzlrm.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2mtcgaawe.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qqsdtvwn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ewvjdyao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2tazbfomu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zycpqdnt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hbbouwye.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2povrmayb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dylrtiym.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2fdlvqugw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2kdjgiost.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ychckwzx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ekwaylao.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gxmrlrkq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ipamaebo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2mnfhihsk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxhvqbgo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ldjbuoer.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jnqhgmxv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ajdudcac.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2bpgksckv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2vqkajjyu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2qixfqfoa.html


<!-- 参考信息 -->