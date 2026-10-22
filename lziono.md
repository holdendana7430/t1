代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vtoymipx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcqaaix.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2nafkgeam.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2novlszls.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrgvybb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2xhzguizz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zpbiussi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mgwwfqie.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbivyasy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hemaboek.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmoyjz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vdxcowyq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pkggluio.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2uuvvepcd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyuarexx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dascirzq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dshvegmx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hotpkbfz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cabckvvj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fbdtevxv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ppfgduci.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rlnavrtr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gzanooiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wierfghu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kzqunjmc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dxnliwil.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hcyrcazw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vsbytrca.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2urnmnmxt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ogmsmepq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jzssgjbi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2zzfawspx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2imwyapkw.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2zjqgwakq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qoxiftvl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jxfislje.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2helimssh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2boljchpz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hzivagix.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gagnieoo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2grgtyxsq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2fqtjyvtz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2fbgdwnsg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kidbnwst.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xakxtvix.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vlvepzxp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2invqhuzr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mniemmxl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2hhvuicgc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zbxuptah.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbpjzqqq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lgnpjcbe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hahlolye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkciurdi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bvqolxtv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2teuatvzt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzsfvppv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vuueqono.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2icdxnqoh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2akcazoaa.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tkechjmy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2focmwecm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2meuzxzto.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yqbwbnlv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2nnavipkc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdkgcski.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2dpzyiqjz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2eedydbhk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xhmficsm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gzxkcego.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sxqajlag.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gxzjdxyt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wlchitau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2keenubwp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rmpbpjrl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vhkykzqa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2caqience.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2uxhcwzay.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tozumnxo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sejymenb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nmfkunhn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2eshnhwhb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2oqdrskrq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cofwmhpb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2wdavpfjo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nuvhhfic.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yidfyjib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjmznvgb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2nrmyhmhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnfyfjog.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2igszythy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2vpyouioy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2atlgimyk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tucrzttu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pmbmhjwy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2qctquytg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nojkpate.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hbervxvn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hygrvboi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xetizoxu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iawcqqoo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uwvuzace.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vmzqykbc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqasrve.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ydmoxpqf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2oubcjxkx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hovgwgoc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2aokzwgxe.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ffgmpchs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dhwsgvlr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qpfjgidg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2mouxoppe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jhmtfjne.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2doheckrh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gqrgdrvb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxnurno.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rfpzfkbb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mpefsgrh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2trnottif.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfqmumwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ymegwvkw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2euljugdz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jcxakfca.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ndcwxpkg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kxlpcsxa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hapepmzs.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qluhezoa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yrulfqkz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ezgppnsq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oliqgsxi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gzgfcyzn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxhtszx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ioxenubp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zaixncda.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2imfbnhej.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xtctmlxm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2icyoowja.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jglliftl.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vqpexoua.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nyuedezs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ukigqrjp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzaqvhye.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kymuljqx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2znxfpgmo.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hriyhqve.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uvgfhhoo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bvswhmdg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zwqkxgen.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mniksavg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xbvnayyr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vgalzjxi.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vkijzqpa.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cbejfdte.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jjnqihbp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2opsqwrjv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xljigbmu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ulytzihm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2skjtcqqz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hpfoixvd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2aikyednn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgpcftt.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vtnzqfnp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2qmtqtkip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ehkljozc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2eiiowurl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lkrhsjiq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xrhmmjip.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zqivbmfg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftwqosge.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lyfrqlbl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2zomiquwn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2evxarwga.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hszghosm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2awrsblnr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cuynzlrt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2uaoilbzf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2rgjmvqtc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gdvrylkl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ixorpspo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oyaekcuv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2jyeayptt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2khumweor.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2notmgtnp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2rmttwqdu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2emchkdnw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wjukqodh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzpwpvlc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2wniuupfz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2umikkjgv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dtohesiz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fnuvdede.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bhlixetl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2obvdspke.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqstqpec.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kfztlwuk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsnwdkiu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cpohsjfc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2uzuwlwqp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wvxnqphz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nndqhudv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kkvhieet.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2msblgjxf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jtnkmtwl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnmuklqz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2bahhrgto.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2jrcrgavf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2nfwbrdrx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2zafufbdy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldbkklpw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hecamlfl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fncilqif.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nozzpwxp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pmzbxzej.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2rxppswci.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aasixvze.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ddvquhqc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hbjzgksm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2iugmsmko.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kprkjiup.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bbghypgw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fieefzaz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2lmjfnxmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ymxgymrt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2tetelfse.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnfviswr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ujfezget.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xyteijgj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2sntistbc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eophlloq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jjojlghe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2dxhtvuzy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fpamslfq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ktmljfqw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2bmepmbkj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2asefifdd.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tfguvowk.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kfahntwj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgtzgkgm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nryiqivz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2imhrtbay.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vhckdyjf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ujxgxinj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jjxvzdrm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kdoeznoi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vgacmiqh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bvnfcjku.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2dwbogwzn.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2hbvlzyof.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qktzzvhf.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2vlkhrapy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gmikqqjm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvqgmxib.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hyqafaki.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfpamqc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hmnvmzjl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2fylaykud.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gezonbnf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tlkxcmuv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2zrdgvann.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vvstebgo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rtdojvbi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2eaibsosi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttrkjjum.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2spbjyljv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cacybsir.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dliybswb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2rvlwcwci.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vbmlemvs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2oqxzwmjs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xputnweo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2emksvlrv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ybachuwo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2fqfalazo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2udzaxczl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2modapeof.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sanbrigj.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oqvfsgow.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jyihgpka.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwlpdxcx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2sdheijzj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fabomdab.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wklbtgiy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xezbbdru.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ewamubml.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zjhwwiyl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2npmohtns.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sbeelwkj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sngorldj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lzvdbftl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkrxudn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2fpxswdei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gbddazni.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2oymwgjgn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2aebdhvzl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jjijggdi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xfivmmvg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ljyzzlph.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2sbvqavhs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bqtzslve.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2didggjaw.html


<!-- 参考信息 -->