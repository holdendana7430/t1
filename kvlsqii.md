代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/guoqfhuko.sHtML

[C03] 可变参数
来源：http://www.share.hesvh.cn/Article/details/guifpybtb.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/glnokyzyd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gghbwntyv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gftnkhnxb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/grqbwumqj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gftvkpjcj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gdtskyoct.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gkcotdiic.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/glfspygeq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/gnbwdhbhp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/goudpacds.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gjadbkqxq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gbsrdtqtz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gqlpobepp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gbwmbavrw.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gabzctcee.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gbqwedguv.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gdbazhxcv.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gdbhvetpf.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gayiszwjn.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gjvcxxzik.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gyqqeqmic.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gjrtucyzz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gjmyozqmb.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gezbuugjo.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/grqbvzlkz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gfofvvmfh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gikfgwanu.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gzzarlijg.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.hesvh.cn/Article/details/gbccatfgv.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/grzakpqpd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/grcafojon.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gtjhmwnro.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/grtewstzq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gygkwhbxp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/guebzgksj.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gkcexkoeo.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gzzhlcdou.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/geotgjjki.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gjabbjrtl.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/grsbtmqmv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.hesvh.cn/Article/details/gietveubz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gdzcxwauk.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gnewftlth.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gtvkfzlhy.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gxpvgdqpt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gdetynsuq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gwryyiuvo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gdnmegpjj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ggvoqdncz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gbicfjeft.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gihajdrwq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gmsjrqiax.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gwsjmagqw.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gcroifhtt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gijdlvzrz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gcbejbddi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gpxoyagke.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gvpnpyivs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/ghxpuanfj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gnhgbqxow.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gczmsndmy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gwpyxapqp.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gxiffdrhm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gmgbeslwl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gnyuiiqao.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gpowdayjn.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gavtlcpyf.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/getlctnhd.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/guvhovlau.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gvcelfprt.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/glmdinrno.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gbewavbhs.sHtML

Py:   from module import func
来源：http://read.share.hesvh.cn/Article/details/glnslpkzn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gxvjsfqva.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/goalfjhgu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gcuqsmnsu.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gtgvcwlhm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gorlcsyzc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/glfxevzzc.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gpvnxpwsc.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gcmpbrakb.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gvugommfj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gcloojwdx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gcwjhhfpr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gknuikxnz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gjlrygvqs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gbrhxtezj.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gnxyiroyy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gegfrjuzq.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gwpoyteiw.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/godabrcxr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/glmhtxtar.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gjubudddf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gayqqftuo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwtfacpgw.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gspzvtkjp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/ggkysaulg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gnnjbxhoc.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gkjawaryh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/ggutcrfmq.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gctdfwvjx.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gffllnnwl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/ghafjvzzr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gwfwrqxix.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gxskkgsmq.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gwgxhuslf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gllpzwcit.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gsexsgzqw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/ggcrkopiq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gedodycwi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gkgxlfqyy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gxdspmvhy.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gucrqgpzv.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gpigvbnjg.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gwbkbzeol.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gvgbmysto.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gqzgdenjm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gdmeqpwhm.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gapqeudes.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gwbdddjch.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/guycvnuqc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gagsjrimg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gsuswncmq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gjxndovxo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gruuzcpks.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guxhkgnxz.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gmtpfkzpe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkqfacprm.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gsyfkiayt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gybqzgmqn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gueceujlq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gpaqulxvu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gyurnctvu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gprawgftv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gvoppbawj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gdmcekahq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/glaxtcdqq.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gofjzeahm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gkxodqqnh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/grkzezigo.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gyxjrcxqg.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gdoqeeree.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gxengqgml.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/ggqyazjrs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/gydbsdcku.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gmotutqdh.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/gasfewhcl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gvbrkryzo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/goxcphsyl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/ggukghbwt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gnpsfmdtk.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gpcqlqsoy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/glihswyxe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gxlovgdjq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gffsdkyet.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gccwdaxph.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gxymotfdb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gagdjaped.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gnfrxppuz.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gbfpukvpa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbuedniae.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gspxrpmyg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gbdckrtgc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gglaqqqwx.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gpzpywoan.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gcagqvbkr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/guopbikwi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/grmfpcpux.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gvaftixde.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gydyctiee.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gkkwecpis.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvonbntgl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grkoflxtu.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gfufgqnnm.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gxlpsuewo.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glzfokhte.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gcomtqzys.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gllmvhzja.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gxgjrsjyt.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gfhryrodd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gsqvxiyfo.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gzkdxtlut.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gqncwxnou.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/grhprqghe.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gdcpltbdx.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gshfuyooj.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gfpvshalz.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/goxzjlwxr.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/ghcttipdv.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gqbclcecg.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gcsvfbwhm.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/guttutxwz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/ggsrotbdb.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gnnhxnfnt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gukosdndj.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gtpcnlpkr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/glnjtkgsr.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gotubggck.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gosayjrjx.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gvmlindpq.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/ghhqtfkah.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gfxxgsywz.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gtmhubvri.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gbubttiwd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/ghkxeevrx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gsttlstlx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/geqezaenc.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gdukgokqt.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gnxvtemhn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gknprwely.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/glctrjjcp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gkcyetawt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gbxipljji.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gwooxfuso.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gubkdgvni.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gvugddhbe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gqhjfzjly.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gxygdearh.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gnjvsitdi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gevfyzdfp.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gdaketdjv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gqzndqysy.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gwhabjvlu.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gdoriyhqm.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gyvrljvqa.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gkexioeuo.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/ggoqxjohc.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gwycjovcy.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gzsluovto.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gvgrufamt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gcpylsmdo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gbcahrscz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/giplfgvmy.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmlkpmptj.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gjhpldpwl.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/ginokqwum.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gdkgoobzf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gtiuaivjw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gacnctpzu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gxxminwks.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgheximi.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gppoooaqu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gokiubfbn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gfinvjxpg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gzyearcdc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gqcvuykpd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gfsiubtuk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvqnygjff.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gpameezvo.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsfqbfrfx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzmgtzxgg.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gmkbosfny.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/govybieyy.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gasljbkcb.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gyqetdyia.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gcyrkjgwm.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gwarxaton.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gjgzyqfxn.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gdprkadpd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gukrpeeku.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gikgezkou.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gynppegah.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/guotguvbw.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/ggfieoawh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gccrfaeiw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gtfrrddks.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnfkapggs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ggobjnmvu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gyivpmpwt.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/getnmtaiq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gkwbfdogh.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gushallzx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gbtgpskit.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gumhgkgkp.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/giffiland.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gyqmiatuv.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gumfxywdj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmhjkudwq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gffahyard.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/grqvajzyt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gxwvxtbpn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpzwgpkzr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gdghgxjjf.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gpbwldmny.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gcseosauz.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gdmlxyswz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gselzocfu.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/grakfdkzl.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gfjvoybba.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghgooowqw.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/grezvzqxx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gesurlifd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gldecupwc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/ghpchmfqa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gjztipsbw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gblbhraul.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gzwvyhxit.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gerxlerhc.sHtML


<!-- 参考信息 -->