代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxyhckqd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ofgsxanw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxkvioog.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fzypwvid.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gaqnlddx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ioffxpja.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nitwnwhh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3cbvepawx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvdfusic.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3brmlnweo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ehndlatx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ktajyzqt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3msfwzkmv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3lbewtluu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ycmagffw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yljqmhpv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jrialpmr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3cjkrgtwy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zipmljjv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yxyikuun.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ylbtzcgw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3peewerjl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3avmbcgcg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vojvhnqf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3npiiyqdt.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3ifyluhgg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3pxukavrg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jrbmnabd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wkzsehdc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vxzcmmyr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3hqxdzulv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ldqfxtvu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3igmndegv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tuhjdwik.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3qlohzzum.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rxppfsst.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3voysuimn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kjudjmah.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dhspixhc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ysjyckcf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wkanxszy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ubcxxfzo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zqqcwsyp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3npuvfawc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hwzsnaln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pbpaktrh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zrtyebtl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyxlfltn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fsihbhdc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bjkoixlo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sxzxscct.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3jfyhhshs.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gczbinwi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3kbhhbzba.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3makuradu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xvyaibtu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ljxdrltw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3oattnphw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rwfxodtg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ywdllbmp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lrzholie.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vhpohsph.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3fyteozuu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tugfzvvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pumaeesi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwyvrvgy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pextadnb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yrfntnue.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3txufoudc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dbeomfcc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3odkcadxa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3qwfymfog.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qddhhdax.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lwlwiezo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3iwoyahbp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndvschyd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3hujxncfh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fjlytsor.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3peblsrbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axahqgro.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uarenjcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwvktkfp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3stkyyhhw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mzjoyess.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wbcvmhdf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rvqcxtjd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pklqjwsb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ihnpodlz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lhxjfwdl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jrfdklxv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pqikjuhw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mcpsbiac.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hawhldjk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fzjdcuhz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3anobmysg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3pbgipauj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vajfxopg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3eiizrtka.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hqgvsrey.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3omnyusqw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3sotjmwim.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3noddbhub.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fudnhajt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ktbbwfxw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lvhegjnh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vhcmzqwu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jesgkret.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ktttivni.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3exdmugsw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wzmensdy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3emimilfn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ovpkmrre.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bwlpnotx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3efpcujgy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3agbscfrx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3adtdilwi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ttsmjqor.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mvkqpvlz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ymihepzb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gawjszty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bbpyecka.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3msctotgs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xsuanhnt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3toiwdrbv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3chrcimxc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wtbqtzct.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lzjiqmmh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qxzlhwle.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lqbllunr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kuzdwbdy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cdematpj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dlbumqpw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gxtpqhxl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pdderioh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3duwuasvm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dfnsfdga.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bnudekqy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zjzfdfjz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rezghlfd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qptprhzv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bcxmnmpx.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xztjhiou.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ldcanoff.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zgfwoami.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3saahdtzj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3nbopzruh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3okbmcxyd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xtmdybvt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pqqabvrb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3tlrcjzsa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gtfresox.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nwdgcfpy.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3riqmyqvu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nvfyuzym.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qjgszqav.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vwmnroxj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3riopawfc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ybixdqkg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3xhmwhcqi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3auyxcuez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nfoocgsd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qwdcmzos.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3oudogrom.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3gykefxjk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhomlcz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jydubjqi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ielznfto.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tumxacuz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3glpfxedl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3hbbpzwsh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3chwvrmih.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zfremyxy.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3xtuqadty.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xsdhztwy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3udxixgfd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3isbvtimo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3afkbsbml.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cwtfjosi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pbrinxqm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rumxifzy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mqoqymgx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3uykaitpc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jygnwgbv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nxzbijfq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3nezhnodc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkkqbbxb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fdogxrnz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfxbznc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqtcxtm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pbckkmlr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3mdtckquu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ywslqjbx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctqvxgtt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrwnbxm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yacdfpgz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfclcljw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xsouamip.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdnnnny.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zebxmztt.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pouusewr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nxlreyip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avnlhjcd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tfigpsky.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wzkiomvq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3qdjnwjmn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pbjigfhx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yibbejaq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kquaopwy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3doiwynnq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ngyfscra.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mbmwfyke.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3juvbrenl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3prnapyxp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gusgivjw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qwoirykc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ntsbpiyp.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dwthqatk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fydvozzp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aiubsyec.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eadobgcf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrniuca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmyfrog.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3yjpxorgz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3teoaejkc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ycamuxvl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3rczlmnbl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qsatmhbj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3yuhgcifu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3afgtvabm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ogvnkqnq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sivgpkya.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yarsjuym.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tvabpphr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3qwwvgdfw.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3aosmhkxq.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3insblboz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zgiewrlm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lpejtpev.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3gczqszwl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wwzvwzqc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wftggwul.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qqilocau.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3icfxogkp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3abhbtmcx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tpyictxg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3qxlxkwlg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lxmbglfy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3afvazzbh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3nksbswcy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lpzpxrza.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wclytocq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3bspntmdk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zsmvewjf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3kixhhgug.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3psecqfsh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3wvihdtxn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3willsake.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3cejdyonr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3eiffrpcl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vabmyaox.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3lnpljcqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nlyetlno.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3otckmuoq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hodliwpe.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lypgwsph.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tncyjzgj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rfhugeve.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mqvjrixy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdhvuhg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3znphizlt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xswtnelr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uyryhyaz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axskdqwz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cqdeunma.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vgnzrjhd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ciedjteh.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mmzqryqc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qbcyuobi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lviuoyjj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ifeqsbje.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tmriqqyr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3stiecpkn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zefjoamr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcncolss.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xhilqecc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xlboojcj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3axwnjrzy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3qqmggfbo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bnmfapbb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bkekfdac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hqedfbpi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gkdyxjei.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wxnlxpvt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iergnayc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bpdmicdn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dcnqbgsg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3exstwqse.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3amboxkhf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3spyawhdn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dygdvrhl.html


<!-- 参考信息 -->