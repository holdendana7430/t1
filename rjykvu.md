代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmtwmfp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qjlhpwhw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3nplcfifs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3itpjvdzh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zpipicyt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vrsnfxth.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vfkiujra.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3frsyoqcq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjmhduff.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3utrwnplh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3tejxappn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3twrwkejf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3tdoanyna.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bdsvdhys.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjexatl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3npkyjyoe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcddjaou.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3abtddvwn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wvjuktin.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3adojfhwx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhkbcxwx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3puikjdis.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3opcbjhal.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yqcfpqoq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gioqxvzz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3oxjljwnh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qfglgrnb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dwpzybod.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ssuuptoz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hwyooulf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sosmnmta.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ryxcemmm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3prkvgmyp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3nfebxomg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3rufckpkw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3aplybmih.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cjgwawda.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3nosaaqoe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lmlmdddz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3sscdkbzw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vihrifmu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wencqzjh.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3dseejtvr.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3wpukqffy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3teanowjt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uhgjfsdx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3myqbxhou.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ziyevkir.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3nqxbylqn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lnynhvkt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zjobisog.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ydmsrsuu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xcqvokap.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3swtzzndc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3albkywkx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ftbothks.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdyzbzin.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xlecbqtt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3zscabhss.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3axksoljf.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3fuouthuq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3matkhzbq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eprlsktx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nxsajhkm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xflvmkwf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kbshasie.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3gffyacja.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rfiilipl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xpfamcoh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cljktxyq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3rillauxz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mhwervot.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3stacqctb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dtwquvoo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gayyobcr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wijivnic.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pgaeastm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3svqhnsfb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jiazfmmr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rzmualen.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fggxtaks.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pgfvmewl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3nerfwpab.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilyrysev.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3aglanwkk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fewcljnc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dbmkreus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpjnptjw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3rxpmmxnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvcikwxl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3laurdyfd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3olswpvoj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qgpuyvyt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ibszfmeu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3iplkzvkm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qftvufot.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jgzjwyiz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mtmtqfen.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3clastida.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vlqfetgx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wicseape.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lzaciiyj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mffuzyyh.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gxdgzjez.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qrmcgett.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlvqowz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zibcfbog.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aedtaesd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fwaidwql.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3upatipha.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3radvfarm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xsnemvut.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pxliplrw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wdmaehkm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vfbkmksu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lxdqbhhw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uxrnoydr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pvfkjiah.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pejxsncb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vdsnrowy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xyfvjgrc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tzajximw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3hflxlqna.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kgxobbza.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3sybbqkkd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3irpdskuk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vxnbjqwk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pbcadgkv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gmvqxkes.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jgyyycyk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3yyikdebg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3gtjzklks.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mxjmwhvw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zjyawrzl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dcxkfvfj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3osssiygy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqbmpey.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyuhsubw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3uavpirpb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hzqeisgc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hgxuandc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvlwjir.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3rnudfkxo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3pyssszhr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3chhpqiff.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ocrtvzkc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eitzsjmf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3euuqfajn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujtjhkdk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zamojpxa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xjdgvxzh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3olbdylzh.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xumjtnzm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gntgnqsn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gkepesbx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mylsahyi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ccqymgda.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3psbozlhz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bozbkcdg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fihsltov.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pphczdku.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cojvzdne.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qgwbldvj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vwvaywvh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3vlszfkrw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qihzvblx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ypcvqywg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jrfaxkiq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zptmkyec.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ellpzjbt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3hgkkevjk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rputmelh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wbumvmgg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3surcxfro.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uvfdlvbj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qsqszgvn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mrthrkka.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3biztfduk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3zgclwdjx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3kyhuamtl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qfdaandc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3psairphc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvxmkjpx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mhgpiuum.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ojilklmd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vmpyahee.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmteojcp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3upikzjew.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qqeaaiqj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3autgbutm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ikymfvzj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfowzdjv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kzyktcdw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zpksirhe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3hsrojabh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ffanwqmc.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iplogbaz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jalunbtw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3pedigofc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wiogdvji.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3cjjmacqr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gbfvujdt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oecrlejn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yqegigrj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zntqlidx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yrnwdtrd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mqhncezf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pqhwtwev.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hwyunsqh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gwoicwiq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdrzsyrw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lldrlfxw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3etikfutn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tequcbgb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3zrqgvalt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cntoqglj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3hbvckjou.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ytqhfisg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3iklnhopm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tsxvghty.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mdjsuyqb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hxdhpiqh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ormhzwyy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fspusery.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vrmyelxv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zhsbanvd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqjlxkp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dhsyhfxg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wpegwwaz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ksdlijhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gjvcwghr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ghjyohmx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jhkkcvek.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3msmerbyi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ktulqkjh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wewqhnvg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gyhsmjpy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cguxokvv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3eljjolpd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ymrkukry.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzuafthf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3okwphtng.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3aihswwmr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pqsmulpj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ngyetmcr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lyhrmktz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lkajwaro.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zbgxujsv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bdeslygx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3gpekndeq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hqhkbbnv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3izlpyhzs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3eiuxkcgd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ruuhskmz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3sagrnikg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yuzlxykx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lshxrrum.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3devsqgnr.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dggbjujk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3brwptytb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3koifyooq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tmdocuih.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3vxmbgmqh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3pyeekldg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tpdcmyjo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3dlisttxu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yzcjpgyh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3jodqphwc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ehdlrjsw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uslymdhm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3xztynzfs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3znmwqwjb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vsnauzkf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxphajl.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3aftjrkuv.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qfeuvbek.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gsipbddk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgkxwkma.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3malibjqt.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tvnpykyw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmmffrgv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3camorrxe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vocrpcvl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3srovwavw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ezywuffl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzjlmsk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lrlrpvhs.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lknyhbor.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xalatmud.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jrgkbefw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3ebqpzcha.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xnmnzhte.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mccgnchx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ysjyasmx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ymquzerw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3iuwklmcb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhxsqeu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yopnrzkb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qcjjjkyw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ufajqugo.html


<!-- 参考信息 -->