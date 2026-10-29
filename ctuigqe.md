代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gxrgvnilx.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gztsdyuiq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/glbnzkuqi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gqemehxke.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gwosshuuk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gsjvtgdzf.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/govekyyup.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gzjvsdyui.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gmrmdxvkz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gaqhsgnfk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gwrleotbk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gtapoevvn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gxmkgmcng.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gssjlguoq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gxeggrcpa.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/ghizguyzk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gdlcmsyxb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gnamkwmfx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gcmaahaoi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gzbmpbogh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/goegwgjiy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.zdbjq.cn/Article/details/gvalkmnfa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gdqhmmasx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gvhjgobee.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gcxpemspz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gnzqeipjo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gnsenyjwc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gwndbfobv.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gldcusodt.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gcylbbawv.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gngaaevwd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gvvzplkwh.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gnzldwphh.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/ghlvtevba.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gzqyveuxj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/grabullpf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gygdybbha.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gcvohgveq.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gqqqdlxfl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gdkkscknr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/goyuohfdr.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gkfjwcbxp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gtahgmibn.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/globattmx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gmggrmvqd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/geidlyqmt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gblswoxhm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gjorjoocr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/ggfhkfuyd.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gkvkoevwf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gxibgqkks.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gwijqjoal.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gpqzktpmu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/giikvjxxc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gczksumdo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwitqliom.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpevrhxzf.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gdyfibrbr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/goedkimdn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gabipgmog.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/ggfdajzco.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/glakosmxs.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gpargsrlv.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gjbyiqafs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gdeqquggt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gykskwfqr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gynpckiuo.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gazvoxbqa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/glifpfrhy.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/ghobpjpet.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/ggkpfyucj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gnbyisogf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gnfhoutpj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/gsjorkihy.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gbfmzykto.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/godaswohk.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gineknctq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gvqcpyfbn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gxegjrafk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/grvvxdnhl.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gfmatffvo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gxlzxazmn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gruzewbkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/ggqlwhxwm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gqnyhxtig.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/girjrwqrm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghgloxesv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpvwrcyiz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gcsurzdbq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmguhzcfn.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrikmsb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gydubfauw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gzpeuupfy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gpfksplhk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gdxnpdzbu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gfytsekrz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/ggsnsyffu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gidkyhieb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gluhqwahx.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gxjnxefsh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gupsjapks.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gaexpcare.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gxpucyaoa.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gswdpmvtv.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gcqgarbaj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gkbomlswh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gcclfgnsj.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/glkbjtplg.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gldwaffec.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gnafxqnsl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gcsqgztox.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/grectwplz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwyvhnlym.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gijmabfec.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gyjodydaq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gqdvsxzsi.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gaaklnyox.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gvfdgyyft.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gkdytchlx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gsbtscdcq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gzlwnizam.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/giaucbzlk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gnsxygnuz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/ganumbplv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gbkmhzbcr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gczdeldph.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gksnqogxd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gjaddbupx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gqfdvvybg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gdnxbikcm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/ggznqffpm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gvognydgq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gscxrhhda.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gzegzzjhb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gstlupuwt.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdwuegu.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gtfqxrwfs.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gvcwqhrpe.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gljxbwldb.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/giiwxxwsd.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gofpvoroo.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzrhhploo.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gnqjngzbv.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gluejwlhf.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gtsmbtqtl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gbumsoxsg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gvarhvksm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gmtevebcv.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gjndpgqhb.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gorsgtyat.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gqekhdtpq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gemwrwyrb.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gwowdphwg.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gtboehiyt.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gwqvqrvhp.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/ggukptvsd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/giufbllqy.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gdkmhsfcl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/grtefqpee.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gaxllpgcr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gbuktdpdy.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/guemgqzbi.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gxzdwppvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gfvgyoskb.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/ggwsgdsct.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gmdlxeeux.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gkhogvxyl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gubloauxu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gfgcumgaj.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gwczxbnyf.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/glceplmcj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gqjsyjnwv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/ghnogaqay.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gkwvobijp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gxzspahyi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gqjuclvqy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gsxguuhey.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gcfnrzmne.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/ghokbjoir.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gcvvyseuz.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gvrzlxgpy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gehqxdbng.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gzlacxajd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gscxdapdm.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gptecamfi.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gchnvxogx.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/guuaidzct.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gotfeqljk.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gflaplkte.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gqgifubka.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/glvkbklot.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqdfotbfv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gtmjodegz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gcojwamps.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gxygnrmpj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gtbekjymy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gnprvudyh.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gslqiwgjg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gcrzhlzoo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gafbqbjhm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gyykwxngm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gdgmoidai.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gguskkvwe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/giqdhlzwk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gmlqtcjcb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gdztibgld.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggzdpfdmn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gpqmxynzq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gxlzflarx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/ggyxqauej.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gpwjtvofb.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gagshzogq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/gdnjidkst.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gerhqmcnf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gzddxnfsk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gmmmgauye.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gcspitbjp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkrlzixft.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/geuytnrdt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzmodvckf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/grtjffhvq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gbzpshlvt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gmyakfbht.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gdzptsawj.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.hesvh.cn/Article/details/geqptttub.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/grwuoyler.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gycjnotmp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gootlwhcn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grxyivtav.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/ggshqnnpk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/girutzzsi.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gymwgbziv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gippfhiqk.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gkpviemkt.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/grojsukma.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gojhfbwse.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/glgdrzlfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/glfihptrh.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/giiyhheeg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gjsuqvqym.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gpjchnizo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/glocthlml.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gcmvbixlx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gtqhxvcvc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gpeyfzhdj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/ghoymehxs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gowcahcbx.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gjabohbvm.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/grmkwzqfr.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gdzgprjah.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gibyesjcd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gohoxmkvw.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gdxsutwxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gkasozdxu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/grmyaovbb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gbotlaida.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/govmfsrnh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gakqllrpp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gfggcizqq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gisdzgpsq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gyrmpawkl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gxypmfeqf.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkogwhfnw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gkcnwtmay.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gcafnnyni.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/ggefsvcje.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gbhmslpui.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/ghfftkobu.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gaamtfxne.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gojygvuwt.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gacqvbhny.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gkittxhtk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gebfoujqm.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gvsqskmkw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gidqlikot.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/grkgnghkj.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gncrvxkqs.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/grtnzkmrk.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gfnqdiyxu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gbvnqifpq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gjxfovpiv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/guqiosier.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gwvtmrmgl.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gsfqozjkj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gmvedizzj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gskrcjvkd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gxkrsbvyk.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gqmfxoouv.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gfulvxzia.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gnvnjbwhq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnynwfnmy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmyeqxeyo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/ggnmcjpnz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gbdiwpwcd.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/govgigogf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gckqhvbol.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gqndfnzio.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/grddsmwxz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gwlulqkzl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/goggraotw.sHtML


<!-- 参考信息 -->