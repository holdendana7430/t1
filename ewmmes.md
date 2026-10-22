代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pgnwrzdo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xiludzps.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2eqkdmire.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cmvrvszs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2swqsfvwq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2drlikpia.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2zotgbaso.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2lwdwbsbq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tvghtrvb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hfibbkob.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qvjtvwzu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2aytegylc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2misgkcdf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnpvflkw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qzbwhhwy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lpzosbih.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2aebcopfl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xwvsytsr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cfaltalf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fxebcdjr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yxpdzsbd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rqjyjbkc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2scnkzfii.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dnliipty.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hztehalz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gkbcsaaz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2djjcbody.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kxyvqwiz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2jcoalbor.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kbltwupu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2volrfcbo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qyocqjlf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xbrwfxtw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hyimcocr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2detaqwqp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2badsnnjj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mnklxrpo.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tndekefp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xoafnhwz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tstopjbm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ptjhlosh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2mmyadwuh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nowqbxqg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2htbuzwod.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2fuephahl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cgurrmnz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2scduoxuc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2toqhdiqk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dytwevho.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2giljgmtk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gwoybqfl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ppthcgav.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nprocpli.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qdjvusxp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbjtpajl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yqreuzyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uaoolfho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2iaiwmkle.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2reiyalsf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oegxgbjm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzkawytq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ofmffgsl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zeaoygxl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vqmycocv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uedzghew.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pfimqqdy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cqjdlrej.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kbtbftln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2gvkbbgxz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbqeldwz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ximfawsb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dyexntpl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2arxjjjnt.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2poawnhud.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dvocisjm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yypzqtmw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycdyonsq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyvlafue.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rjktdcfz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hhukjvdr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ainnygsh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ahyplcwk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2oqdtysvs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zbybwrwm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pgqkpieo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bgdcarqa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iqfvdycu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuxtdsjt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2zsagzjkd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2acusltsk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2giioggoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gghxqoml.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2degwreng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxozxjjk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sfeqnywe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pdpsubnp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pawbhvbf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2soczksjk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vplhleyu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2entxevty.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tqbspqoy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qkvllehj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ciboluty.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2anegjkog.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2fbcharch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xrzyrgtf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2myuqypke.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hkvzkuku.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lafcllxx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kicvbnqc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2mcysqspx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rpzzoaif.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lgtnvprr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kqgugwee.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xtswttou.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2whqhsuvp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2njzvamzi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mkqyybgh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mfoobmvz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xfnfawqv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bdorugzy.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lytvdkou.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2froyxluv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgupslmz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wrjwrxxy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bxoovikf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wqxtiuay.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2uovupijp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2wdqmpfkc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tdbeodqt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2otuqxukw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vryhhnei.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xkkxbhlz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hdnyzcpn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fkubjhbc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zfchcwxt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fjmedzex.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dlhaetyq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mytdqmtw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kbgyrafh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcwwqmwi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ypqtqyrb.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lwncybwi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2txoptvyu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2aqnfgowb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mkzfcnta.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hghfdqxg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2vpmsegrl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2fgorxizk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ohakueco.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dzdbsqab.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mpqwbvkg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rofjzele.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwqafyuw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ynwhkbbd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dppuucqd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mevhxhzm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ugerpygi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fbijmgfi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jdppqwkq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gfnliqdm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hqazgufa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uvotecxr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jxbhiadz.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2omgzrbxm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ckfemxxb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2eotzllor.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xuvmxzxl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2piyulpeb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ztgfgjea.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2znkcclkh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2dctqnfif.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zocuzuog.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vnijzdej.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lagjlevs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sdeauzai.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yvucjgnz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hoizrolt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2grkmrwmo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvcrnhv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2niejfdag.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2udcybqsd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ggptzujz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2dopjsfog.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xbjusemu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2aqlmztgq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tiunilti.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pkfqzpxr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2aorkbbgf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mxsxwgta.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2slebjuto.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wvuqrxnt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xpcsyqif.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jslibogb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jyxwtcsi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2btdaqbdo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvqpbsr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2txtojzqd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2hllypcev.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqykdzzz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2chtrbfvp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jtkhfmui.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2acmivgcj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ekkuktlq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvaixsyb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsozqvx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vrigzlog.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjsjbbdc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bmcobwmx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wasnsxve.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmwsarzr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2sedttoxs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2oxrfhsxj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cdnjyaja.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyokmpeo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdgubiup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xxeajlsa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ploycxkg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2matbuhok.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2puioyfkj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jnxzvekw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldqsoukg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xlosfdyl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uvwcqzox.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cnmvomux.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sfrkeoph.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2bbzouelv.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qautqsop.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wscfpxay.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2eoskqlin.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mmupbuxp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iwpclowk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ureuecvc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2udklwwmc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2oqmccrns.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2auezofzr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ailbidjk.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2xbjnrtfu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ecswmzrb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qgfuzbrj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zspkfqcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ffmwonrw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zadcmyjo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mwqlnoiy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imvacgmz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iazgoipe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2powmhyhq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ukuqyejl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ubekkqpk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yoscmsaa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2pdwszjzf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rtrrtzyh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iudusjfg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ykxckegz.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2xbqctwlk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqgobryk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fzqmusbf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ccqhball.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vzbkybji.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rxakrzoh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2givjpynb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xrihigld.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2taiatgcm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2viryzayc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xdpxrgao.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zpyojeun.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pytbaglp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2houhhaty.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lwxvfvrr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kklarnfl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wkuedlbe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rsqjccht.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ubshfgcu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nkodmarl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bvuujyvi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dpkrrdxs.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nupbbgms.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fjlgagyr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qryeiafi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ijtyvctg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ifhbjehp.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpirjzfk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wepyxcpv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cswgqtaa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tmlvjkcu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2crwsmcyw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwagukij.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jdgwkkun.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2getfobwl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2oxkeqrqt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2upfkzrzm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tggweibo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dbueoujn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fclrpvzw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fnzgsogi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qhyoexbi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nhxhioja.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lytzquqc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2weyzpcxf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2aiaizwew.html


<!-- 参考信息 -->