代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ywtrqsxj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mvjbjwbn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vhelunsj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emvpzsid.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2stxhgxrz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgsxnqm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fyrzlsmv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2mwtslceo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2cmwrtkbr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2elgcuxsm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2zfrsjnlp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tmnshroy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2wwbnktot.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tnrzryop.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgtbnvsg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fkgidaar.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lbfgdfwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2ugpjwdat.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zuwuvmtc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pmahwiko.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mwdgjxsn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pczwvtrf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hibajfsp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2eblursli.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fswsxeni.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qeimncgj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wsmfoecy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xjfhkbza.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2svjntrpw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qygqcnwq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2vybgxgil.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rmtapubx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lhdabrsi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zzmmpecn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ablnoioe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2enaesyde.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kbozvzqs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xrhinyna.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kuqzssrh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vlymekix.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gavhvxoc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ttneiywd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ughmxfky.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2kbvlworj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fikhiflb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jgmowtdx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nwthofne.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ycljiylg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2osuzojlx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2itwmofjq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aishaoir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vapvnpgo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2rldepcex.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2blexecxl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lgbuyxoj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ihtirwkt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2thwqmsbg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2liecqsai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2boftvuds.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpsixqal.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlsjbhlc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2lkzumtcs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ilvadsdr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2nvcavpff.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2gzmmzppo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2stirbakb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ythebghg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2irebpskt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rimaletf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2psykihpd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ilmxizdy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vyotxyzr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jizitvrp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vwbspvli.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2slmovtjb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dwbuznws.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gmhkpigz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzvckvto.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cyrwrpxx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zhlsztbi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2wiooutck.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mcshyjpp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xatvghwu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2chxqkszu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2bmkiyfiq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jmxjwafp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2eqxitgxy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oecjcman.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xpafunjq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2koecvxzt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oibatvhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srlkdblb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pptkxoga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiikndhw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iqurxjdg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rgfqycgm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cfdwfbtz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gfnekczx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lmmfsjwa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pawkszpt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2zofgjako.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hezanbzk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fotekmdf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2upnocuef.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2uwsmjzfd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qquknkru.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybsbrnkm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2adqrybpk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wqkvtpnu.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zadantrg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2muztasjr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fzkqjrpb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2aekphrud.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzmzmra.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2wthfawsh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2gqgrejcp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vhejugce.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqfdrcoj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2qlpilqbu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2icwctbnp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2czqatwuu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ezirlkkx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rbrsghed.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kobdukfh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jskjhtxl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hbdveiwr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bphxnvvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zocuslrd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2secldumm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qvymccik.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2utmjvgrm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2igoumhtw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lbsunotp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2camopdqr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ksiluzjg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ipxufzti.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nnhntmvm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2phchevkh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mrnqxiyc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2uqiczvje.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzynqvdn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cnaznuca.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2enpylhjq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wnyeidhd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2agpqimob.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2urgxhtcz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pirfemjz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sjcrpbrt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tsgvsaze.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2baqncwyu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ttkcrlzb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2htqigdbk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2camjhoor.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lopukjyl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2arxukwvi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jzeoxhbp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2shclenfz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lgrilwjr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wehyxktv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2vwdcximn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ssgxvver.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ascjghpf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rocnmoks.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qlfrolam.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wcvqdngo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ntfuurft.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2lrvzziyh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2avnqdieh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xpykpvrn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2veiwwvhc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lccfhfwq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2atprphza.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jzhvxfyk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hasxkxic.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2nefqcvfb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ajzydihy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xcmojmfs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2omgyddmx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vbignfws.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wstyvqly.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2wtuvytlb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ogpmrpvi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2mbyalxyh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zweqpyxr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xfafklgi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rwefdmpm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2aitkgcia.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ibwensel.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2sbisadsk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2gcojxpcp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qqbpieuo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hgvekodk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kcqpjqbs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dosqtywj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uwbjcxjs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rycgpczt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2upzqtmli.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vsuawdgp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ybtegioa.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cayoiaim.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ledenlgs.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tlppksdz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ehprlheu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xmjykxea.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2peaeuqwg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ffklnayi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nungvfav.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fvqsjqwc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2dmylgexf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ptomaahr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2welxgicm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fphvrawu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ymwtkdxi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqawjdnr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2znixujck.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2puidptee.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2zwclpakj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2gpuymihd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dvekccvp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mlyvyynj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sqbdryzc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dwzxzhwj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrhkyr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ojviwtah.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qhwtosyn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2daudeuow.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vdpjyakd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vccyrnjh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ewfxyspw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ighytpbr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ztfcybdo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aarcbxcz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtjratq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2szjcakdx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2rzffhozw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rgcytcdv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lxadprvj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zdfxhzxr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fjdukvll.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uyydqmyo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kmpbxygd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mpmjtpxq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2drlcnlaw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uyphcybh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfaabeze.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vdktjuwv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rtetpkwv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2zbuhaxyz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2xxqphhie.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zxvrvgct.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zkcdzlkj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2gpqchkrs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2mqywhffy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xbjartyc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ruyljwgu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyhdbiru.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nmnhirso.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2waueyzaw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2wczpddme.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ahgjrmnq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ktzxoevs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2hzlapkys.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2spiwfwcn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2lvgwidlb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2unzjwlto.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ntakmekd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zrgfexce.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hgjtuszr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zixuopik.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ykyxjbxi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ynszdzid.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2bkikwoor.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2xhtpgwfv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2pgnolkmn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2oswbdmlh.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sdsabvve.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vgasbybj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gxpjunpz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qgiqxaqz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmgbtzut.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mjaztyot.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vzvpovsq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gywlvxqz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2nkceqtcm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjcpuqvz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ymgzxvgh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ifbopkbz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zxnlmytc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2iktdbfef.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtlpmof.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2munawppa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qsxkhfue.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yvtfycoi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2scwjjjlp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2iyaprkxy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cspodgdq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kgtxyqvo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rswzbleg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2evrhszoy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bpxfrpax.html


<!-- 参考信息 -->