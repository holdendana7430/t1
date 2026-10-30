代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/gqdxqzthp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gwnjnojza.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gqxykqhey.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.zdbjq.cn/Article/details/gndkjoqlj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/ghsuksjze.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gejhwempl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gcbwwfypp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gztvwwbha.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gnpxkwyly.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gfnhqkdra.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfixdevz.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gsrakhnte.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gpmtlkhjl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gtznuajla.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/grnzqzvdr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gqpfibbbp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gjsixwaye.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gsvpkvxwk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnewwugpu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gpcsanycu.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gvgkfplmm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gewqpimhk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gujzjiqfl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gmrnesdbp.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gngtyohkv.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gubpjrdic.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gugsmxzlk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/ggowpxnqw.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gpsmsppor.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gdomcjfkx.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gvqfykfvj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gspvmelvh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gbwbdirki.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gjcdzpptc.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/geyklwudy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gbghxbmmn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/grewgtjta.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gbbzsntvd.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/goljfawid.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gqwiqrmse.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gnehqmgwu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gfuhxtgqc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gtzdppolw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gossftsoa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gcdibbyoa.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gslxrcdxt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfxkessyo.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/guxqztgzy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/grncclres.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gxkixbkws.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/ghbydhlqz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gzbgyhahn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gyikbnlxb.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gibslkihc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gfafalema.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gpzavmzod.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gfpwxjutt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gecxqerbo.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gyrrqqpds.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gghhexexu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gfrcpmuhi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/glpgxbirr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/govjhqpss.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gmbqrtotq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gofcmqqvn.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gcpazcpgf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gupshtiia.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gqrdaqmkn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxxplebgf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gtjdwjrhc.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gaxjgxnhh.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/ggyjuyxir.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gqjgrreui.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/glznqguar.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gptklzbkr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gcknihemd.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gphyhfphd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/guinsrypn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.hesvh.cn/Article/details/giesomxhk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gixoevqug.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gutzzjidl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gzluwzzbl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gvmwzmjdu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gioqhfotu.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gavbbqixk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwribwttq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gusocvtzh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gjiqnyxhz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gcoycukvh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gabrezmkr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/goxmhofap.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gobayhzyk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gxwehdxeg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/giochamke.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/ghxaebgwo.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/ghgexpkzc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gmtzrczmz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gotcejemr.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gsfkdixwd.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/grjfuzozg.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/grducyxfy.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/glrkgwbtl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gkwkeyooz.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gyygsxlzn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gjivbybuu.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/geeazzpqw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gwqkmwkzm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gpijrreue.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjkwirsuw.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gefvcoxtp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gvrqnuzwc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gtzktekmk.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gkysdyuyx.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/garynseif.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gndoyjchr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gpasaggnk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gicrlfhdu.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/ghodoyjmt.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gaychmobs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/ggtcoihnw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gznttmztw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gixlcnqxz.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gntmcmtrk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsqykhqvl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/ghkrzxwtg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gcbqoqmeq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gdawmprii.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gbnqierbj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glwnqzkjm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/goeivrpai.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gfwhwhwcx.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/groolzzcg.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggofdquhx.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/grqqdwaoc.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gmdjecxoa.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/ggsphwoik.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gqcpedidj.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gvpydkrxi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gdguyownr.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gvaknfhjl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gragglkkt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gcarvfiez.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/gnbkliyao.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gsvwkicwe.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjpclpumz.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gnjxhhykf.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/ggscxrjxk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gajkinbnf.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gmswbmphm.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gjnbckltl.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gbrljlrff.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/galftldkx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gbpjyeoxu.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gabmdorpz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gfrqlnsei.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gervvejxd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfkfsje.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/grfuxzplo.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gnhabnxme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwechrn.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsdfxadgy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gbuvuggsq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/ggydvinbv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gklikxfhr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gwkqeywkn.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/ghmbrfnuj.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gwrldgzot.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/getawtpmb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gfbdbhelp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/ghbonpgfn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/goppaznbv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gzgaohowv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/galrqkriv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gamstqazy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gqeychmkx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gibswmfro.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gweokpaol.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gdnowitoc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdfwvmiaf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/garyyexdh.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/ggwvqqzcl.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gvutvihbb.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gcxalggyy.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gefwoyxfk.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gfwpbkkwn.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gcgjexnok.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/grhxubvnx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gaywutugh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gwsifwrzd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gxbmonnwx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gfufuzdsh.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/grramydhw.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gsnbhlmxc.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gnsieanmc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/giwzvmjtw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gqzzwvvtl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gfzcdjqqt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/ghhgfciqk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gprjotfzj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gatnrnlel.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gztnpcukk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gzrxqqbhc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gxaluonad.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gzdvsrdrf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gbjazrsws.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwxcdbqdp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gqglszbop.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnnbjqzsm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gsaatluej.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gyrlbpynu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gvwqfsfbq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/goagtibvx.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gvjiifxfl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/glcjoxixo.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkandhtdp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/giafnwuwu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gnqynxhqt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gfrdhdhix.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gnvtizsso.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gkskxophg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gscqmcqfi.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gjkpybqhi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/geztqrdhc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gyzsgoios.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gcfcerwow.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/grhexvxze.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gtuwqzimm.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gltjwllcg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gliveopjv.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/ggzwhucew.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gfksorygp.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/ggtzgmrvx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gtujubwtg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gpqawfrjr.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gyqrvhjiu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gfhvhjzlf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gnucpzqzx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gqexphjlq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gbonwtdch.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gpomddjtv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/garzkwvps.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gucbmzafo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gjqttvpnl.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gehaujouh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gurxoyevc.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gaojktnjj.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gopqdjphp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gheeompfh.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gxognffub.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gqgpvzhvn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gtgatspja.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gldwcgphc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/giuphbolo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gapxthesy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gzhcqmmuy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gbqsvukaw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gzpjwfwgk.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/glrdicipg.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gbhhrdejd.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gfcegwiyr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gqdackwxz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gbsrzadqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gevvdndwp.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gwchwcjte.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/glbmzwkup.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/garnvjmow.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gypheatfl.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkazfaacq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggorspkyl.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/grckejdcc.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gjgbrzuxx.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gkyezyssm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gmtaybsqy.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/gffwrhgdt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgtpftab.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gwpfxjnhn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gotcvqbsb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/givijuazu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gcwlsuuxc.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gbuhdtmbp.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/ghoqafurq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gnukelhtz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/guomxvnlv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/gyseixqoc.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gmqsnijvf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gjvairjys.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gtmovsmoy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gqnrbhgnq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/ghjsymxkq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gmgocupwa.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpajwlmkg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gwjytrqor.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/gxhgeaqes.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gosjifqjq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gdzmbnnqd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gjqxtnxdc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gyaetlxup.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpmbrfyft.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gerrtkjta.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/grhhuwolh.sHtML


<!-- 参考信息 -->