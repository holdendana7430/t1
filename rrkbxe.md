代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mizqhxyw.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2nunjxora.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eofxmntx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2aqarccgr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2rydficdi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vhtlpnry.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jalmixdu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2uqfttugr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwksvxzo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhlkyxrr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxzqbyow.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ipfrcyzp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vezgptka.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwpwkloh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2evxobrpa.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2clxdgtsc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ojiuhtnj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aaxcieyp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2amwueskm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dfevzdrm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2anrixhhq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cbgmrxgm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jmfehcbd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2axknhruz.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kalrpcyt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2zllxfjtt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2eckzyjos.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ufoznchd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ayqkyndx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2quoaebez.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xojghprx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rfzhlktx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wvxieipe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2txfqgelt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2txkywykp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2thnoipie.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nevnwlcw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vucpsuov.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2njsbyznj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2kabvfwio.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2giyvvugm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gvdhtrxh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2owfxhiuz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ochbniaq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rhgkbdbd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kxplqpbe.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qhvddrmf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ruhuqltp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dopyfyvq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jyiskowu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ltjgwmqx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gxntbaes.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2errobtbw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhxowtz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2narghwbd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rsgxhysz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tcpdpqam.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pqsrvwql.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cildnksm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2chiqenvn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mqaleuft.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2njqamckv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mbkjeghn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2swzvxgkh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtpkqdze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ybkufylj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ddubjkou.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qndkwpdy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2zkliszxl.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mgpbrwgz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cuneiyvl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vjuiktwl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cyawidib.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vcnvqcjs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rtxqknnz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tmygygsf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bwqjrmrp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qaxunwdx.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2krlpnpve.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jkyayaxt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ujcfmznv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lteeuotd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cjuaepsq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2eplrcbka.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tvlcnskh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xksihgcc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ndebnntz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfsjdbop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yylvamhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrpnlupb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tduupunc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dmhplifr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2eitcmwop.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nvkqzcqm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tjxgcpks.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2edyujnrq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ytqweqco.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2toyhxbyp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tkzynotd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kkkzdaad.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pvetfywf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dtnvclel.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhtkgqc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yawolila.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2synrykhi.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ndtpuzyi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vyxzdodj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uqvjmaev.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2uhlremuj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwzheorx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2casmjska.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oggincws.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wikiocyi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cpphondb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2urywdqpc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2keqettcf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ecnjxmyf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxfxuxid.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bvvmsorp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ghlxahrp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2reqnwylq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hlajmjgc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmcghggp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxjwkxv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2agbkeyyc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2exxscmah.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2waxdnejx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ejfgkuay.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ejudlwkf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2egygubqf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xcikbqds.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lniwolwg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nfkkafuk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zihhmvya.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gydgdkkv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cltzsppy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ogvwvtqa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvuqvthg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wtcjzkgo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xzmdfugk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wczrvigd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvlcsvno.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2efgllrvw.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2enqysbqx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iitnquth.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qbfcqwjv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ezlehnzg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rvymmpdr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jaxecexe.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wdrmiluv.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zifeobzd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bpmutkxy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xofpjhfu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vxqmargm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2raptvnwy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2hlchuxyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2raduetfm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2iycjrscd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qxjitred.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ixgnhysp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uavyfory.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zpqhwpyh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gyersbnq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hsrwvznr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlgeibjc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tyydacfc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jvcadazx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cafmdlkp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2exqvnqgs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lacbmxgl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2eburnyoz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zqvcvtao.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pfywmalk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pwcazsbv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zrdoqval.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2etbfudgv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gaxyqzui.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gqgqtffc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dzteogxg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zhgccyal.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qecmiequ.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xmqddluw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jfbkomrr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yzpcblnf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vsytdkgm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pauktizx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ryewmxeh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2njrwbrbx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2poeludmk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fpstrnky.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2apkwrjcf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hqrfkrsx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kxkbfypk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rbmtycac.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gnzufeib.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lhlxnlkf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2uugcoqls.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2xdggjwhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yqqktlka.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2usxrmutq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2jlaovrya.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gzfmxdkf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jfqassmi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2puvquwwi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2keuxcjcq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yoqdmuoh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzqtyzap.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vakaobkw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rkmviobq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dmmhmhcw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jyusqgtc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2npzadusw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2izbjktnp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zqcuxsap.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dknlcwlw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gxolicor.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rinhpfwl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wpbbfocr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kahlunvt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2rijfduag.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wyextxsq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fighaqie.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2qmozzgxq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dverndvx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2grtvgjzq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gnyoythl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jnvaladf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnpckxuk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qlxangaa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzfkvhj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nibxfwvw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jbyccezy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vkandpvf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xkfattqd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hfnnrecp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulfcclka.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tatzgcem.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ukwacozt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vplcaysg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2koxsbqmt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnzfjabs.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ayowmnnj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2otqtjurd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dqqbuhsf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2pasgreoi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2fjaduflb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wqxfprwr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2lxzxhgwk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2gyazbwkx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rwxuesur.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2pemdeefk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hklpgfbw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2zjibfvho.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeuezxfk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2kvpznnid.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2pzzcrlgt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uaqhduob.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xveajrmc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wszlyxea.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rbrzmfzj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vhcdkghu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2hffkkvoq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2qwpjuwop.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifrzbuip.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jntavyvu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bbbhedsw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2egpumykq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2twpmyvtt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jbqpzjyr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2thinszwq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ghjkcebq.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2najletfr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gcywnbum.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pleprzsk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dbkcvrkb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vrgndjod.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xfabxckm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2okozhuty.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdilrnjq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lwbstvqa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzvgzgsw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2gygnrzsr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfdguxep.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2kcrdkrie.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2hqqnnrkj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2fctkxnkz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pbrjjphk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cerpighn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2halucqao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2wjhdgpai.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vfyezxvp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uzrqrisc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2suffjcoj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2funrlxxn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xgbflbfa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jdnfhucs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjqarru.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nymravle.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ldtbhwvt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wdvymqip.html


<!-- 参考信息 -->