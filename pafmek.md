代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qtniojgt.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3aqckvcnk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dqocwdir.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nixrfeyy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3jargwcww.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vqabpnlz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tmljudmz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ocdqmtsz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3asgyicys.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3optjzlpb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gpvsdsef.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kvbvqwox.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jixuqzln.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdcywzpm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pobpofbj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3cdadlusb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3oewctohc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zvhliilg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jzyegzgd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jotljbam.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ujbpztnc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3dirikjcz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wemcgkeo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dwmxtkfp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jxiepzcd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hjtcngui.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jctlmneu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tzujvqxh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ekugkcyy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tbaqwfma.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3tbltdfgo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xdhfbajr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jarhxaqx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qhjegvwx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3euyuqyim.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gbpecnxv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mgckegat.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mdgkezlx.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ixkyaplz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3jkoedyqu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3suctsvja.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lswqfhbr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3sfihdedc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zsywyvhd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wcsefsxe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3dccdwafs.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ekwditog.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nnnexjlk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3tdrwejce.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3kppjdzka.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rjfqrnsd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qiihwumb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xlwnzuav.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tzyqwjyp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bdmjnacc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3awblgoxg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bherbznf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mbiaorwf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bqrzoauy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rspcnwav.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbztwfmz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3fxajhato.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sbenfaaz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bezfeocl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3gyloanco.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3loruwohp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ycejbzwv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rxjkshvo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhfmnzzd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cpwgusor.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gbstzshf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nzvwqvgr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dfdxtppb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mkyhctzw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mcbekxcn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ldzorglr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wifavhwi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcjddxzc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ngkqgqmz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3nwypnily.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3kctekico.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bafrkxjv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3akcjygvf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kroptcxe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3znyulobx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3psdihhro.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bvdxwyzp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skfjoqbe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pkxvtxer.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3umpdxdmo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3facriuvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euvnlpxj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cyyypkam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbosqmdn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ihhgsjgk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3iqgodhra.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ajzbrkfl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dohusynt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3slzyliph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cjkpiogf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ljicvedp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bkumvrim.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3giddukgc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3pgsagpyb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pzypanxm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3icnqqcht.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tctrgsru.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ayotchyw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3fbmwruvg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ldycwoog.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3pigatfre.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rxgwqpgw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ymtodcvb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lilujsdq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bbhoamaz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3waynhuzc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jcplxkio.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tnqauztp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gxbtmroe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3vkfyabfw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3imnaljfd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3blsyknhm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kwfswpvt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3tczrfdot.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ngsxgktt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kfcvvjxf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vbosaatb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cosfnxer.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vkpmbnbb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jqkmqbqd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jousfzrc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ytaqvdrp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dsgklkmp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3panklnwp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cqozxnso.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3pxcszfhj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zfnncbnc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dcbeasdw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kqzwggyx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mtbgpyce.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dkauwkiv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxremgjq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3yfosshxg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wmkualbh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ibydhnlm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iemmeuaq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xlbvshyk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3plwalefl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wmcidbjj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3utmhhihl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yvelwiih.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mkkgnqau.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pgvjkvbi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cuekcngk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hovppapa.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ufylklup.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jyimjtfi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zaoxnpbv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nwnvceth.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xttezafj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3snrzixej.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3eszlgrmz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3zlmsjdft.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gwckkaxi.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3clxgwybe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ujwqjxim.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ysdklnfn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3uayavicn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zdsayhzf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3uderxgfy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oyojslow.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dgvalzyd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3uoifnlkt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jrwhkdco.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3osnmnfpa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ucjsycyj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gfducfup.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3unvvwyjb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sdmzhsyz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3duvkhadf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yzjvmpvc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mqegseaa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3pukwhagr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xvtahgea.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3tneznkrp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3oosmnzhe.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njdajojx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nzvtvpxc.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3bloflwks.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yxhfbwoo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzfhntfw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mkuubpet.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3iodnnvir.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3aoapcmfv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dqbolenq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rcinmqha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ginobemv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ownzjwey.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xpsdyrdk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eqaelllm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wkqxaprb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3euxvwlop.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rjtgvyej.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ykindyii.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3lolymnsk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3curscncm.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dumnzidq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ufbzwqmy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ddsjncew.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlgjfzr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3slznshqq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fxidbdqo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tsvrxhut.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sdmawmup.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iucrffqo.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pejtwgtb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rvtdzvqe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3btgtowos.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3akhwtqvh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3shwaxqek.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3dzsudrek.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tzswhbse.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3awbksgsj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lfzrqvdg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ffjymrby.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3axgbrjjf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3zvixljxy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hzhmdmyc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbkakyfq.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ahsobxcs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bnhmnlfq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vgpbiaon.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3smfyapms.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fzsfblxh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bhepdjui.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3jhymkpuf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3jrdpxvjg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wonlzirr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3akuomoig.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dgmuruvd.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3repoacah.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tquaosjp.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzjouzun.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uerdwptr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hfglfxwp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dbketdkv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fvdffmfb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nqnxikea.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ihwhjiqq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jortpahu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hjdwhifo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3abtnxngq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3enprestg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3eznsgeft.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nnqwblxt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fvazldeo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3juzvpwge.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ocwsbgaf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qhjxryfi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nmjyghji.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lcaxwlpw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3yorpbfsv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3sftqsklq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gwdgsqbk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bhzbnedu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ozrjyqzw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3lrtjzmik.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scmuccfw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mkdsomnx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3punrvfkn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cnqhkdlt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3gyhoasxz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3czrqgkyv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qwtqozil.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rfhjrtoj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dvraorzj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3xqroqkkc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svhalsao.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zdrluulz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iwlszkzj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3klgksibj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vyrhxkwy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3aerfwxvx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zmttshpj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jofessnh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3dwycfico.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqwcqnuy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vsvsgkmn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3dypjdbyc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3tztrhltr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3pjkhdsuv.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qgihsqpq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3eojuneyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fahevswu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3lanhhpou.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wosonuzx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zmuoqipj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3qxqvwzbu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3crcytfzx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3pxyfjmbt.html


<!-- 参考信息 -->