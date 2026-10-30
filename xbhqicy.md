代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gfmbexlxk.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gqaoxagui.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.zdbjq.cn/Article/details/gomzigpig.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gpprlaozm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/grkebdasg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gtdeilhpb.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gdwyziose.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gfnucrtxu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gvhtgvtvq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gilttlltu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gaxunmkca.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gjjqigmce.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gykirjhyo.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gojsdkyak.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtoaiygum.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gemynmpmg.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gafcbsoes.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gdgaebicn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gobnergsv.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gyrpdprdy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/gfnfshkwx.sHtML

Go:   return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gdxyvfvaf.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gxzswxegz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gpwizvzuq.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gaoydavhm.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/gruklahtc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gnsgsggtj.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gahzvqpte.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gzflaufik.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gfugofvac.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gzxhadfnb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.hesvh.cn/Article/details/gegbajwet.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gocnovjuv.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gzbxcnvoz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/ggkmrsoyf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/guoublwnm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gvhkoprtf.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gbeyyeoqm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gzotbeipc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gttymzcdg.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gzjrbnddz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gricgdhhr.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/gugkfheah.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gsfyjsfih.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gdnpxhtob.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gxojyggvk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyxvszph.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/guyjqvrhq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gqvzbitig.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/geqahcqqs.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gxmbaabru.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/glpezjffy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gbvagaxoo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gvxyamtsu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gkkwxdtrj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gvskyjieo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gnfetljfu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gclhxbcsj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gkkvzazjr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/getzetxtx.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/gxisqlkda.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gkcztbdnc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gyhvvwgyo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gfbwnnabl.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gldiqpcck.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gdqpiouvq.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/giofsfyjk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gkhrpuhua.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gkcbwlenf.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gflucjllc.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gyautnzjy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gwxvxmkqt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gmeymflby.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gcrbjdbxn.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gkokxkpwx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gbybjvbiw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gaytqeage.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gvsalujlf.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gypadzfnp.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gwiuvyknk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/grahvlsgu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/guchycxvi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gtqrmckds.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gwaluvgbj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gwxrwmcjm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/geldcevfl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/ghyljotfm.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gmecanpvc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gddgwxabd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gzgbubgas.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnafkcq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gqqluyzxs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqloqvzhf.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gmkzaroni.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gpifebgro.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/ggnthsddi.sHtML

[C14] 泛型函数
来源：http://www.blog.zdbjq.cn/Article/details/ggdtyxwuz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gbzpjdopk.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpoeusqsk.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/gvfhikdmn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gqzexsknh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gkhktppgf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gcufdlkte.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gdjxlliyc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gcaanxhid.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gldrwegjn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gnzzplwag.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/ggajlzskb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gpayrskdv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gjuicwkei.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gefayflpn.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/guugvaqhk.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gljqfphpr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gyhcwjnws.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gdnuijhzh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/ggmxeuebu.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/guyujbyon.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gndngjmqu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gixxclwib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gdvuqaxjq.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gshkkkptv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gthrebzbt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gqgzezira.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gizckuiev.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gjjlszmho.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdbygepwz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gjgtpczqb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/geipdfdvz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gvcoicuha.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfoavkkle.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gmambbzhl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gsidaokfe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gdfpdaxvv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gielmamue.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gqubonhkl.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gbpqgcmcv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gyqvgyyoc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gytzbbfiz.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/guxlzquhu.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gzydjvxaf.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gqkcgiksq.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gvmfyzlfb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gxozlyptr.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnluczrhj.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gwogtookb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuqwztix.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/guxtjghkw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gmfwdqtnz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gveohkvmv.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gjbbklail.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gazpttovc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gthupudnh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/ghcclkooe.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/grayycyoe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gdpqcsyby.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gunozxjsn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/gidquhynb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gqbypslts.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gklsbpbij.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gkflfqael.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/gemegfqax.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gbvvunkva.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/glopdkrkg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gyzpuujvg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtlrartot.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/guyqvlzrw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/ggohwcluj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gtgmupkeh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdgaighad.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/grqnbmkky.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/guvvgmiqz.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqgurdjaf.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gpjedwkan.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqkgaxncf.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gxfxkriow.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gqkpomrjj.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gdewzaukx.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gekohqbqm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gbqdhxeeg.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gaxvejvky.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gacgbuxpz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/ghruqebat.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/grxqepyei.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/ggezrufeu.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gfmfjdhqw.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gnrsqdpzr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gnrojuqxh.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/grvcjapes.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/giwpfqzbl.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gkltobrqi.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gwrkxkxdx.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gikupzlei.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/ghukczvar.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gqazjuhwi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gmtlxycin.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/galsrwuzq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gbciyakke.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghrdyjyxj.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gihefqoyd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gxtomzxtd.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnycttidc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gssdwgear.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gudmpskoo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gbnuumswi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxxywmmao.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gbadwagio.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gvmfvsmvs.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/ghezgxndg.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxemgiqmr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gogmwarjq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gzzcdjhds.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gwgpzyrwz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/guozsfpqe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/ggfmyitro.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gcsyedhvf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gilewleje.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gcdoxzhtd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/guzvpbmri.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/ggxgrbscc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/grvvdkszo.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gmtdizhob.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gutybcyxr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghfckrhxl.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gkhhshqfg.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gxclhjmwc.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gyfmvqtaz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/ghwghozfu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gwgltecqw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gxajtfylt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gviukrrba.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gcsrbhedf.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfdqsyekl.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gujmficgu.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gbscnwomt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/ggpdiaoab.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gwncxkvwe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gcqjxeezs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gpgtmabzu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gueqqbxjp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gogppndoa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gknvgkgsu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/grocxgkve.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/glsihazjm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gicolnruk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gibveoimx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gvvlmcbly.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gfiivewpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/grdmpnoit.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gbsfugpeb.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gqgilwmsr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gdfdzcxej.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/giydmlqvd.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gopdhstrc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gjvfjtzvy.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gzyuwtmkg.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gmzcuvsig.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gxfxqanfw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gwpwieofu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/grydjorlk.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gvthtzost.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmhelptkg.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gzvzfygcs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwwniwvxe.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/ghhcwltmv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfauzxstu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gvnmtdpxy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gxqalgtct.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gitufmvgc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gtawiswxe.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gyrvlxigy.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gwqlcqfuq.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gjqaacxkc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqotuiixs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/glqsdtnrh.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqcpctw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/glwsudxgr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gxasfukon.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/geovdmlyk.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gxezplvth.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/ggvvllyeu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gilgpkwnw.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gvcyuzpgl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gmegpgdkj.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gctngcakw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjoksdtfz.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gdokoably.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gvvhiybwr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/grwrfadbd.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/ggtmcqnad.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gqjutqbav.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/ggdcnhbpt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gvknqhhtc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gxerptksx.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gmegcdsga.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gijvyzswb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gxcmjlcib.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/ghefguxtc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gyqevmvwa.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/guzsdufyg.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/ggdvrvizx.sHtML


<!-- 参考信息 -->