代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ticlrdhb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tjsrnnjh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaivzvda.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3vsznugfa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qipoanxa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vtqtzpko.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sdhtkaav.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sdhbtyzw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3rhrlbhvh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vvoeomzm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eyngxzev.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3eeoegluy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kubjrfhg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3obppyoqv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qwdviqxq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vlnqftjh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ztwepjhe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3kffggjyu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ldlktyqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wrtnixnm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wpvrebka.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vgohwmit.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wvkpptwk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3enufmbmk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qoytqrjd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mfkjeuan.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gnyjgdxp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nldgndwh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ytitcrzn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3swzpxukw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uyoedmmh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fkibfcrh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3zaepetek.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mqnsyens.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3jbdgkuws.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3tzqeuyra.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eeuyrvdk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gxbewxgw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rqmnhrxn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dgqosbzi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xegeujcu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3iosneqsj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sdvqendz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3fitubfci.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ovshdarm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3udjrpojh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3przmlxas.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytmxtfgk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqdzstrz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vusgvzhn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3meyeqysc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3olccheso.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fxrfejxj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oiviidmm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qupiulwd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zuwxvnoq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3otueyufz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpwwfswb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3polhqgce.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vncybejz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pydcbusz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dhoolprl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bkplukiy.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dluyzsab.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrzqqixd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glbofdyi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3waifncdb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3meyfpdbh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tnloptaf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kbczqnfq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hgfarwsm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xbfkkuwc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fqhkpogo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rmryovel.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3obybaoxi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gvbchvhv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3lnkpruvw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3tycjfeam.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfnghgdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhtcdzic.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fwwfgyau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwnujzun.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mhvkgmid.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pmjhswwg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rvbhsuxb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ksnoqjog.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ytabfkev.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qicnwokq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3imdxvtkx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lbqdfotz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3einwfrdn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pttehyed.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vmovvaky.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xymfgjkp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3krjwwgxj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gcohknbg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vowttteb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fonfdwjc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jvflizye.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pctouqmz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dfvvpvgr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yhrzbyrv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ilbaspar.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3bmfcapwz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pjstrpzn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3flkllzbn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rbokoegv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oikjckbs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xsfvnkni.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oqsjiltb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3judycaqn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lgkhmfqs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rsjqvepl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mzobhjej.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qkvqeice.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3iccscobo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyripgl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3gwxuyedn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ddocxylo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3okvtfowj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ayugijkv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wkmfubff.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gcafrtri.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bcasxqiy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ukletbew.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3airxryxt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tjuwekzb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3iloqovyl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cztftuzb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sgfksrks.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dwmibagp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cqvnetsf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oumtgcws.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxblkwf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lmpfetoj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hvkzdzbd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3lxvkwsxl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3yjkmavut.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qydftgxk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcrkncoo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ntmnlbjr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qhadsspr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3gntqazjn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vumbukjf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dfdagsir.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vsalytvn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3avqrpdml.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3etcrgvsr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3xpubicok.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tnskspya.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3dvrkbxbw.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3tzshgmwv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ycgpcocn.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hzaravje.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tslyhwrx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qzngdozs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gikkbwck.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3jaetteto.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3cpamhzqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uerylbig.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulzmfcvq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kgkmdhsm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dciusmke.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wbmkkzos.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3chpozibs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rjgppofn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rekemfdb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3xocpjxkg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hwljqspm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3shqjckmr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ahfejkdb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtdltq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hepkzfwj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wgvglufw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jilcogry.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3sptunxxb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wohxmkun.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mxapylvu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmxynqbr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3tlvuxchk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xvjikdxz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3mzynitrb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3plslftly.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xkiipkjm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ujtjkvfa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sshqlnyn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3hqygzhfr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ekvdwasj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdybaxy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ymymsqfh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ihvqfhps.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cpkkbqgs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mmqssiqd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3glcaqxcn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vpycfyct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxesjydr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xnkxarci.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gsxznano.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tpmirctf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yaqsqfzu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3zhszeona.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3vvgayahm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzbdbykq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3drwjqunw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swhpoekr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vpldkitd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3swyjbnoo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mzzbqzvr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3orpwbfag.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xgbheueg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okuyoqkv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nlgwebue.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gpenyhll.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qazxrmhh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3oakpgpqi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fmemradh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3llimdybt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3zeqwqfzy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ceufvjnm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3idnctqpd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qadmrbwc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xtodpfnp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qbzcuzwl.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xmpyjlpd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3znnpzlgi.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3bfvqbwsr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gjimjawh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hxaoaumt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hewzuasb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awqdrykm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zjdzeffy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3teoitrcx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iictfbyr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3eufjnapv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tinietzx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3mavgivpg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3oqbsvjeo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ndepmaaw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3tcrsvpcu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zeoeodzi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqqmqube.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hrbyjyyc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ewwvsylw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kairfutt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zlgmnbxb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3pvbtnzgc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3hbhokexa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3hwkxkcpb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hqycmyps.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3amipumww.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wyyrnvyj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uhzzgdjl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3tupefcwx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3wuflelay.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbefkesl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qljbkgud.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3otgodbvj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jjvuyybz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ghurhevh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3cuwfderu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3shhtwfjq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mslmrxzp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3oggsrygi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rbcdrbkz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ylhzwctn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rsawngss.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfhsykvi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oalowggz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqcwpgkq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kmgtavnx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxzrfito.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ksvzvjsc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3degbifay.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uigwmlwc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ggwxyeum.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3foijgnoj.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bskzrfmf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3koomfoxn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mrbvtdzo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3omiyuiym.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3fwavjwwj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eqcyqcrj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lxxfchnb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rhvoiiap.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ezfjxurw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3pzqovonq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkijqgrc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3uitvngne.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3exntiaxl.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bousdwpe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3tnanappz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xlvxxhao.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3aubqztqy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3mfpncgwa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3qhgzzpux.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3xtlofjbb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qlosgdma.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3xgtvzbyl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ruqstznu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nieammsa.html


<!-- 参考信息 -->