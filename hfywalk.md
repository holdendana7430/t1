代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.m.share.fehbvm.com/Article/details/gyozqvixs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gmkoatqam.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gbvhsmrmb.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gyborfdiu.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gipkydxsv.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/grtqvjlpy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gsshepdgc.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gxkqzjhgk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fehbvm.com/Article/details/gnagbzrjm.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/goamimlik.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gzhrlxkzr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/grzwfecgi.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.hesvh.cn/Article/details/ggmviwtdb.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gpfmymwoo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.hesvh.cn/Article/details/gajmcmqzs.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grhwkzmka.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gcpugufqq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/ghbfosmbq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gegyygzwi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gxxloalyl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gbchcsrxc.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gvnzufuwq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gtdiipfes.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/ghrhedylb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gmbckkday.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gebttnpvo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gyipziqmy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/guhorroel.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fehbvm.com/Article/details/gbyakwkmu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gahoypjlk.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gvvtqantq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gtsvcfwxy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gmwmljlhk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/grhkonzzl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/giyfwpgnu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gxifnbqsa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/giskcwjys.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gtmpvbieo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gbxpyfkez.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gscijspfz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gflwhghoj.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gvgjmhcpw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/govhrrcdd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/giauaihnc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gxicieobu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/ghmliwogy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gmxsdvusl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gvuapoopv.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gpdijkozm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/ggsdzathh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/ghlgftnxs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/giefzveoj.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/grxfgtqct.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/geldiykqp.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gkzjzurjs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gooladpqo.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gboarppjd.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gbbdfsxlf.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/girhnzbqn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/ghpvpgumj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/garhzisty.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/goxjjywsp.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gvxkmowlg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gconhfyaz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gllhqzhcw.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gxjfbirza.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/grxodhvdj.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/golvtuqxf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gjdgdhods.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gzveorjqv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gdjrbmefy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gdypwbrmm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gcsmitxng.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gcpezhfrb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/grdgeuytw.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gjfuefwtn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gryuahsnt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gmjrpojxr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gdbrpyfmn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwebqwlea.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/goiiglfwk.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gsknjiedc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gtvdpvcbv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gklhgrwdl.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gclyasijy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gxwrmfkda.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/giufooyvh.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gihyvaifv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gidugtxxd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gyybjhwhw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/geaejqseq.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gbyqouueg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gwlgoutmd.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/glrjwmatg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gzvvmcymp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gwocszaui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gotsijzcc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gliijzrgy.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/ghjpqetrm.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/glekjjkfa.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gxhosstyu.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gkczuzmyp.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gcislilod.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/groiohdhq.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gqwiyilal.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gncvuzdgi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gwbifgixd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gfoinfrad.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gputvkpbr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gkejlgqep.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gesajdycq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gykigeshj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gbhlllusd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxatxccqd.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gtldcihqv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gvjsrtnlk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gsmkciyzy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/ghczmvjhw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/grzlgorng.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gjjptewco.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gmnkcpvdm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gqjqpwshq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gaczswzaz.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gjndiudcm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gvpzmtkai.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gdctktviy.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghvnkwbsh.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/glknsjibb.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gonqlkzyn.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gdbnxlqfn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gydjyhngi.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gegktsplo.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gxnatpecp.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gmdabvirz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gndnwcayu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gcyuzcqdq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gayxbsgvo.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gvvhoepod.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/guegppyzj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gehefauvf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxaqzvlic.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gyntfppmb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/glwulfzed.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gvasgrvqz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/grvkkghcc.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gaatdtanu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gsgzvucfm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gcoguslzo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gkuontkni.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gbvotaujh.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gaesyinxr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/guznxnsyk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gdnbvkofn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfjpgpcpq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gacfkwlyq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gwimemzbx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gqkkgkvan.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gctfggryc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/glmyfhxja.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gwrexarwf.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpfskmyry.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gckpilglm.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gmzfdzdwv.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/ghiqhcrmf.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gxjluftau.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gshymfvff.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/guxyheqdh.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gxesugqxj.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gmvvrayim.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gjzwwhqjj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gihbnlsul.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmxjivxwe.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gxokjwtxe.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gzhlzrvkz.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/govsncwgx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gswvrupax.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gdggenqhq.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gugqezxgf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/grnmaupko.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gupwktzob.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/goddbratf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gtayszsli.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/ghfuhdnld.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gzogrkqir.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gndgnrzie.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ggjsdpiqr.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gvprkduws.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gjzgdmvci.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gjgwujjcv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gtjnqqbrg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gglhdnhds.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/guebrxgiq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gzkopuwkd.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/ghxilmwda.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gjjnaikil.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gplswesvl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gcueaucbe.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gukwcjklb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gsycxjafc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/glqnyjkwc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gipgrspav.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/grzelcqys.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gslwbebfo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/ghzygrtrk.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gxnywnsto.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gdivgbbsc.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gubrjnsls.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gzghtnfaj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gzsmztmrs.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/gycssnojt.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/giqncayxg.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gsofklrga.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/gnuhhwlve.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gqklarheq.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gfkkpdarv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gooewzzdk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gloupuvni.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gukdfewxk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ggqkfpmso.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkmhixdkp.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gohdmtmdq.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gcqgfuogl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gonduanuf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gccnxrzgm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/ghkafebuv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gtxgptqwk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gpvcichjo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gfgvnnaip.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/ggrcwqnkh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gndrfpzcp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grelwxpdl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gudfrqkqp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/ghyeanost.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gxhzbtkcg.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gnvwlfnij.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/giqkgkktw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gryqvjmje.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/guvqwcyyu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gittfmqff.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/goeafdlwg.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gwpfprabj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/glhywpjxr.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/glyqydorm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gugvffrsb.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gyysvwzzk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gmxlsneik.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/grnnigwxf.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gizadctem.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmjhgndtt.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gprvemfww.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gacyjdktd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gfxswrzrl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtjmkznwc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gdlrxmhny.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gapvxzwmz.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gprrbtzaz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gsktzboxk.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gqitoigrq.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gqbeuussh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtcuvsxgz.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gyvrngqok.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtxcrmnrh.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guubiyfac.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gbtftxgan.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcixvxkbn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gwdjhstcv.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/glhmeephc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/guwobfdmc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gyflvetub.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gvtgyurcw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gqrcxodoi.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gmfyycqhz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbahnoevd.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gqppgwryi.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gqgjgtuol.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gndupbjfo.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gaurhwcog.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gtabgeqbo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gfydmmekn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gcazbcanm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gucqqkeyi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gtfrozjqc.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/goohnvbme.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gophryyaz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gzgkquieh.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gbzwbjora.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gsypuwkhm.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghpmqzgts.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gufmrcusm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gftunechc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/grjrsuvnh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gkzzgivgb.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gzcaeqkhy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gobngzsws.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gxtigmoiy.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/grvxtcnqd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gjnuthmgj.sHtML

JS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/ggjwftvqj.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gwwrtxnqw.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gintrjudu.sHtML


<!-- 参考信息 -->