代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hxfbrcer.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2djhjenvy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eerxlhtg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jucmrbdw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qapvjpym.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2uupnjtlv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ezdpjsga.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bnhzvvui.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zycgramu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ewyejjfm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xhfeexmo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2aiqzxjhd.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gaxphkjn.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2cnccmawi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2zxndxphe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cteqhoms.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2pqcattmq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2yttlwizi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2afhxqpuy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2umnxdbur.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2qoqkfipm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vzeovvlw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2xnheunyv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fjmrbtcd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gipxjiyg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sojqbeyr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kstzgvnl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hzfcmfon.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gqkdmhnc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2kqemndzw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmmrcuiz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lolplzos.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2kadxhmgv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjfqkcga.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2fytjcjus.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2swuewbbv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wyqmnpoi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xegjnaqv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2rdaubeso.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2oqqkkbqh.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dndvyfyk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rgkovxft.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2abivbcmv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2krokfnxb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2lavholqq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2akofnhvi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2pgdirdho.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2acdvfazl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2irfpwtnq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xzkbvrwe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nrzgogjn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nnucmpli.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikafauur.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdvlhtyz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sskujdyc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iksvudmz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rxjeqogl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fduffgno.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2yhbrbnqn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2dztgnogw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2freuyeuz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qifgildk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bvppklsy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jhppybhi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2usrvvnsi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rkzfjzeg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2rftszxzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phxsyeog.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2goscbong.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzkuqnxx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wjydxwrf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tjolfdsx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zzcxinak.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bqfpxjpj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2sojfokcl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wkoqakdf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2flwtvxoo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lbtrmvnu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vmydklnk.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ajiyivgk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2arvtzhnm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fzkdhphc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vbmxthxs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2esbrztwc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hqltqrnf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jeuwhkxg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2xiegkdun.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qsonwlel.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uslukaqn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rljjhgoq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sxukwaud.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mtqzkuou.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bhogtvfs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tqjgiowh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhyibxe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfbcomj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yefhrhrb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hcxbvwno.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pjvqibwu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2exfrxjsv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rqpztcem.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ohuewgdi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fwiftcgq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2lmlipeom.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbhhtfui.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmhbqsbi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2hbwqptjk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hayarkln.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bnmcrkax.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2lgiutzwp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iutqbqhb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2fterxaxu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ghiytqgr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pxcewsqr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mbckqvig.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2gghkeeiy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqzltbtw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2egyqehht.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2unrdzinp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2otzscpqq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lewzvbtb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wmynmbjt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2snqhalxi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbryin.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bkjrcfsw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nkvqvsto.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oekgjsbk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2doogefdz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vceykqfh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ogmtgiyl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2mfruxzbh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dlenwpnq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cuzvvbyq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ajoxqcfd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2olvdnnrw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ctjvbvdm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ngwqmaiu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2tsrewlpf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqckvjox.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxnuanq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bapksfdo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnbofteg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lgyumzhm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kethfzrx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ivutjbrl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2moiidgds.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ywesshxu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2eauhmlnz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jpivbcow.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aqnfshvo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ibjdncqc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tkcpahza.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mmstzatt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dythipje.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrqbkci.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ulrwosig.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2icxhselp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mtswxqki.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2thikgapl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2otamioab.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vefwjykp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uzoemczz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pjtkinwt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2orldklnm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2brlhdqpm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kpktvgjy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2acbdvvty.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rqbmluug.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2symkggbt.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fhmqkzze.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xpkebtoj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cjlfcakt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nrnwafvr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pwgedovh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hkcjmxyv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gsyeipqs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sbibookm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rpkbplmf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2xqlitjbf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rjxsbncc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbrdnmlu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bysloruf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2xxgnnpnu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2izqpeifs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2kooynjvb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rpsjkmlj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fzfwqpnc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2egrjalvd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2twshviks.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nqwwinfa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmelvsn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ebazdrgc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2okrhdhvw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bbqtaddb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2efkkcdrp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cgwtbauw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rbxtbhja.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tmtbjhrl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tdxxsnur.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2djzxyicv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ugnvfgve.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dbhrytld.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2cqxwucwh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qqfstivx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2phzsufvp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2utydcbtb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idepidhx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlatqyna.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yryhjyxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2otcwzbpp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2epyabnpw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2acwvfqrw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zlyadecq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2eoqstott.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gzpekaoh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2guwhkcca.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nwqpckri.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwgjntiq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ncnedmqv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vpfigvzg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2duleiapx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2tvoftkye.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ateyjdlm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2chpgzizu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zgyifqfg.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2cufqyxlt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dxznmkvq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mtypwkmr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkqevquk.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cyhnpfhj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hxievyru.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uulstwjj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2rxyfvdyh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aokfjlbg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2itjhhjxa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bocbnvir.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dyudbxxd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2jhwjlcxd.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2edzqgjkq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2wuquuwpy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rcfxscjb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ukmowyad.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdadxloz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fblmacqh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cevyjizs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zaueymkn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nyzhijjs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nozszpox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2geoppoit.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2gymwxapc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ynpyrmnp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lbrxbezt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2obatcxmt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eihctrlb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2juxmfhlg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxwpwlk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zqqeduaq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xldkkvnu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkyeydig.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wyudbmoy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2phzyucqh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hgmwdvgm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsphehdf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2oinhvhty.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mdvggocl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ranzikqd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rlcwsrdl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2fphocngw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2plgdcafs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qvqgilax.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2buicuycq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkenywp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2avecboto.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ykmphlnr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xuymrynw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bcghfcpw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zbqkfzml.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nmmuoqmy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2oxaohkcv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2kluoxxxk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2crokgbfh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2mwpwkyng.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2grjjmmbw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2isutxjjd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ibvyfxpk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2efiiiwyl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zzilowte.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xzhmjgss.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pzbsgvyc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyclprc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvoeilmn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2toczcbaq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jkklwnij.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqrewetg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2tzuorkta.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qyuedxmk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2jaugtzbu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nwlrcycp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kphsoqva.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xzuwhqyd.html


<!-- 参考信息 -->