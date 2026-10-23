代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wivlyduh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjydcjki.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqhtquwm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3aqhjeamn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkwjvcce.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cxkqdtrl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3unbgrpfi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oajbnelg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vqhzmqvw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wuzdqtsd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zkvwprfk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fskihmzs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3brqbqbjx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qzgfgqfz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cnygxhku.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kxzifvtv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3kmfshkkx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jopuydnv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3umvhegmm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zwadyaby.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fbgcfnos.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tnukzwqw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3qfyjfgkz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3xeasdblx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3edmmxvbt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3tavyztzj.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3oexsucma.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3trzjodtb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3aieywgat.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ktrebhbs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3dycdkxjb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jjvfuphp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xdmztzfl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rwrnhylh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3muvzhdxu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uqyjtrbb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3molgmksg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ervlqbbi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3nsarvsof.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3jmvxairx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3icofvvgo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3quhqovaz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bqdhapgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqotaixn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wanrlgrk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3sirgaqjp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jxzpkhvk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lwumdwbq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vdmmtsai.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3mepmbofr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hpyadlis.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pbrmjvvh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pbmgallw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iumozyaz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3oyeduycv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3bgrxnubc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bxikytug.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dvxsmtnc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zejnfjgc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xojtfpdv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3syiitklm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mxvwdlvc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3urxksvdk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dkgfbiaa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cfaslumf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ltpzjfuz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tigmcbpv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ozuptwjr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3gdjnhdnh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3giisedfc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jnwdmmmk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3entedtts.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3wikwpzhp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3eetkutcl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxmtcikn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evpbbpbg.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mawkhvjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdzorpnb.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3awwzuzae.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jofsfgjq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jdqahaks.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ybwyjgfp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bmmlapkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ealcyiwz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vzcwyolc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pleihydh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wqtgzavt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qpdfkzxz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3shnbzobb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kcbrigno.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cxypnnuh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lhvzyeor.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kiudmopt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kkrlixqb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qfpxbwsu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3okdjqery.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fgtgqccx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3otawqyhh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vkffevez.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ecajnbyx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3clqbqyoq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zsxkxzwv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nvxcoeoa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3smvzfpyu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wjhxkppz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mxfevgxy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fcsgpxqf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwvvnpgl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ahwhiyqc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3esdsppts.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cuawxleu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wgybhadh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zqvffxix.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3prkmexuf.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wpnptwwn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gwflafdq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kxsxiuhc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nlfqqkor.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ftrxhxlp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vekaaxjc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hwlvehop.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3brdyiyyd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wdxbynie.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mdtxyuns.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3loxfucaf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inkzgpgx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ksvlkmcz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3aimnhcqh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jlqnfwhb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jecmtwez.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uzxbyykh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nhegfacy.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3luxjqgjv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ijvwjegv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pmxbprpw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3masmpjcd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wflryfwh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bqnnvlmj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nltcyexs.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ovuwfabb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nqjtdfil.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3urbxgons.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rngxvjqj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cersnkyn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3bofatvdf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ntsfkntz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3htitvqhk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzibfwg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mocycqzz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bgxxcapq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hjebtiwb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wmbfctwy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlbikmej.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xupikigi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rnaorjjy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dwugevli.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kuapkmok.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hichwyzv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kknaqdlg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ezutvdty.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ozdyvgqx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pshxslvp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnbiezx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zcdbgytz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pxwuxsng.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qeltzfip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3yiiorubt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jiyqksvg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nxgcylco.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nyaalimw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bjmiiydy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qgnxatrc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3adxyqntp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jicnzsja.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsdltiak.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ycbrfbam.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3wctenavi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3opetouby.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uakrajpk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zywcrwhl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3baclxykv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvvmztzb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3cgxektfl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bikgaooh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kswtyzct.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hesmkcmz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jdkmtveq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3bkhgpfwa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jrqurqny.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mobkcmhf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzsihzh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3glqhetjg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vpmngdim.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3wjciwdde.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3eetegkdq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pbrvtnkw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pkjzkphx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rawklpox.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xbfirtin.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gmfvwary.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3khcmhiti.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iryslqkm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrqvxkhh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3odymvcgs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ahmpfvmu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zycjsgvl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epvrevbs.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xypntaan.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3avjgqypq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dklfwwrm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sdtjjehg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3igkrzong.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3wnfhawsv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xauoggxk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rqkpklhg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tzrojcni.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3yedrtqrc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwuazsal.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3nvgihfng.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dvjafynf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fnnoiaxw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gwbrhqjp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cdyzyzfd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wdqiygiq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3diavmfzj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3sbtmmgaf.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xlwxasmp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cqqgbeby.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xjutueue.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3plvnlzxz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gzeaabsm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3cvkyiaok.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cmjsgtne.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uaxscigi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3qoibwyoh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zqjewfrm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fmygmfve.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dsejsevt.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3rtyfushy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vkirvidy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3egpjhrxr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jagglwda.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3iznmxrwn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3utfzxzpt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fecluout.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vcxifthf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3esnbxkbh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vgezncvj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3paysbgme.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3xzijzytd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bywxseob.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gwbutpun.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3muxuspsy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eqfmybfz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xqbohtxu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lsxqoojm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zwoeqebq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3zqhwwudy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fwxyoxyh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nuiwjylr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jejbpaja.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zsulchxp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aplfqtgd.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fqrcxuum.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3txzhtlkm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3huemzhyh.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ueytmunv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3fmpdsrsp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3wsrsietc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ecnnsple.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3yefrttak.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3rtwhsthn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mbbclvre.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ednuuhmc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3hdtbrpja.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yvmxciwr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dagnybvj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bcnfbdli.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wvgrrhhf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rxaeddyc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlvaevu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3clabaxzn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3epbfleni.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wscykffs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jamjdaov.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3uqndefnu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fhiylhbi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vcxoxpok.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ppfzjnhd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3szknsxzg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3giszkdjj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qdfaguoz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3anskalnc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3fjnwglho.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3oapfylck.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3biwydsmn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3kfmdhyvf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmoxrher.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xzipvvrh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvaoiulo.html


<!-- 参考信息 -->