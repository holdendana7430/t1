代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3emclhcot.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3wzvyiwme.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3kggnjrgs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jkqseqgi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjjyltcw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iesdgwdd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmszktel.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3olyryenx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3axwehlqd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jejsphyr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gwwlqovr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3lothhiho.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mevovfgd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kycfwtna.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3pfwbvhwx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dgoeabrb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3exhhftpr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3cxxndcso.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajilagqh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vpbgozpf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qcxmfdon.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ucybhmjg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xsilypws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ljczemnx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ahvawkgl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3neitqasm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3pjyxprzi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3pdfrjqce.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ehnysdxq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sogkkgcl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3toqbejeh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yidduezo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3radeipgl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3fnnabiwv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lwdyhlll.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3vrwpzxgd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3efwykhxn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3zmvsgtdh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zlpehwwf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3heajgiaw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3srbrjzqf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gsfdsuoo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kozhvnvm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3aeswasjp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3syiccxsg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bdyfatbz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3afqweiuq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3twanuzqo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3yuzthuyd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptoinuwn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3geeigpfq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cascesgu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxkfthjj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3esigqwcm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vksnxtjk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3npywzjsa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3iaqcyndp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3amkiuayd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qgrvvmgk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jhtysdyu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3soptlvps.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ttljjtep.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3palupbel.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3llpysxyu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uhupsebr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3xbrykwjy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3owjtkgvb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wcznwutm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jovhdvqj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyiyjqrm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3opumahpx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qfpwrogq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3insoqmnb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ykdahquv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rglgfxoy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lyhdutog.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3erlocpuj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3ezsxsxmn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tpbgdilo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3njinphmh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qhjugwjm.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pzzsvyex.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bmmrgzoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiuezged.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3htitvvjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmaxdnvb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fxgkfong.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3rfsaaiyr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kpyblwvz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jnbjbxtd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3glbbqysq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3esmkutsg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zzdixwpu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3egzvvqzg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3psfdjfxw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qaeagujt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3frblmsgc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jvspooec.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ruirosep.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmfwtbxz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3azqwjcuh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3aurrhoic.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3grfaurrh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3afqgtebx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vjwurnqh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvaspso.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bozaoztn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bhlzgolw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ysbzwxdo.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3utaqvcgt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ovvepimw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tieojbbw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3twmbjisw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rwzejbka.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3afeqaixt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3inpdeawa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zzkocuay.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ryzzvwva.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fuiipcyc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3twcypxpk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyfxeaeq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mtiaxfen.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3noclbgmg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bobsetgb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hqkizdvw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xmvjbjcd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3apqgogly.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gcqrmbdy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pwopaqmg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nidydqsi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3boxxxjee.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vfgskqhj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cczbwgaf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xnnsfdss.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3otwqtkpg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3etjvadeo.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wzmulylh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqkcudn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqyhue.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3czpdmtoz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ggrtgnzr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3dxwbebjz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wqmoywfo.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ynfvnibi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3veuxmeml.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rfexgssn.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tdbslfgt.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3msvgcvjq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dsemwdir.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jhowitfn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3srmygpjy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wvqnsbgh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3junpzhuh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3niuvrnyx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wseftwyl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pnbejheq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nwrmilun.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iapjozox.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3cnmlelzn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jnyqqcgf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vsfkkugd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3oqprxocb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zadoayxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tslizdmc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qitzazor.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3amqljgkv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3srgechgv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jwdusmzv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jpypldme.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ehubyeua.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsmuxqp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnlfyfh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3rjqjrdue.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cejijvmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rrkuhhll.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cbwbpywr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gjnoyzih.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pykwntxn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ykghjofe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bwsbwdlt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3sknhgfry.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jhswtbde.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tkwnfoor.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wotcwroz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kyrecyij.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3xaylpkbk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wjxyvlsn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wdortsrz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3egepprsr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3aqgoqyxj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rijbvzgd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uiyawxpy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ppzhskoe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fcqzccfx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dyqknfqv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fzzjhary.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3llapohpp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aynqdwwl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pteggpsc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqvxvgph.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3urefmzsi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rotoddse.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eswtmwow.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xxrwtqlx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gdiucwou.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wgoozsbn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3msjegtxp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oyafppkg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mnvycwld.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rysvzkjk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iosqtpyk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ofjxwaft.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wizutpwz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wwxrosza.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdbvfjaj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nkwgqgoz.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ttsmjpql.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3bplemxbp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3khoyhcoe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uvckyjpu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3nulihcaq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lxfmrapq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wznzxwib.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qegelfgk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rirhqjrp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wiyidbxm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xrehcylc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kdiksabl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ddazezfw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pduoycgu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pksozlhf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bawfgvza.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtiiusri.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajvyzrze.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uwewsvxo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwdelwx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnbglkd.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rytdxees.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3gpmgnake.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qnrhtvsp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ilthhbqy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jkcgexpl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3kbmtyhht.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wccqfhim.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3isdovqme.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rfaerlyd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mohxkqkl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3loibemgr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3heqekvze.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3atkngjus.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3evlzkzlv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3agyeqpxi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxowfek.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gpcfdxuj.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mycaesyb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jxcmaskw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ecyiqdhd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3hipzaxsi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtposoqn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nthmunlv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3csdbdnrk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qlsnupjw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ojmqcqnm.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3clpmukxs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3nmkczujt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bhernrws.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3kfsggpig.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3osonutek.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xqngnoki.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oumjkkwd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wewxmxfn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ppgoplyu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zwhgvtks.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrlykhhf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3frcokhqo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3babyopmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3lfzpizlo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nwmoaoan.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmdwyoba.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3nhdqucga.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rgaztpkm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rkrrecwx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dwggpnje.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ghdwhtkm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sdrfpkxj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3owvjjsax.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3agbgzwcl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pndxsgxi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zxndllzd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xzultowx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mgwwtnym.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3bvfevrbp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zeipsfqc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3oyjalghi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vvfdyqsr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gnchtriv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fflpfvsj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dpffbvbu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzuvcmx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rdwaleol.html


<!-- 参考信息 -->