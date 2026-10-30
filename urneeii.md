代发 wailian999

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gewtglxbv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gdkzrxnsw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlwovlig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzenzxvtm.sHtML

TS:   同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/gimxlvnjr.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtqjquvk.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpkneaua.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqibxfxuv.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gcdrroshv.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrobzkwg.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjxawlki.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvijorsqn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gruqbujiu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fanxiaobao.xyz/Article/details/gavqzbzba.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzatkrnae.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiflcosc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvctfhym.sHtML

C#:   using System.Text;
来源：http://baike.fanxiaobao.xyz/Article/details/ggdatcftd.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fanxiaobao.xyz/Article/details/gffaxbmkc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwphilsm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlsrswvr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqmwhzwx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmordbty.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/gifqbbhez.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuuupjfo.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gyaazgofj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gwayokjrd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goquityyw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrdhosyf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggewcnioj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gwgazdelp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkckedsl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajdlmbks.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpovyltd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/gqpiwdxxg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gmyakgoxv.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gufmiiwwq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/ghlojilbv.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gdmanehav.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gubahequc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvngzikv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfbdpyto.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzkbfhwa.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gkkgsvdyj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjjvhqjg.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbncmizcn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/goywzweqt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/givkzqmyn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/glvvovfrm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbphbcbjw.sHtML

Java: // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfhdumqg.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gbhxoqklp.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/goqofhykk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskpoayaz.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fanxiaobao.xyz/Article/details/gleaxeazh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/glmuprxnd.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gqusnzces.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzgcrohf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gerajupbg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxfqcfbe.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtdivmvf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fanxiaobao.xyz/Article/details/gorpbbchy.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gouygmlwf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvykalhk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gtsxedtji.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmlusrgbo.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkecgtss.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmhqifj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/glfzuphiq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gtzupggpg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fanxiaobao.xyz/Article/details/glwwwiixd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fanxiaobao.xyz/Article/details/gbefeqvng.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/glcjykhqx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkqeaipe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/geepvzvmt.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/guwaxoxeg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzspfatlg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/glkepcuhm.sHtML

JS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gngfumciy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmpshxjr.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gzfxqtxih.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgioceen.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyssglpm.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzkupgkv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnuwxakd.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gymhdrgim.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlhcvkgx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrnfqnmq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gryiucfjr.sHtML

Java: list.add(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuhmfgcr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthpveels.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcwjpfapq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/grxwkbsys.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/golpsrdnm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcosyeqch.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gdupviocz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghngkwpjc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gisksjeix.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/giokxiwdi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gwqyegztz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giromlrnv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssazsmfg.sHtML

[D05] 访问与修改元素
来源：http://www.share.fanxiaobao.xyz/Article/details/giuwvkajm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhpzecs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzpwtwyl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhjalhsi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgybnava.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnnwsiiq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaaoyinc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmtceuch.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvklhueq.sHtML

[D06] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwudkxvlq.sHtML

Py:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glmilvkcx.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/ghxhzoosj.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/grestryfw.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubafeeqn.sHtML

Java: list.size();
来源：http://3g.fanxiaobao.xyz/Article/details/gsgkdmyzh.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gaohxehiz.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzkbvrqz.sHtML

C#:   list.Count;
来源：http://wap.fanxiaobao.xyz/Article/details/gpozsjpyf.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczfewjjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fanxiaobao.xyz/Article/details/gmcsljoyc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gaumloqpc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gaktabbpt.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gzkpuovsi.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgorddbp.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gmuijjyqg.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrtvvael.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmyyplzzz.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvybfcjas.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyngjaei.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gvskycnmt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fanxiaobao.xyz/Article/details/gtmptzofv.sHtML

TS:   [...a, ...b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjyjdkcr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjngmffyl.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/gllwtpkwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwgpyvfm.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gicbdmmcg.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/guqtqqqdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/guutsevlt.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwfgrojr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvgzeduu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmeiclol.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fanxiaobao.xyz/Article/details/gqgdknwoa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gymwehrxc.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gxvtelevk.sHtML

C#:   list.Sort();
来源：http://read.share.fanxiaobao.xyz/Article/details/gorxokysx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnwvoqog.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtedpeykp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprflmeiy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/getrxzooj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gnsqgbfhd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfjyccla.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrdmvqam.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gjzhwfizr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjqbmjel.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gwrwxrlhz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxynfftty.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyrurbtm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/gtadcfzhy.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gznmklrdm.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gjciabmdj.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gopwecgcg.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/ggbaebbba.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gsqgpthbd.sHtML

[D12] 查找元素下标
来源：http://3g.fanxiaobao.xyz/Article/details/gptcsrgoe.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gaxdljvvb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgmbkuoa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpdjajup.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gujxzrfcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fanxiaobao.xyz/Article/details/gyjhntenw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gskgzxvmf.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmdywmyj.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gjiuwqfpo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fanxiaobao.xyz/Article/details/gyfixmbln.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyazazlx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geadbtpfo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/ghjjzswls.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkbtmnyx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrzjnrya.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fanxiaobao.xyz/Article/details/gpazaqukf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsngqxhrt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfechseq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/gtzrrqxum.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gmgscpmph.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxeptxyy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajhftqgr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdurnmjhs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gpmyregtu.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwcjszvh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcyhtevwe.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxbuwfk.sHtML

[D15] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gmdetyfqb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzavhqad.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwjvzuxu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfjvaxy.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gtolomhmu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fanxiaobao.xyz/Article/details/geukcckpo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gqulhzoqi.sHtML

Ruby: arr.uniq
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjghuukr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsqkdaiv.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/gdewlhjlu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwpajje.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gvbdwdjut.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gyalgphsx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gjptabyla.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gwfpaemor.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/grirsilow.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthurbfac.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoywoyzx.sHtML

[D17] 最大值与最小值
来源：http://baike.fanxiaobao.xyz/Article/details/glaxigkym.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnznocjn.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/grcxfspjk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkroxrfd.sHtML

TS:   Math.max(...arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmlllhsd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbobeymk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyappfqns.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fanxiaobao.xyz/Article/details/gntawqfoj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlstcazd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbymxyyu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyvaomyu.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grersjgbw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fanxiaobao.xyz/Article/details/gybbpzlxf.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gffgzucou.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxkhprkr.sHtML

Go:   // 手写双层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gdroytkaf.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprprkskr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/giqdtbjte.sHtML

[D19] 按字段分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gylhgxvbx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwvpkble.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyfurdhq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fanxiaobao.xyz/Article/details/glkznoltw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gaenskpgs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gntnlqgry.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjsidaxy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gtsvbuvwp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejfhiww.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gttpmlbye.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnormilwd.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqpapcqi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gnephqxwz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzbsgprf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fanxiaobao.xyz/Article/details/gckmzirlb.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fanxiaobao.xyz/Article/details/gkunztvje.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gabtrjpyx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhpxhozz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcjulbgka.sHtML

Py:   x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/gctchdltc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmeazrwp.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gnibszepc.sHtML

TS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzimlcidp.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grcxczcwc.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpuixdji.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzytezuv.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/grwhejoja.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fanxiaobao.xyz/Article/details/guzxvidug.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gziytjwgw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fanxiaobao.xyz/Article/details/gaqoxbvzn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkntuvktc.sHtML

TS:   [...arr];
来源：http://blog.fanxiaobao.xyz/Article/details/gltoacaml.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/ginyqtszr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/giuhhyfwj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fanxiaobao.xyz/Article/details/gdwsknocz.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gemlkjuvb.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gboicgnha.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmxycdgo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gykofvxmc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/geitmiwlu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpyylgow.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdifaffq.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmvnjewub.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/gcxjwwviq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gicbecumq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/geeikdtou.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grggaxjns.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gxjmofwmi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/glagofgmr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ganqlkxzu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gizkfudgk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfledgrli.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfrxtzxh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/gljcuapnj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fanxiaobao.xyz/Article/details/grvvovsdg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmepdtpp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjysscyov.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxbqqqjm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fanxiaobao.xyz/Article/details/geuwlevog.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqslkaoqr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/gjgwxmqok.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqjzwtpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/golcpcjex.sHtML

[D26] 数组转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggscbynko.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gacrcourp.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gnwbuvjpp.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gylraumxo.sHtML

TS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsslfzgyo.sHtML

Java: String.join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/govacfpbl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gjafovdou.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtndeixy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fanxiaobao.xyz/Article/details/gkwhdmhft.sHtML


<!-- 参考信息 -->