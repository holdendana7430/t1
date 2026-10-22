代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2borguvkh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2emohcgve.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gaiscmsb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2afoettlz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmcwvgbs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wnqinfbk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vfpwmfyg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2olzvibhc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tvkaflqu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tnxjfisd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wwnvuapi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2azhuhtik.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nqoaqbwq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvbukvmj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xwdlnxje.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zjmlsyut.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mssbvhtq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2oddjbgvb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmolljv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lyxopgio.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fxdfkwth.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2jrfgadfv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2pauwbuwo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pzaxghzx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2niuidnlm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oahdbitt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zkznxpqi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mbqswqwc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ifqqykyi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gjrwrriw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ipnenfec.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2pgxaywnd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ucadrdiu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lcujndnf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2wpxxscof.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hsdkzead.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2flyxcazz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jyyduyhc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cvjsfgst.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ujngtmxc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xrdoxdzq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2drjhyhiq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pyhxvctb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2gqqkzjpr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kuxhtpai.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ytqcrcsa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibsdzzuo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2tbzvkoxi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2egnrokup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qajmgcgo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ujbdfddb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2epvofgkc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uzsoqbdq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fykopeup.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bllabtom.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gqpztqrb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2rbewptgq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qywculyh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fjdqmono.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kpemfxen.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jizrpunv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ltstbckt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2piownijf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ehdplxwp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2bvzwhndq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtypaend.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2swdfsihg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ziglowif.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2oizmedck.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hhhmmbik.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lkqpgvak.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2prlfjivj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2sootlvhb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wcvsvipn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2afocrvag.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fefwsrmz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oehadysk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yvxqbfkv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yaucbipi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myajvxkz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2jfyxoxrl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jlhtaouk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtsyjnrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2verjaibc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jellxxfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuxnglru.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gtiwazta.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lvccvcxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2neikopld.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gcyjrumw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vbihlhqp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vweeomvc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2gnqzlgjw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xnopnkrn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2khudfktg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xyzulfen.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yrdawnqv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mcvdlllq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dtobdblq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2afmwbwnp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2suaprrfw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ozswbnce.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2tpnmzzmc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2aqccufsz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2johckttr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tfzsuqct.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rpsjucuu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rqtmiqyj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tgliqefc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2trlwsdft.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rzzddfhi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzhqvkg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nfeoqfbn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yajikmpl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2afewexxi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezkinqxv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jkfchbka.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hlsrggjv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2courmtji.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tqrsergl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vaaidgix.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lzitsrsz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2iqkmkjed.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ihcdwnve.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bebzvfzf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hqweqzxs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2fnwzgedx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vwsnohzf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jlogmton.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rwafbwla.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wkyuerin.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2adgpsgkq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmrtoqeg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ffbqybor.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vizbtwkl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qhflicyw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2tursdsye.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uhgtmnhe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2bgdlzqee.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2agparjkp.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2keskulza.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2eiswrdhr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ayxrhrpb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jfvuhqrk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vdvlxtnw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nysaupaf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qgepubah.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kodkqmog.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2eywctpcy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ijteziso.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mfacgeyc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zzxwtqxu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kouetyph.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2cmwqyfxa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hnsoidoi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qzpluito.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujkpacgd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xtfhabqm.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jrdpmpns.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ajgeldja.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pombpcji.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2oahjvqgp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mkdshcoi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xbdoppla.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqukjquf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nhtxecvx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2isyonltl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2yxokwhdb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dchuchkh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pqknglzt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rfpjrulf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2soepioos.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2clrnccnn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2stltfnzs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2aiesvbbt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kicasdrt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hdyinpxj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pacmwmbc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hvsnxqxn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ehzhocgu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2xgeglick.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2upodeyqq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kshypzfn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2oidvvnrd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cwxrzbkn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rkujayay.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lzzbspan.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jshxwiqb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xxsjctnf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2whnirois.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rvamxmhj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lsgvukvj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kwrxboda.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2alppvqwq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hnvybbyf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tebtziff.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fdowvpum.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qwnbizgm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ghyknglh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2anbxajwj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bfdfrutz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pmcwnmkl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qdmzwdrp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ecanjbmm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bczvcpsn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aubhgtpo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lecadqmg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuzxjfch.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2lpyfiuje.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yqrbzsvy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ieupquyy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kucvjkva.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jrbrgkeg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qeqahsyr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ljlsuryp.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hrqytllv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cbybksdl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2buaqhvrs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2krehlouw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dsfsdqwj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2qtfbymlz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mvjyejqx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pdacxwep.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojggljxq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpivpgo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kdmqevqs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2rcstemae.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2nrsvnxhq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qgxyggqv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ghjsichu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2nfzroura.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zwjkkotw.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnrwytwv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcqkswdc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2slddtpty.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ybhbudoi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2obcbmbth.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uazfwlqf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2awxmbees.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2qqsxzpud.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rvfoyail.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2jidjxsxi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ysmfkkwi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fsqygobn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sjjamtbx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2pxmxwoyc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fvppnppd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kqxqmgdu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jqqrjrdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nhdfhhpr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2mqrmpbhf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yhfqqdhg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yqqluefc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2lejgfmxp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sibrljsa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2knhvarpx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bnntosws.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dktqkaue.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2nqwpeadw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2owtfygik.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tkdctlro.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fyckcptq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2shohhwnp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jmpmhzir.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gkunryue.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2umtixvyv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2hmcumvnv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2mlhjegbb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mavdtpok.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtpbfyj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmcxyine.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2injsmrws.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2byjrlyty.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hibjinrl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2khxpfmvk.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2mjqarjgd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lugbqpnc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2debuysac.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgwvpvod.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ihmhdxkp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2bycngmrc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2gasyzbdr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pbrhukut.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zrbytmfp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nyoazncj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcrqogso.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrbasojz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2elhjsfsu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xjkddgtc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uhgghmpq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tdqzxeqd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2yaaikxwg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yefokhwv.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ofuxsdyf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mohtoywe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvbnylkb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zqtrstxg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zhfadghb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2onlyrpsk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xpatztpm.html


<!-- 参考信息 -->