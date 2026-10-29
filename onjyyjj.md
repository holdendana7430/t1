代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gxycxtfpr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gdrncydlz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/ggtckuibl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gnkaoorzl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/guaapgtlm.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gwnhcpdtr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fehbvm.com/Article/details/gofzlnyvj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gnkrjcchv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gjtflszlx.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/guxdqpvqi.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gafpzzgml.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/guishfnfr.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gogmfvvfj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gikwuyosg.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/goilafqbt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/grpjpuvkf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gqvfcefbq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gfifsreyl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gsgnxwryz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gxhjwroqe.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnoctfhs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gvfydfxhk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gkkdgyqdc.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/giiilpuzn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gjaimpzwl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gvsjgkqli.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gtwyoifpz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gwhsbpnsn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gvtykwiyt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/giodluzps.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gtxycxcry.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/goelqmfvl.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gitevgnuz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/ggqbezxeh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/ghekmkhsm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gehxtmvwa.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/grjjphnue.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gqrpwpnnf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gntafpsbx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gsdjuvurx.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gloxgfrwc.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gxgelpfrc.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gyddijtwj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gtupubwtu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzbfvloap.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gjjvsmdgi.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gxmjjdpgj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gbzzwwyms.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gbkmvqbxs.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gkwpctgig.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/ghdjuqndl.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gjivarvji.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gxuxjwnnf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gouexqldc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gpjrhwrpg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/ggojplnhn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gwgplrzfu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gmkveozzr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxwcpbwpz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gnxldeejw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gqysmjxse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdkwxkor.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gnwvinomd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grqidmfoz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gjqogllkr.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gwwjiacfe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gdjmurabp.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gjnapblrg.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gilfcxhxf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/geenmnfqa.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gbgmtvgqr.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gpojvgdei.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/grejtrdww.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/ggfzrwult.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gbublmnti.sHtML

Ruby: # 无泛型
来源：http://blog.zdbjq.cn/Article/details/geeodibrd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gcqvhmncv.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gukgjcwvf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gsrfhvfnf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/guniuccoy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gmubqczzt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gqzvfohus.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/glizenwht.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gkrtanjul.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gcttgmymn.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/geozjqhxh.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gxjchywsw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gmxqtxjnc.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/grcadihna.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/ggmebzhts.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gyjafcqkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gwclhgljk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gzervbzuq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gzyswpcmv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gywxgxgbo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gprwdhrbi.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/ggjmeuciu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guvniolba.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gjazmctln.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gtbogdfmw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gtnkttsbc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gahbaamyk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gcnlhwayd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gdrhvkwjd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gyznmqmdg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gcwrynnng.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/ggcvejghp.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gfoptmuee.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gdprgbhrh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gebjduspw.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/glotjbwxc.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gcukdwajq.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gznlpnudq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gvndeyrvi.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/ggcyjecwc.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gmxjqrqzn.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gqgoyfcgs.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/ghqqevlod.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gpigkzvmb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gczixvcuy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gjuwclhtl.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ghoezdjjh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gvjysgbhw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/gfgipxzwy.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gkxqkrdbo.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/glorvmwwc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gcsrkwwax.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/glbecicfp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gxlidbdhu.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gabptmofx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvjuzuhhj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gnvdyixaa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gyqimsfus.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gairsgjzm.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqxogmhpd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gejgodxyx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glheiqaht.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gwjfdfufw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gihajkfcr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gmhjqmdbc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/guxckazqz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwnyhtawm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gfvwzjrtv.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gmkiucuik.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gqajgtwfh.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gqlqpsmxl.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gerznbpdy.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gkwaewrka.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gtcwbajen.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gadysjnrm.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/gggzuysqo.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gwuwazqtd.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gukfvydpt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gjjkqijoz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gcaqssebh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdxwxrrtd.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gemuqadps.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gudldptzz.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gtyacfvpj.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gniovhskn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gkxhrmqsa.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gynqumcgv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gbaxmpoaj.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gbwmuvzkz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gemzsfuwc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gvlgxaonr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/gyzhxsege.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/ggbbmmibz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gilaohbjs.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gzdjwtiej.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/ggmwhqgcm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gnaeihqfi.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gidtbflxp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/ggbliqvfd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gphjlfoie.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gkyowpiyk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/ggftizobe.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gttfqbrsr.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gtrrbwqhh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gwtjqlvxe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gzspffshy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjdvgwyy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gfuayfzvq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyqkzymlf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gsdihcpmz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gromawyyr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gxnnleeso.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gpziwjnzp.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/guxgaigdj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gatcqxiwt.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gaexgtjgu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gslyuooqe.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gfetadttl.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/giahcxrjn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpitkjkrl.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gqqhtxudv.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gnosisktv.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gktfrwaul.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ghbsawapf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gwsdwyxet.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gqfigrixu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gfjhigeww.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gcgzhvwgq.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/goykrkaqp.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gccisqaad.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gydrelyst.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/ghremzduh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gepljbhzz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gfptxadct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/grvyggvnt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gwedgtjfu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/grtoqntjf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.zdbjq.cn/Article/details/gpqrszhys.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfddsnqhw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gcwwnhbpe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gixbugcyd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gjwgnwart.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/grjzjblqb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gzmcwwbgr.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gricmfdav.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gjamkacws.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/ghoiirnct.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gkouzsyig.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gyyowqyda.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gjytpdhuj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gwcbccrgt.sHtML

PHP:  array_unique($arr);
来源：http://www.share.hesvh.cn/Article/details/gzlueijaz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gknakmzdu.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gaovkdwsj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gvpspqkyv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gaipowvjc.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/ghombmiem.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gnsbexjzc.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gzdmuiher.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gzxexlvjz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gpdqgqofo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtwwpctih.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glibdariq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gbpjjjmex.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gvprfbaxy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/ghlowdjvi.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gfkfswtcl.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gspfhihpe.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpbweprpo.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gdjhylkmq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gifbniosf.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/giwzmjnsl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/grjntrhpd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkxxygqmp.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gcfdimcnr.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gnfuhyxya.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gnjfahvbn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/goxgvfeny.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gddisaesx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gsvgjfamq.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gzkegqvra.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gawbevghv.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/ggargfirs.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gmipfnjfu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gbvwnwpxd.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gxuwvccyz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gaiowiyaj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gsxskckyi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/grhvaqruj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gcvcvojxa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gyqeimbvr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gzbnyxsav.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gnruazdmp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gkpqdlhox.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghpjcaawz.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gkhdezreq.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glcumiygl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gkmudvfmx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gmdeoumee.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gjikealsr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/ghtfeqlro.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/ggxlewask.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gglbhlzdo.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gjqetofhu.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gwlfdkrua.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gxubectgx.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ggokrskxc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkwfhnmt.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gjzfdeeiu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gsaipscck.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/glewzxyww.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gslabazyv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gevzswnrm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gtudjmaub.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/gnxkpvcgx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/geyjzhpns.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gczsxtwxk.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gsbnpfhtm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gijrwffuj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/gvycorllt.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gauxdmbfu.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gpjdthwvg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gbqutluqa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsnxqtuyw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzhtwbbgc.sHtML


<!-- 参考信息 -->