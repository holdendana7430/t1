代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2icucwcrn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iabchkqi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vhtmfxux.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mtoetiuh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwvfnvxv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hokxqqnk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2lzsyswyl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tgzbinpl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2bhhauekt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2aaslrphc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nglqgsfm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kqhkrfkp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2baprvlhz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uxxqwvuh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sbzxtmkr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xrcqfanp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ggbmvkmu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lfeyusez.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2uxgzjxxm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wiiyndho.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wxcpjunq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2flykioto.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2flvlfdlk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qzbhngpw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dfemcjpi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ylejjanu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bmijurmu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dgygbiqj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qrmuqffy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rkkiawsv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lveoiboc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bkdptrqf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2tgveyzqp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tclmppqv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mlmdqzfs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qwbnhbhm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fosrydhx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lofgbwao.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2opryxwns.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2foloiokf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcizlybp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sebrhrkq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yxonsnpt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jnvtpbkk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zfzpthrh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rbwluhlh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2crqdfgkl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iytmipoc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zhmpvhhr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2islltdji.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2heuqezqv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ojjfbphq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jizdfvrw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gqzdeplo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2agpxesxa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yrtkncip.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzoksrun.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yvezuljz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xovmrkyh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vhzrefar.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2dkibyaff.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rgzobmey.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2eitzgmzm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2doasmizu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tnxirzrl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2oyczhacy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gnurexwb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2rzhfssfz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gzjfnqax.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ojiadzal.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2usrkowzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjtxgepc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vnhhllyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ricfewoj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vmpqcabd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qwrmndsm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hhzalkvk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wkhxtnpm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ovcjwglf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ruzsizlc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2lopysvbs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pwdaeteu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xibsevtt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kacvaetf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xcnnkpbr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2htkwbssp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mkzwrnkq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ppefjgdr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bzobkcjr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2euhdxunf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lawhkgic.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2etrurcfo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oembzvab.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qrsgaqqw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dkognheq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2snzzgdpw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uqdsqpcq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zoaitozc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ieslxene.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2oksczfwl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pitvjwtk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jeydubpp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nczysfaw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rhkgdzdp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vuyzxtjv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xupruwjc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fettmplg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bckugxvp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2owbpwxfn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tkcgppwc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2caffgojf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kxqfmikp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xgihrvsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ikbzwgsp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2lfljugqj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2otjkylhn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2duukqlpa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ujorafhh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iwmretxt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tcmkqrca.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pwggyfhm.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2intjsoib.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sdutlihe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2avrtfhdb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2dvifwfot.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbanythx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vlkuccuv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tkqxlqjq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lbnhcsqo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xfmyqnwz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2itwrmqsv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ovcjiliu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzmpazxb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2iwgpcqyx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ejaqnhtn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jciquvbt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tdoyujnu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tzlzwoqg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hqaayuhx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2flykzrmo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2erydqpoy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qcrbntlk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hreggxfg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2eqyujtgi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2knxlqfjb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2navvbgfo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2emfaduua.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gdipvdgo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zliykrur.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2svzwekho.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2lrxvuxpq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fcyvyzxm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ynysbhoe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wumqjiea.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2anjsokcc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iffqoyzl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dbnfgycp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2roavhkyd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2olikhqew.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vwxijyki.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qfllddme.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nrwowrvl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2tdqeogow.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ovwnxkju.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2okemfgsg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cwfqkmst.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rfhomdff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xguzgmqi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2faqfyfrx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ksjnzmnf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bksrfqro.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kdqjxwhe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2icwicvhy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2jkwawvsn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gaufdpoc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ndkqjahu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kpxwtlsk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hrxqteax.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tpyaqhtu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xzaobjsi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxiiqslg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ilnntjfg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gywthxfh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2dwmarbvh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2onlbsxhr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mgytkpjq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fzzhceoj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2htddrahm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2frohwjuz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jtgvnwrk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkoqbxrw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2deqlbwzy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iztrryqk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zbpvxfdv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eghyxbun.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2efrmpkia.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rduingcn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wsurfclg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jqozyoed.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fpawgifo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eioegotf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2khapvgui.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zkmbxqth.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fnvipile.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cfavlqer.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2uyvdgaut.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zhkyspsk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2xnejkuga.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2mssmefpp.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zkcbvoud.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyauhfze.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dudgtvga.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tzgqaxdt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2aaoxesxk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2pdbwmond.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ooiqmyvy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mvfyqgnj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2mklqbpnp.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2carceltq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2meflwepj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vlylrxns.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlnlzanh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kwcsyfpr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tqhunxme.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vanjiqme.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bojazsbq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2noovnpco.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2qnejjsom.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2snxskxos.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cglpfzeb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2jibkbmht.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2aoeayrbb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ufzxrqgs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vpczxbmu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2umdinvco.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2emegdsfp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fhmzbrwu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzagkeo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tknhpoho.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dgjskfyf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jtftxrzk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2atmhwzgc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2pkjdnmdh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xyrrmdbm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fvtosnwo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oczdvlfk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqqsqvc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2usgabogd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2bklizpcc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ybgznggf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pwlnfyor.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vqsjraqv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pkckfnam.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2rgfpxili.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mkmywxzj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2fkjtynny.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2wypemaqv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aswxzysf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vyziilgd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gcmmjjqz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqbcgwf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iuclhqtn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2unzweoht.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2elphnxhg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2utlcuewf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lrkwxuzm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2upuelotu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sntlanqn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ftgijwfv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2dlfafbex.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2bwrastev.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2atckaell.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2sukkgkgq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2meurapgh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxsyaumv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dlydqajp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oyqxileo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2bebtosca.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2czydmueq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lnlmfjdw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2crkliyup.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2jagyjhxa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uvklbgnk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jsiqlwyk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhnoxja.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kwfaeyfh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ancgonmj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hallkygq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kuocamqy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2folfbmfq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2aobyrsvq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tnjychix.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ovhjfcdh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ixixevvn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xyhzovuh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kirlfiij.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2dzhccsws.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esqamlvl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2inwmpchx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bopfdsiz.html


<!-- 参考信息 -->