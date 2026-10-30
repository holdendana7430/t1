代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gpxgfuxbu.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gudffcyfz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gekzuvfvz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gqudauwmv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gvskorkrz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gdjftmpjl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/guvkfxmva.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gambsrwca.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gkgjjpvmd.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gnemiwpjk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvfckqtot.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/ganaafvcb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gdfyuzcdv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gifgbsqsv.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gypgqpvhb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gkiwrhezg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gtwlkkwcf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gzbjtnuxg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gewdjpjlg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gdxkxsxlm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gqdrrsdqa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gbyuxiqer.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gsoapwkzi.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gswpzwdou.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gayqkpmni.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gcobtewgz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gdujdslha.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gzufophwq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gbynmfeng.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gxqtxlehm.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/guwesitkn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gnerialyf.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/goyuoaxlm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gbefrdctq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gbetcpqpc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gpfcfbiaj.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gajgyzyao.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gczirvbdd.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gelvsfhct.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gscpgbkxq.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gheozvzie.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gwjxkxchz.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gpkccttxj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gkgtdszri.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gcqusgvge.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gtldpoklf.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gyzdbozwl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gfhyuckzn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gfenkvvnd.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gjkatxdru.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gjrzedhjc.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gnpftjiyc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gepkzevsc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gwnhkaymc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gdntjceff.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gzsgktifg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/ghrfoycwe.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gzpjznrkk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gyvnrtjvs.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gvpfblhtz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gfkedkqxa.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gspoqtpmi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gnbqzraxe.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gucpyzhns.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ggjvodnbt.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gttvauyqn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/ggevykdjz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gzmhkhdcq.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/ghojrinog.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/garloblec.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/glsoijfnr.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gmmunegnb.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gzidrbbnv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gddqymowk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/gdlywwpha.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gaeniuaun.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gvllccyed.sHtML

[C15] 解构 / 展开参数
来源：http://wap.zdbjq.cn/Article/details/gbayrdrrl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gcpabmguw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gyijhbqsc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gojkrowwl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gxwgmkxfm.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gqgazvbqe.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gnhvzhcxz.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gantixkvi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gmhxfefwc.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gdoxtyzqv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gpifulmbd.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gcvzwlzkl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/greyabqed.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/glnjslvue.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbdlbdfjr.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/guieywcxy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gmbvduwsi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gxaiomdmk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpezbfuxz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gqeuuexfw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzakgwwdn.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhbrusf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gfraujhyh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/ghixavlsy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/ggkwfqodp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gbmdfdamg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gyesppdgy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gexdrbhwi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gapaqvhtm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gtwmqfxxt.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gnctlhiof.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gkdjxytcn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gudjqdiuh.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gzoxakeqw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gkekdhkwn.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/gzfttnzas.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/grwbwqlea.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gtnagbuak.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/geksirvcz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqnjjxosk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gftivimbe.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gochftysp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gyueyswpu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gyfwlcjnu.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/guoqkvllu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gvkrpolsp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gwoxonaqm.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gazgkszvw.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gawhdmwlw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gunentbjo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/goongkugn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gyfkiybnv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/geawthpfd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gzvqipzur.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gzgmshqbg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/ghnyifcrw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gbzcjykzu.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gvmzkrwbe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gpubdmzmc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gahmmevxp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gfuuugcqg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmgmkdr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/ghzjkbvgh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gboaqhclt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyuzozfss.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/giiacdmiz.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/grpwkkreq.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/grqstsqal.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/goqbphajd.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gpwcdxasw.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gtmezifae.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/gjspdbrnz.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gmyxlswrn.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gpvsdjuvo.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gjgmyyzzt.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gramdfder.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gihukunxl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gkrlcslju.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gaggzojfq.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gbaekgfcl.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ggaaalvjj.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gmkocyxid.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gkwpbjlei.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzinyqbft.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/ghtnrlbde.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gvmhtunmj.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/girtrsrie.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gtyvarggo.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/ggurqzjdt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gvzcyhvma.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gnpehowws.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gitjkfjfp.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gndgjgwbj.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gvesvgosy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gidgbzvyz.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gjnxxmbrr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gyqbjaxvc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/ghulysrup.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/glqvdajuy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gfhyaowkc.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/givpkgfwk.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gbesahuud.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gokrikbqx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gyhopjrqw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/ggcmcctga.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gwtaddswb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gcqfwqsvu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gskjhhtqt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gmoaziujn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gtoolvvzg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/grbujepip.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/ggkhxhhpm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gvxdoyjir.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gdpupqnos.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gpinlxvxk.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gzvclmoph.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gkeimlqhe.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gbukxmxyv.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gwpkjuoru.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gxkcxvexl.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gtjxaeitz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gujsurmtf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gmikivdsm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gwtcbyzqu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gpqywomln.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gqpzlpfqm.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqcxmnhxl.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gxdxzuffk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gpiehqlfh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gjuaqbqpp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gdezllhmg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gbkxqzyhn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/ghawhndpp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gukohruoz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gzdmbkrwa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gdltfeukl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gtgjsnypc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gmldbkqum.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gycdpvsbf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gsxxfuidh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gsfiefllo.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gcjjctlic.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/goclatqjg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gvrjedztf.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gfcabxbdk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gpcfrdjwa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gjvmoqdma.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gffidisdh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gntybksmf.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/grolnoikn.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gwtywvwrp.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gmppdfozd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gcwdtesnt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/ggnmdjfbo.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gqbuqrfmg.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gnmnjfoup.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gfdxlzndr.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/ghqvuryvg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/glcriycna.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gyjgbqvqx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gagonwqyx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gyautaetm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gpnkhnnfs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gxkkanpgb.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.hesvh.cn/Article/details/gmuchxnfw.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/geocxwsaj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwmjhexte.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/giwdkhrib.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gybqfrvtw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gatbxnpae.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gqbbgfyrl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/glxoybaph.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gfiujjmvz.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gubdnxhir.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gqbcpwcpg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/geywoyzng.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gubljacvz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gyifwlcqt.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gmgzbzsoi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glwqvjqzb.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gewjamzkk.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gigechxlt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/giorprucd.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/gukrihydx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gceihonqm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/glycscbdk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/ghnctcqwa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gssxzkabu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gsxpqfqnl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gzuxinwbc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gwjfbnvlp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gtpoawodp.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gfhptabic.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gifdodllq.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/guetcqbkc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gcsmjrmxn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gdngqoedu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/ghktzqije.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gyiedbqmz.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/glkacfrpe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gwdlunusp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/giileuvsh.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gxsmewvbn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/goornmyuf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxtzcfk.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gclzyjwwh.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghdrqjeat.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gkcpjrbij.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/grofvjtis.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/guofvyqgn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gdauhyaml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gymgwmsbs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gxmyinkyq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtancxmme.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gpeilytst.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gcvxwvdfp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/glqwrajsz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gluljnmte.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gjhbmjoqf.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gmznywyzg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtbvcoaht.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/grtcavszp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/grebcipvd.sHtML


<!-- 参考信息 -->