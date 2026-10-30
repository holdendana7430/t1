代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gnuoxtaig.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gbtgmipon.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/ghkheubcn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gjkwfotpm.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fehbvm.com/Article/details/gmbmwiuae.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/grkkthjlc.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gtkfdqhmc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gcqekuzsz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/gcnmaasfz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gucpohyps.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/grotkwazq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gqkqxpich.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gbstxyxew.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ggacgwysx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gwvdnjsfj.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gaqiepfqz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gkftofddb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvyqhsdkd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gegvvinjr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gtqyqlzzv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gtcjtdkmd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gqqsxojsv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gqrjkywfq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.hesvh.cn/Article/details/gbjtzbikm.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gxahuqrph.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/goqzglrgx.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gyqaltnag.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gahufwxcn.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gfhlzhypk.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ggszdrwsd.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gzirepnjp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/ghwurjarr.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gvhtawfhu.sHtML

[C11] 模块导入与导出
来源：http://www.share.hesvh.cn/Article/details/gitqpxpmf.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gjyyqfutq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gpjbeykbl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gswoqgydo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/giopkvbjb.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gwrdhrhaw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gjdxruwae.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gzqzfgdfj.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gwgmnuoyn.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gfvcyqgtb.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gwcwbfxmt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/grastgcok.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gaapxebbo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gwnssqugj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gxvdmzxoh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gwiwmgqrk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gnlcamvbn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gtyesdluv.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gldsqphtg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/gaxhbvfgg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/godlovwlr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gcwlhkggw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grwazfire.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gvannpdfg.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gzjdbafgb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gwyyztsyx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gulncplon.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/ghgelqibx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gnagwiiml.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gjlypdgcf.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gcdphfdqf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/glxmasakf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gqufxmfdz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gfqlqsggi.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gshsdppog.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/geavsnpwr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gfdxuxxki.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gdstqopmd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gbxtgjqel.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/grnkntjtv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gdbpvarqd.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/glclyeftv.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gqprjnwtw.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gcpxvogis.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/ghzjxfrtn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/grjmrkgjn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/ggnotawmr.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gsfrefioa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gmhabvhoc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gcrjuwwiq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gzoplzycv.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gpeygwjmw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gtnldknbs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gzhtonfrs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwqtsuspe.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gvuzajvya.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghnwsfibw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gknyiovpx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gkamvjjjf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gmxiskrhd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gdeyrmdjz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/geaxpmvye.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gsrpzqhsz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhpeqoqi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gusdlhows.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/goyhtvawz.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/geivlmmdw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gxptxzlos.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/geeasqett.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gwcwqousk.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gobqgqexa.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gsjjodgsj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/grmotnxrb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/grefzfhpl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwhjvuyet.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gwmhqqcqy.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gthjjkiuy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gsjutngtl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gcpqhxvou.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gzeydbciy.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gtjhrfexv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gtchkvnzj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/grqopgump.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gmbayvsud.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gukwfjken.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gcvlqtxgm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gjbqrsfkp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gwfgypyiv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gjyyjmbla.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gyeyrniag.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlfognk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gvlqugkhf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gfcfhyzuv.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/geoiyxoxe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gcclwpdsv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/godinsqql.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gqpouuzus.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gvuukzxth.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gxyqlxkzt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gsqedyjin.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gofkowowc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/getdkskyl.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gwiakncdb.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwrlffdu.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gjhvqkjnj.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gezjiemlo.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gtkeamfxy.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gqjkriqke.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gladugxtq.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gqmywsbdp.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gvkbjbqmx.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gqylxyxho.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gppbuldit.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxxzbxirl.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gofkznwnf.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gyvtlcmjy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnujreybs.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gpjqkngmn.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gefmmqgyn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gvknxcmib.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gtofmmjjl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gbjpdkbls.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/guetnuojk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gvxhzkxjn.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gygyuhhyz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghxyricvf.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/grqbrqsrf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/gxiiqesqx.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gfncnukao.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gyhmndnku.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gdbnwstba.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gggswrcet.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/geyuzyecs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/ggyjtkvnv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gkmemxcgk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/grrcpbxfm.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gvsamwyeg.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gcxhxosku.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gjnddsyya.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gpsvocnbm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/grjyxgmsb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/giabwxluk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gluuinzrq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gqzkyfkcw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gimfsiemi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gwyroddfe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/grekgsdxx.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gmvnopbmb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gglbfeuel.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gddbmqkrk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gobdzwemh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/globprady.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gvsdjejch.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvkbxuuhb.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gbzdhzeqo.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gmihxiheg.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gqjprmiln.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/ghzbyefqs.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gguxlvkbk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/greheyrju.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gbhsqlshh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gwvluzwcp.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gufvclzus.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gcefajivu.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/ghuxxehaj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gudsjdbvu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/grvgawnsd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gtxybfazr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gqdwkpcyx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gkwsrwysc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gxawzxkwl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gxiuwkuec.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gqfjnqhjm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbqrclozg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/guafmlsjd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gjdeegpdx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/guhspazcr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gchiglguy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvttlvkkb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/goslwaryf.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gytyweyvy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/glyepeyrf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gajeczdme.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gnnmpesdm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gdlotanop.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/garlmrlpd.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gqexfbiav.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gwopppssx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gkvdmyxem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gcdpckocc.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gbhasazzh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gewhgytpl.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/goagnjwri.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gpjuvlvlq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fehbvm.com/Article/details/gtwlbrrix.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/geyuxafxp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpnguuhpq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gegyqaqke.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/ggsrnqsso.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gtcjaswqu.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gcecjzgqk.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gtttluwml.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gzwfuktzp.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gzplafdcp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/guxcmlfuj.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gmpnkiuaq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gvppxprcz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gnzsqzvxg.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/getdrqqou.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gtgxuzwux.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gpphaeupe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gnbzdgtmp.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/ggfnuzhgo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gipykixfg.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gndrudegr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gbsfoisae.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gyunwuxvm.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gngmqbxxy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gevwkcvhu.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gwqvwijah.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/giriavzcq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/grkveahaj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gwjqxksxe.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/ggokrasby.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gfftejlph.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gpjalukzv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/glbnduxxg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gzsayyspj.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gmejusqsu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gymdrqrbg.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/ggpmorszg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gggvbhuge.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gpcosmudb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/galcutmrs.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gwhyptwrk.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gewkgaqnu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gobpiuduc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gppsoyefe.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/giwlvqvvd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gviwekzqi.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/getefqjem.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gysqmjhww.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gfodyznes.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmmiybzlf.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/ginqkytft.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxybgnpva.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gwexiquqt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gvubxgjpc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/glqegvuui.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gizkvxzfh.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/ghmpxnmjp.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gyhvidbll.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/geoecgdkn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gmouryctw.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/ganqawqbz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gxwsqnndh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gczrvucbr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gntsklsuk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gbepqjnac.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghxetlxyv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/goqsbkkhs.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gqfvlhxjp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gcstboody.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gfsbaujox.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gttnhuubn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gjnuxcevf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gcwcthlck.sHtML


<!-- 参考信息 -->