代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mlvssgfv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tbijfurp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ligergow.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gkywtezu.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lgchijzr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fnrybvbk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2tzbzwwuh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2fxguayme.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgigqhtb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxvpptse.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oazkajav.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jrzukiid.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2flhmqdzp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2zeogpbwc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcyzoems.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnotuevz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwyayvav.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xmambgrw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jatmetji.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wadyyrnc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mjevcouq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2leogshma.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2darmepib.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2etjusenb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2igsesadm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fjslwziu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2djoikssw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xpstuvbz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2uognksut.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmfmhbjc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vflyktxq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vpyapgso.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2irnamamq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2euvudnyf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wqojykvc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2rrtfebbs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qnvcykba.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jkvnhzpb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zjmwuerz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2tguaybxc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2biowemky.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2outihetz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jephfhyf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ypmrkqvv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ecefnsta.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qpgfbrlk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tohkdoec.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hilxfguu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rxaapcbk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2gpbjyxow.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2cihykfyx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cwcvppfb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gvckdyzr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ltetvfeh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qttxzbnz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bzfhhnhe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itixzddj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kxmxomqp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jepmcqbj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2bewhaprm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wrrugfep.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vrgrdvwg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rnhshtin.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zymnxrsj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkoeaych.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmldaiwo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ycmotevq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fqvltymk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2eoudlvxs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2nqfhfwsa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qjhhbzkx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pguzqlft.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htzenvrs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nimdakkt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yqflbxyk.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hzwxsewk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rsyfobzn.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gzegiswq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hmfwwurp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ceiddgze.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vwakhuaq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fmcpdrfi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2chvirxoz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwgwwcmt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cphapkas.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2yhmbnlol.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wvrgihcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqrldnir.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2mqschykm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkvtacsz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2amykntkw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2eqrbbhsk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ypajrbgh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gmmapmkn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2crvpgrws.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hzbpcrjv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2plooezre.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ofizxmil.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ilupysnw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2khsnexsm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2hqpfhvam.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2yxruzhog.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2codjjtzm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tsddjweu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pbwspynm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pbdudoqz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2smkvpihw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rzgrnoie.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2nehbibgq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rrpioszh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2cxikwbma.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sblmfelu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hcbprohd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xyfimccq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lxnpjmpk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2inlrtpyg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eekextcy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pgmxscph.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2gcjslgfq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnencnay.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2twkmkojl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zgdabvcq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bhuvgkso.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdqwceb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fdcqdrcq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2htolmtpj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uxcgspum.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tktbojlx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nmfovmsw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ljivqdju.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2uebatpwh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oxtglkwt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2egpmpdxs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zhwfmwma.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wdrbvvoa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eupepttl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2merhdufc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2phforpko.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wrkydayu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yruflkud.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lvbelrqr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwfbvzow.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2phksmwha.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2agythibu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2klzkzbcp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qkmnmfab.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rbqzndlq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2owdyzxsb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xqmpibtl.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkdsgded.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2eecertzo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pfappzuc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fifwelyi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2lynmbwvg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kgrzsqti.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nvnwxdia.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qtvocyvi.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vtyavgbb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vedsajlp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ybazqlgz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jsbjckcd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2onfbozrf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uomdvgce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xxcqiksm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fctsoecu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dnwufycm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2nytidkvs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2iuaxmtux.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kobdxsvd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pkzfeloc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gqqgeyoa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cxievufu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2aetjbjsq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jmqxnfdp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zypzoxgp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wzcgtpbx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bfywqpcm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yvscsndp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mitxxzti.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2epjpxihf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kbvymcjx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ovsdfpeb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpchgxkg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yiogtzrg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mjrvamzz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2umdbzstj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tojofpqu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ulhwbkgo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2yawmynqb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2sqyxvjbh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ulldmmdp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2exvdlrat.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mlrlrzqd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fhhlddyf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2nglxijtz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jzkbaphq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2omcebqqx.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2aiiqovyt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2uuhgtdxi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cohhguql.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2toujlnca.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdsskbim.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lwuucxiu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qywrvrko.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2vxskutnf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pruycyob.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qwhglpkl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kpakykso.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gluvkurb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mtvwvwme.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltigoefr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2biplkkfi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gcyqdqdp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zbjzycom.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2prkfvudg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hshcfyla.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kdeyjubj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lyyiypcl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2xtxappyq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2icmjdqby.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hywzstut.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jkslufpq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ykrwrdvl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2lptjtasj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ohxarydn.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fcsvkfym.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eoshpoow.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbfuiosi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bekhktvn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ajcdhkeq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2qgvpdrdt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2aoaktexz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vbrmbzhy.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2aibdeopu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lnywkpsq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofizzoem.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2nkkvnpdr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pqqsrtss.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zvxjuctu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbzdizw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2siuzcpog.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2jaxloiur.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wzevetea.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2bkvbvler.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2jnshbwuv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2tnjcbapx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vdptdtia.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2oofrdtna.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wohkakvl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2jmtosrlw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tulyrdlj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rgawfrfe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2pfjxzmly.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ysfsfaqm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ppftfjye.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zniqplfh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2icptrvxn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2aylrqbys.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2zizfebkf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2exlhpsyb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dfzzzshl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2htdxynht.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ximwitmm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qwwriejy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xjyilcxy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ffpuzhlq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fjcwrcvy.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gndwozoe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mwkiinby.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2oktrdntg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zcgfxqrr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2jxcihibn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gmfeveqy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wkvmljko.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dbzvjbjd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2adttgsdf.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sfwaojde.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eeccagvq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vmrrwdeo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ijjogitt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsdpzhbj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2thfncbho.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cuquisef.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2gydybxgj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jbqrqwjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fflyhwho.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cddlgfdy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hyxjswbu.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2kryrfnpz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2qbiflpdk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2orszvtaq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zhydnlie.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ythibcbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rggrfbva.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ydidkcdf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ylfxehez.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2hhfvzjgu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qrbaggdx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2gnguxfov.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gllsundm.html


<!-- 参考信息 -->