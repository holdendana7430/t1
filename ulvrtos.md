代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxskiruno.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzqpcvxb.sHtML

[C08] 闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gihsnfhib.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxfeiquu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guxjwjzqr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdcajhbw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzmgbzls.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fanxiaobao.xyz/Article/details/gxvnqeoje.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvkuxyuob.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/ghyjycpxp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glaaainsz.sHtML

[C09] 递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gcognawaj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmcwpka.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbxfslgb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/grscpzmje.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoawvlqy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxebgxwwb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfkqpkyp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpwhzhil.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gpsyrtdnf.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaljnqzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrraamhe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fanxiaobao.xyz/Article/details/gdnhgpjch.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gygornxwy.sHtML

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gsebnkjxy.sHtML

Java: 方法内为块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gawhgthyz.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxzxkbx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwntseke.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsgjazrl.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/glmlkwwtd.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/giqhcxwiy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fanxiaobao.xyz/Article/details/gefypvgny.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/grnykrwqx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpuniutb.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtlnabk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvksxgyz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/ggxyhhlmm.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsurlhlwh.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gngssyjol.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/gclseatvu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gustfocmx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmeyougg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gvzrhwxll.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fanxiaobao.xyz/Article/details/govofrpjw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvhvrnee.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fanxiaobao.xyz/Article/details/ggrxkrrho.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glycnhzaq.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fanxiaobao.xyz/Article/details/gmfjhxfzr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwwuoiee.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/genabuvyj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugwevna.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gerlsawte.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdhgavml.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gdnbhlfwg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwujtntz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gnpfyuziz.sHtML

[C14] 泛型函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gftphojyl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbgvfaa.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/getkselhp.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtammcqb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkeuefwpe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/grmxkcbow.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fanxiaobao.xyz/Article/details/guschcgjz.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfbiywau.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbxytgah.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fanxiaobao.xyz/Article/details/gvcaaatyp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/gyvqhahiy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijyyxgd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gimgsbdbu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsjbqice.sHtML

Java: // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gaomyehht.sHtML

Go:   // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gqkcsyqzd.sHtML

Ruby: a, b = pair
来源：http://wap.fanxiaobao.xyz/Article/details/gszwirtha.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gpegppzvs.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gzzkhdxhd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/geaexsuvt.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gbglomqaw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbbyrpm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxgfxrbx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyivxzuxe.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fanxiaobao.xyz/Article/details/gkiwsusww.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/gqjvhomcg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkboudws.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdyignmne.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpqpurmm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscojoigy.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxiwwxbln.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gjovnmlqf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscbxkwqc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzqcetvg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fanxiaobao.xyz/Article/details/govhjkrwp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fanxiaobao.xyz/Article/details/gllxwawzo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gcxagycir.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gjbqrtfyb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyafptluc.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gggjibxbu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshrrzcnz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxfyxjea.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/ghlarlboq.sHtML

TS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvftmdow.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gtuskbnzj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjszgaoyy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gphigqnlx.sHtML

C#:   list.Add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnvmqggs.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqriaqjrf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/guktgcxor.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gcuharqfb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/giihzodyx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gdseqfzlh.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbugqwvx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/ghtgbwejh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/grpffvlhf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohnectjr.sHtML

[D04] 删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqyzowge.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbegfruh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gzdocseta.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gpboljafk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggafmotqe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztuxinpv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gzriqoveo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/geuosahud.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gntdeglpy.sHtML

[D05] 访问与修改元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjctasbe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/guqxnblmh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrzmjqrx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyliogsz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gephydkai.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmwrqyns.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gypmqryms.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwiywrmt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gtubdzayv.sHtML

[D06] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcakncdl.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gidofpdmq.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpjnlpii.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/ggirgihaj.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gteekrafo.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnawfqdax.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmxstbe.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/glfvigsnc.sHtML

C#:   list.Count;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcpbfqtq.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlohcftq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fanxiaobao.xyz/Article/details/ghyftbfzv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/golvblrxx.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxptxlx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbxpgqtxx.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbngdhld.sHtML

Go:   arr[1:4]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiolhobo.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gemedshks.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gcijickbr.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvkfwetc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gdmntrcjo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gskbhiywk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gcwzisbhs.sHtML

TS:   [...a, ...b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gggzjqptx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gzztolvsq.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceriabzu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfhxcykw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnckqcwri.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneymneql.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrkvxtda.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqafppakm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgznosxp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsyehfet.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeztewmy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyefcscl.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gelfsomcu.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeggpoob.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/grozxmhic.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjujjfzei.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gselqcsmf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/giawqyjvt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gvmqbsvdw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gxgjbhuau.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxofolsps.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvujaaagj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gynthmezp.sHtML

[D11] 反转数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gikmzivql.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fanxiaobao.xyz/Article/details/gugvgggkq.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gbvyimihg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwmzglzg.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexzziadg.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcnvwngc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzivqxtpe.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gwsubldte.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdecwkjp.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeushtzz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjlrglgt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gfrstismw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/givfwpnnc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnwbwtui.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqzmujqm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxdpkfux.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviqgeozx.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgepmlpv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzjmpqsm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/guhxkcjes.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumzkpwcj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxscknsk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdwaizjz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbdnzfkm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guajyupez.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gjttwnlvg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvlydlsr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpchffqa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbzdvonj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gnkodkqgg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gksiizbck.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyjqslhtd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtulwhbyo.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gmvtsgqfm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gcrcrifew.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gajiosxbc.sHtML

[D15] 去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpqhjwir.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gqvxorovk.sHtML

PHP:  array_unique($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gpkkerqzs.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fanxiaobao.xyz/Article/details/gkdjqxsbi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcawdmokp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fanxiaobao.xyz/Article/details/ghbmrllsh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpvcnadg.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/gnpodguvi.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyvqhvxv.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiaejymk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstfgdatc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbijipjjr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvzwabbb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuhtabco.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvshrupaz.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhiusjzx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/grikuxxvr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwerkfnpl.sHtML

[D17] 最大值与最小值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcuxykij.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwktnwzmc.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvlsgxwv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidtjzivr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmnljnsp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gxyoxwqdu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcuotvqu.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gcfarhkmk.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fanxiaobao.xyz/Article/details/gobiinelt.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gfjidnnjn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fanxiaobao.xyz/Article/details/gdqupinjx.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gutiosyjp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fanxiaobao.xyz/Article/details/glripxbpf.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gfffzjxue.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqaezwaf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkiuhwat.sHtML

Ruby: nested.flatten
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbmgsffb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdjswmav.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcovlfqz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbkcjecpe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fanxiaobao.xyz/Article/details/gfropanlb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwuqbxx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/ganykqwzq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fanxiaobao.xyz/Article/details/gtukzzgzo.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrvhrkbh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gekujeytr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/gayydohrh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkvkgpsu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glynasqtr.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnigegkgd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gexljjdsv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/grbwjuiae.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcimmifl.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gesrbhqro.sHtML

Ruby: arr.tally
来源：http://mobile.fanxiaobao.xyz/Article/details/gvngajyip.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsnlymxf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhvsrhcn.sHtML

Py:   x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/grgekeban.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gmzasqbgf.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkmmqvncc.sHtML

TS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzuykkix.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gzzkvyzvk.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkgykovkx.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxzkwzair.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/glknyjpdi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnwyizwv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyzwwisx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/gtsihokrx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaoejicc.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvttssck.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gyioahpcj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gudmlydqw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsaowwqs.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gewpgvooo.sHtML

[D23] reduce 累积计算
来源：http://m.share.fanxiaobao.xyz/Article/details/goafrqdgq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gnelpqwse.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggolxnhcu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gainkoqxk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwetkrot.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgyxlkaf.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gamjppesf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fanxiaobao.xyz/Article/details/gtdmpmhux.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fanxiaobao.xyz/Article/details/gbkyguhra.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gdlbccoqz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gsioweavj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gipwzjhyd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhcjnrqu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtxyavngf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/geylohadl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsboucgxa.sHtML


<!-- 参考信息 -->