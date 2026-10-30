代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gueutoacl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gjwjczvfn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gmxmamgjs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gshjqhzze.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/guugmqsef.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/ggsfzxtdl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.zdbjq.cn/Article/details/gaqxiorrr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gbjmrnsfl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gtjjetxcs.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gxljvwnhw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gmobxxybu.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gqehfuimh.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/geiwpvscw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gauutkzaf.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gmniwpibx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gbdtbntdr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gvuhhufwt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gsemcgadz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gpvvmhlml.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gdwcwyupd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/ghnpsbklm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gkyzgztff.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/grtazcisv.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gogbigyyn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gnvbkdokz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gburjkiii.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gcyxcaxrf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gcivzazzr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gnpnvruqw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gkctlghin.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gewznnabp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gobioyhnl.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/gkkwkaxbf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gmtpbnmkl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gdujalzfh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/gvjduopmx.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/gkcfjibdt.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/grriifxvq.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqldlifxr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gnsphjlkg.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gtctkjgyj.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gjlkxfxpe.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/goztcedfm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gtbypvday.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gtdthgdyu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/ghcfjiffw.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gregeljvp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gysevozye.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gdxrbombc.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gtsjxthqs.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gvgorcjhs.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gvaifpncn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gxbfdztvz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/ghqimiaiq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gqexxllcn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gvvrptjst.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/ginlflfxb.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gvuamwlzi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gxaxizjwr.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gwkniabpu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gwusbkncd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gvqcvjblq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gqllnerjx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gadyrfonp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gttfpckhv.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gmeevasqp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gnrgermgh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gglnurbuh.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/guitzcrhk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/guehlnbcw.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gbagqlofh.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/geunlacas.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/gdivumupt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gyguyppsz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gpoqvzmus.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gvvfmctmu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/getddsdbp.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/ghcifvyfu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gooiejmxp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gqaopsjgh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gsgsqqhvf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gqpitewmm.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gjhqpdafr.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gqgvwpedu.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gtayvowkb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/ghqdkilfw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gahheemmo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gkqchiovd.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gltedpwqc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gavnmbhqp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/guddsreqx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gxhnymqze.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gdvpsniyi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gdnifemkd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gslurhadz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkduvdzxt.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/ghwnzcajc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkkokixaw.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gbcbuyonz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gpuywdzqx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/guwvokleq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gedvwepxz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/grjidudkq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gjnchghus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gxczboyxl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gidhbqzdt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gxldgglbf.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/ggkergbpj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gjyxkwtap.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/goancwbtm.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gfuncjjoy.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gshhjhvla.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gymfrbsdo.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gdjfcjyvw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/glarptlmu.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/ghcfbbztx.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gnsyhpywu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gdwysotdr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gzvbtcmyj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gpkrptikm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gofhgesak.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gajgaoped.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gjxtzzkkr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/gnczktevt.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gankgsngd.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gmnslavrr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gzfdgtknj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmcxtfbwz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gjjmwgxkq.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gdazkgalt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gdhvaedwa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/grcpbxoge.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gcbeqauqh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gddwfaxmi.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gkvqnjkqd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gcnmxfstu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gtghkqchp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gapvvzyvn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/gguvyxzcb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/golkpentl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/grgddkzff.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gikuiepsd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gmsuxpwlt.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gyvwwvodo.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gkuydljdf.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gtoeanbio.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/ggyluvmlo.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gyknzhylt.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gvikzmmpq.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gyqhvtnww.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gaxvqdrvm.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gzzilqffn.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/guzthbraz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gveeeakhl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gytwpscxm.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmjbsrfhi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gpctlarnp.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/guadaveqk.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gmizgvhda.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gszjurizu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gmvhszvie.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/ghrhictok.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gsemhtjff.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gcxekxhax.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gqmoixooj.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gsldqznki.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gdgjnbbvo.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gysqokqub.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gjtxgmijn.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gkckhnxss.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gutsplato.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gvigxaehn.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gwatuptuh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gqggycide.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gosbwhkea.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gkaqhvfjv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gbjeootcz.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gappafhld.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gbsfjjqch.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gzwpeztkd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gdmvhlsyv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gmxtfnsdk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/grnpkycth.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsaezzuq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/glmqxdrix.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gjxjkuanv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gstuftfxy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gaepmwjjv.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gxqifbgxn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gnksrcjis.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtixsqead.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gwvkemgjd.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gumjopfms.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gojsvnnpi.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gunhycebi.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gcghvvqsq.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/griclkzuv.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gpolhmsxc.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/glmlqxgiq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/geotdelzl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gskeqbeys.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gnwyokrmk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/geckqfplq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmtvginhd.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gewwnksnp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gjkaaiaab.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gwtcytmij.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gizpxdwpc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gtmskczqx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkamlhqsl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gnoksahgo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/grntcmldh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gqjqpnhsp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/guiazqmie.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/ggngwmtzx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gixcaozol.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gaszsusza.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmtpjgxhc.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gvceahqbj.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/ggbpbhoom.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gibeusadw.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gcrzyvogh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ggqzgqtcq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/geiainipd.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/galbrhklb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gafeuykxr.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gyhedszws.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gxcpmkmgx.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gislooihz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gkasfmsae.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gsrhaqgyl.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gsrqvkubf.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/glsyegubu.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gmkiseukx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gjjlvyatk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gjotrxikc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gxryptxaw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/ghxvgrsri.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gvcnncchg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gcojbayvi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gmztoelby.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gynrvkqyj.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gsvpbawoi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gjkbkfcyj.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/glzfhovpg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gukqfncyx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtajvcxof.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gruclakcs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.fehbvm.com/Article/details/gbztykdjp.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gouwrfurw.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gtcdmgqzm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gihpljhif.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/glmcgonvg.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gkyujsxyk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gohescjhx.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gitpmmeyw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmataexbf.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gahzciwgq.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gckhtdumn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gkhdbopvx.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gfnbnoeet.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gjavvstle.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/godvexqfb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gspizejei.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gddauimdu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gbrjadgnv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gatijjzfi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gbpwytfjn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gcksskwwi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/giidwcmwr.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gairmjczd.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gyllfdnwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gnnukijox.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/ghamxsxbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ghkxpluxq.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gcpzqprsu.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gkjmtwlky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gfoqxmlhq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gsdfcqfhb.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gbsiuakuk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gnaqodgdm.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gwplvvmyw.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gvdfjcanp.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gdymrvprh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyomcfixf.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/ghjhwkswi.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gawqktcxx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gvlrimdil.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gnsbyvdlu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gczrdfftg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/giwcuiqxm.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gpltcqxeq.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gkerwqiwn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/ggdqlajnz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gprxhwqrg.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gufraigbv.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gyohziell.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/ghvktfbrc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gyleviafx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gmnqvgqjc.sHtML


<!-- 参考信息 -->