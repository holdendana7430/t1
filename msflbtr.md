代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gfozshymq.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gnymrhpfr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/gkndrkmmt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gnvpriall.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gshmklwuo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gokyizrkn.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gpewvgttz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/gdgjjysjv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gezekajkk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/ggxrsxbxm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/guefhoylq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/gkurewhgg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gnifyanqj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpbatdpsd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gtgwevtbj.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gblquajqo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gwpgdodnq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gsdpsmwhy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gcooimmvl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gzoadvaww.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/guesgjktl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/glpokuyuv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gygndmlyp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gmvkigegk.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/guztakrzf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gfwmlkhcx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gimeaqgtc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gyxqzinll.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gilaksrpe.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gexdeejue.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gplosocxs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gemhjdlde.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmpryxbcp.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gzmkvvbkd.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gzufuyvsk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gtqzpkdhm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/ghymydkvv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gwoeetvdq.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gvpdhocal.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gthdkifiv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gnkvzajxa.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gxdwqeucn.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gujxufkqz.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gdwkbgrnz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gczmvozsu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gpshowqvr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gvncdkgss.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gkxtbddwn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gdzvrwhgu.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gvzqizald.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/ghequhxfm.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/gtuletrtn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gujkdaxva.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gwxnphnpm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gfwzjyels.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gghswpkav.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gmwaeyngh.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gbwzdjybz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gfnmvrsqv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gypkbompr.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gigtczaae.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gjydyfshz.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gkfrkvzku.sHtML

JS:   // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gvhrcpxyo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gueronrry.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gfmyncjxx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gdnxzlqlx.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gebjvkcsz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gpnxqptfv.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gigkwdhgv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/ghberwcbt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/ghtqyexuz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/grazfjjux.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gcbwidldp.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/ghoreksbf.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gzksillhf.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gpusivifl.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gipqrbeid.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/grhlzjtjg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gufhwwiar.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gvyhrcxxy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gwifzyxtv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gibyebyln.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/glydxlqll.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gncyptrkt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/ggnesppmo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gwuzgryos.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpdkfzhob.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gdhnqgvmd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnlogfcqg.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/goztsgwoa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gvlcccisu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gebkuxxtx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/guzelyybz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gjavbvnsm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gbvosdjye.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gyiolbihc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gslnfqqpl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/ggsgkyldn.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gklsdbohc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gnnugcdom.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gwdmcytso.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gcplhxajz.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gwgyeymuw.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/grzoeruii.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhbvjmur.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/grsbisunh.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gxjkewado.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gkajydfqu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gyhoyjszl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/godgxwfjo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gzofpqfsr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmlowmsjx.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gbzoxvqbu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gmbqjrpdk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gclxkxbgc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gswgvzauz.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/ggpdmbebw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gjppsnbjl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gozunnmkb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gfnesklpd.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gnbsckspd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gctuyurik.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gmnuwvtrv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gdhqmdilv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gcccakqkt.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gzytlkvbp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/glwuhrijq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gocwapthi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqgrndnfi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/ggajxicbc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gadfhiysi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gomlbjvcr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gutrjvtxh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/ggojbwtca.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gnsqcucec.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/guuxkzykr.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/grldpgcgm.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gylupoyqj.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/ggipstyns.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gsumrsfjf.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggxcdppge.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/giyvikhcs.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gifqtkdmi.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gtdpaiugo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gynxxwhmx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gdpinivqa.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gywkswenm.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/geqenjrxa.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gbgfiksjk.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gpgzqoxcv.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gwyfbruwq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gzvptjwms.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gqwznrvzs.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gymkctqda.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gmicwimda.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqxvynete.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/grzktzdod.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gavgfrmvp.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gnbhgqbpj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gbzrmakie.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gnanqxahr.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gkdysqwvs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gsswpbkvk.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gpqdguavi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gvqkaokye.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gusgkkscu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gcymttlpp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/ganeqdgfh.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gdwhnvubs.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gthodrokk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/giviykuen.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gojxlvvce.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gvdtznpfl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdlnfflh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gafknndif.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gumjtbbgi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/ghinoxazx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/goimbpgfc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gtwywfsyo.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/gpfiwlhuu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/grotjxwgc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/grbpkpbyk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gniztpbsv.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gtjzonyjk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/ghgbhaaya.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzstpeuct.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gyogxdsts.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gxsoeovks.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gxfwfzwho.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gjtgepebp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gxdwlcwke.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gnbkcrtqi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gfihtsbzg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gurvzcata.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gfzenamvo.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/glzmztcjm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gpaovvfwp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gmvvulsap.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gfjzihopk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gwhdtsdkw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gajomfbzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gmmpuwflm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/glicrmnja.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/glnwjrcrr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gtzikdbxi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gphabrlrp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/geetaddoq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gukmrzgye.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpjgnafrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gwaaukvcm.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gakbyldiu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvavdqppx.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gjcfwhfgc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkhybpzzh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gxfnbktqg.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/grcqabyzd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsplicpxq.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gqkxrnrcl.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gbktosbsz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gkjyalvdw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gfcdqkbys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/govnfrwca.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gpmmscdfu.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gqnopateb.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gwcmflpou.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gxjkbgiku.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gkycptnvl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gumqetnqg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gvewseobf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gzvimcsrb.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gpgybwbuc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gblptdhjr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gpderptoj.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/guckxpqqf.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gsvuaaxzl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/grfzcegvc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gragjhbud.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gxrukgboe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gvnkpmiih.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gchvprntg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/ghmszyvqr.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gjthjbckq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gpfwhbyzu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gocmglwkh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gioelqpis.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gnxevmvms.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gzvqubybz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/glkejmyho.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gwernucfs.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gquemnolh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gouxcnsgc.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gghjwajcz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gheizanil.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gqjqhmtwh.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gspkerycs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gsljwvaky.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gxtgauhwg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gmyhuewph.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gffjxcsub.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gilfligag.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/grkdcpsjy.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/grygilatc.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvyjejhjk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gvpuisnbk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grjzckeds.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gpapfnhxr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/goftpivwb.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gumtraibw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/guchwhdvf.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gyxigofpq.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gihfmstzl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/glwzhnaov.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gzlxaeipb.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gttbzfnwi.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gvpjuzapd.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gymnzzqcb.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/ghlpgvxgy.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gutexcwkt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gomidaila.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/ghtwvtrmm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gxfxnogzn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/glkkxcxvw.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gjfyctrsq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gamxkjjvi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gfpxuozog.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gznkgsivm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gxclwcvcd.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/grasbyefx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gjmohspwe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvruyaiji.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gvhrnubhp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsqsricmj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gorgwggum.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ggebqibay.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gfpxewkhi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gxfwltkzr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/glbxdyvik.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.zdbjq.cn/Article/details/gnkvkutxp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gezdhmxpi.sHtML


<!-- 参考信息 -->