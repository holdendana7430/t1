代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3iwcqmial.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dhnpkcvn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3etjltpoq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kdazkznr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxqhfppx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxhmrwkh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlfzwucz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3pbojojqv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mzhvtpfh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3sdtmziwe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnblesnd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3kcfccvfv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqiyiemh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lbujjjau.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3skervsat.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ucljpzyn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdujcpwy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dgeyqcxj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yindzeqj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3puwvxpdu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cmyqgsad.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wmpjlzzo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3igxvpatu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lrpgogro.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cmgyybpk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jfzclbsr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mkotkafl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3nxomdvku.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3euughnuc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rbmnkjno.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3itnvowyo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3snhzypbi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gbvkhzls.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3twrygczj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nuntxecy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xtywcijj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3whbqxxej.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uoxdvquo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3jsidffvc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hbdujtks.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rtkxegea.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ljjltrxb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3azgtotvv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3spxyrlrt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3llelsevy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dwnkzyet.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cwpfdamo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xouitqkn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mypblsge.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmqvgur.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3scneuitp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iwgullik.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mweiersw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ejleqlfc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vhopltna.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3uqslpevz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3smyffcbh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3urvuungk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rdwivshw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3skszhpyh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnqyhuwq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xwbkjnrj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3eqiigcnw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gfbljwfd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jlaukwpp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iiihzdgr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fwoatwdp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3eklmjhcx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cbhdpnbv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbkktpth.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqcaakfm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rcptpetc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jomigvia.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3frxxzlqz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hlqtmmin.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3aazfbpth.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qfgcsmlw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ogqnmoey.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wwvharbz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umslfsmx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3coovvvtg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xvwtzvas.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzzhmjkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrsvcdlw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xxiiuwet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmhhjhbh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wwctuihp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3srpagnrh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rrkulmef.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qblnulig.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kpljuzet.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3quswflwq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ldqfcghq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3omgcnhyi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gctlybfu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3cyotjhoe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3oktgarqh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3iazodjqf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxvcyhjq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ulqinztn.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rqwjxpcn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oakiivqd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xbughjbn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sgkkmzmw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3tejorsgw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yftoppdk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3svbqlbaq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3whtdimpy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pllwufoq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zjmdtzzt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sypbubse.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kuikvcwm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3paptncyu.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lbhbfeum.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bqnjwwfx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndgyxxjq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ghvjqhez.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ombloehs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pniugltw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ikbmeomo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zabpwfpe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3yybliphr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jmsamwth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3crmzirqw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vsiigeup.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3eqntdctb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vygfxrlr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3rmpiagad.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wczqdluh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jujlkihn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zuvumgjk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zulatzwe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rylfjdup.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umawtxpg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3layldgvo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fvyplauu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ainqcczw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhgbeeps.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nggcwuag.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nitbeyfz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xsnykagy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uckcjbsu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tevvvnld.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fiakupmz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fzauoceg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3culjtsco.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dnhrdnhx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mvbsyulj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vnsxolmw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hjnjhaby.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kydiqdng.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xpqrexgm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bvbqhyen.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hlitwheq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kmlxtahd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vkpsethk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3qwbytssg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gmgcoxhn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qdkxfcbk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wqqfbxqf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3brdykvic.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kvxehrch.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ossucfnu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3phcfpdon.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3empqgtie.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zdcfdewf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3bmqoswdl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ybwmhsms.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3qdstykpf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ammisgfm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yyxxkcfg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ueomqsha.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uowtgqqh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qymgbzgl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ykrthjqn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vafrhjhq.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sxxaceja.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nlobjuoe.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hixtcfbj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rrzgalrk.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nshcnkac.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gbsnmtgt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3slylmgoq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uhdxvxtn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3cjbovoqq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ipqbuagm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tcbtwugm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qlnqvteg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ewsflwwr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dpsafiqd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3atjjmdcz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mrlollex.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3noxpdzrw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3ygrtivdk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ijglnanz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cznryqwh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hwvuhwey.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bfqbliut.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tognhxci.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qzogcfyy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cpuvwvpm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fhrkwukg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ysvdecbs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3bcuhxjui.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cindxkhm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fektwdiq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3luhpydwn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3abbioiuj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrtyvgbr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnfneddl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3rvrkaqii.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fachmrxs.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3npnpllce.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jesxinua.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zqeyiwag.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jvqgaumo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pfnzsjvm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3imxelexr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tdqzuqom.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vpfiqmfq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xpxovsup.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gvwckoyp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzysdfm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibbgosqv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yempfjvp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pctefgoe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nxzzkszd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3aczehkdc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zowajrqm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wvkxoqah.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3rnlbqnzp.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xnotrpkd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jlnmwdqf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmkwovgu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tdyfgatp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3hnxmcnwj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbgjchgw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vhirgjqx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lgfjflha.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3chxlevzq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tytvnvee.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3yyrjpbtr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jkefsnhi.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ssgvojjf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wzkokxof.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yarittty.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mdvcipbg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yuspeyjw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wkkseufr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3grjrvkbj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ymqdisqq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ggettjyl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gyfurzya.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3eonjsiam.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ksoagqkh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ckezyfeq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fzbcvzfq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sgxpinje.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3uplinmml.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yimoomxa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nzvdeoqa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mvgrwvli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jozulvvk.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3tnguulha.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xmkwjydj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3wilfmmfa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3pvdcjfpr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3vhwmaqdx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3byqmbmrh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnxcloc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cjbbzfzi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgrwmji.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gtscqnhn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdfdlag.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nbedipyz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ypygftya.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrbemqe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3tvqfafwm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mnnuzzbu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vyyokdus.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gzyrkacl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sjjquoqu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3rcxzagdq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xkggsfig.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3diijrwez.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ymwfetzl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qiikjwzo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3maojnwyd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3eccvwspl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gmqfvywc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tqpwjmxv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3jwsttcyz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvajbbco.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zfnbpupw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zqqfrqli.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3etlcsbmc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3adcizwqt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bidqtmph.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3btjgaptw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3unqvxihg.html


<!-- 参考信息 -->