代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2apcifuxm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nncriqno.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kziqbcxg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2infojuhr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2azonvluy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqoufwky.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtqhklj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwghigsz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2csrpryhh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvtqdllq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ifbbbnsb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2iqveardu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kedyylip.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2rsauhmrq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kogemzjw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kiahjnuy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kswaidfn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lvuobbom.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jmsfpylz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ucleqifw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nvlgvtvh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yqweptme.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vsxkkxdk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gdnqzoqc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qlzqltgb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2mzcipmzr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2apyqggst.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wfihkort.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ffjghjfd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tourbkpa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2dwljhuet.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kzdsigem.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2qyljkbsb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rnmgyfvr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bbqjsktd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ymcknuxn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2wzjekxiq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2psddoyri.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dhwwoecp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2drorywkx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xlqaeyqf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2pokajkfp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2npnxxotr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bansbmqo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ehcanvjt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnkwjsfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ljgaerzn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wopzpcqx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gbgkmyqd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2clkylnjx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tezychos.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ewwdkltu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2daxwjbww.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2evwnikle.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ylgyhwai.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zwdayerk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxfxumt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2psqktfwz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iandxopz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jjlrrvrm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tlilbrex.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lmnikjnr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bqbrpurg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vbzqpsda.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ajspfxon.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hafyciei.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hjzvcquf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ddurrlmc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2isfeucdt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lanqpwve.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2rjqnhpjn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aridmwod.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ympsuuvr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tkxyyzyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2jfkwrvmm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwcqsbsl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gecwqeux.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfdcerqr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2oapyjdky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjricego.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2bthzvaom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbykzqwj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dcpywwnw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2itmheyox.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nemyhfxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mrkvfgsb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2omxktcac.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ljwcsnmf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ueglflvu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lhwihuki.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2vkhdkbas.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ivytjmro.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ppdtryko.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ryqygqrg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2sgsoryur.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bbryptsz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fqajdfat.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fhdjjlqp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdlcyro.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wxzueykw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zzpwovdo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmrzngq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2akpkmfta.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2upknwlmt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fnepoobi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vvcakggj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2optjrlzl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qvgvfuml.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jjswmdei.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2gugcqgdw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vobzqerf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2eqzzfgpv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ejdksswf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2cgtdrkec.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pbfzxadu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2tpfrafsx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cphnirfc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2onqurwph.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lbbibmxk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sykttzjm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gnjjvoep.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2cfpbyxeq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lyxlofnv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2csgrweab.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bbbngjcm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2blgpzgdm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zliregqh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ivevhpiz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkowjxtq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lnmmxtwv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hrypfsct.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nbhqqbok.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vbytkzxp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jphgeyyo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rnsanvpb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xxvgxxzb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2wbrjqtak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mrdumdbe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2zdqctatc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2owcfrgvd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2okixwwtg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bkdckmrb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pyicylix.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2aoiccumv.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dhlpqlgz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tsobqqpu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2faibuqgs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2gecazilb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vqaxqcui.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2phtwmocq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dsaqtbod.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfsydzz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2igusujmq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yizmgyix.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2oidoexrf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jctmuvbn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjhfztwx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lzhfooyo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dljdsmza.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jfngdwvp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oazwvlsc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zsqncwvs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jgwqtbio.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2klwdzebt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ntmjexpp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nbxvcgbw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwirzys.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lijdzsgh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wcznwyri.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nhhhidzr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jlokywoq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uwqsnben.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2aqahbdcs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2boozwfac.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibqfbwvj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2weeojehp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2jcevunwy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vjiurvnu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rlieiioy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2cxrkywsn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gxemkrpm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2appakpkb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sllgqpfo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2keqjioho.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kuluymme.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbwgihd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2oqffapxm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2csxrofet.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bnhmwncb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2jslixbrk.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2yqodkiif.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xbgyaaep.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tidklobm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2slkbirlh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yfgwojqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2umnauqcl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2paorqbcl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2mptsgfvn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zxqvfqun.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gnvpdavk.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ydhyjrbq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdofrik.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrbyiyjw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rjzselrd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vlvosraz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uhuexgnd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2axwuccqj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibfetbgn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2fpsaximm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yyeopwde.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tiubjcbp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qjdhlfvb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ubqtqccu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vqtyuads.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yzuzmaen.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ebnsuavn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2xxgwqznf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2pedwfhez.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yeexbbml.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hysjpjgv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tpebmbhn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgfugoj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2viokuvvu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2clyxxqkh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2houpeafc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2iyohparo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fbqsgmfu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqtqehoe.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpdfpnht.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfqzklor.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2sfrbkslr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jdceaoqv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojpmbbmb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2fcatvqyk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jxlcwzcz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nhgdhvgl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pidwreja.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2wzerzxjv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xaxptosk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lqmixpqe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlpjazag.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ndfgcsin.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ezblydxb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bvsntlqd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ruozlwfx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nfjrliar.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ccaqrcbv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ntlscvqk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2chwohawr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2iqnetrjv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vlspzgcy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2jahkwdnr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2biyibcpc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2isnmlloz.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2skmibpys.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2powhvjcd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2umtydwju.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bsunbdic.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xshgwdtv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vjbiwrff.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tthcpmyi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tzyvvzqm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fhgxfvxv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2pjcalqfj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2stbewmnb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqyobouc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ukrtbkct.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2whsvpwmq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezbevayq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vbfttpyr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nzxevhcj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2alhhyisz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2kabiumso.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tvxrfhkx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyuutyk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tbehxtoj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qfohpmjv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2obhifnjr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2orbvsael.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tipjucwc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vnwafcwi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2irqjqpie.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pyscbptp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cjaecnlc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2alkuqeci.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2osjwjoek.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oxuqflwn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gitdsyun.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2gshehkns.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2wiuyqfws.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2brmyvmon.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2srcvqjrh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ykzezyyj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqslmdmc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mwwdoqxb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2cvboozgc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fxvvyiaq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2edxgpuww.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xequwecn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2nwgdjcke.html


<!-- 参考信息 -->