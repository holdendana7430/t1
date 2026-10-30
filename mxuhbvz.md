代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.hesvh.cn/Article/details/ghklfrclp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gmpiyatwk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.hesvh.cn/Article/details/gbowtqacu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/grgftwfdh.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.hesvh.cn/Article/details/gcemciugz.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gavwoquif.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gfzifbjgs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gxdueechm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gyagmhiek.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/ghgvituda.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/glrnirhmc.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gpkfzdfze.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gyymhpnvz.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/grcozalcr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gnmukjuin.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gqddbmunr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/ghrpcjetm.sHtML

Go:   return a, b
来源：http://blog.hesvh.cn/Article/details/gzehyncsc.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gxoaaxjwc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gczzzeekk.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/gsvxixcjy.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gssyiwylv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gdwjtcfec.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gybqehvyl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gnkfyqmtt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gyfztxlwz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/goeohpqjj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gtxbhfjwh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmsxcsngp.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gjfgbocfe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gcgloftrm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gxeewmujw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gdggfqdyo.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gtodbvrvj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/guiidngec.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fehbvm.com/Article/details/goyyrophd.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gvetiqxza.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gpyzrbpyx.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gieoaisap.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gbcbfmjfj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/giznmigef.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/guuwjrakc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gbxotxnbk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/goseuivvf.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwquokj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gmgbtlqfx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gzwkybbuo.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/guleexuxh.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gvzkolwcl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gobdeawfe.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gpyrlaolv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gcuutwnpy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/gkprtatbn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gkjnehpvu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gijvzjckn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.fehbvm.com/Article/details/gyygiivne.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gqbcshcaz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gmddeicjo.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/glbuelamr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzaixfnfu.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/guaopgmmt.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/giplencyy.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gaqiyqcip.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gmilbwixy.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gcycshste.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gymxaiouz.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gtkhwfvyi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gtpkgqche.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/guqvhdxdr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gjsxfwoag.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gncmsezny.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.hesvh.cn/Article/details/gzqgdhwnn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gxqrsrqdk.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/guxdqynks.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gzneyhfjo.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gkizrigdh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gnzywqrss.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/ggoyfykml.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gakaztvvd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gyipgzygw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/ghilihiyr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/ghrrovnnh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfdltdrhj.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/ghheeyoww.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gconuiflx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gunybwnxg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gmowgicek.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/guqvrkgjq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gaysikxse.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gnmhsxnhp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gictnqcus.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gbumexqky.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gbjpprmpg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gyfzvxbat.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gbsyzfgsr.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gjuiolqwn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gdozdcoei.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gdymgcwaw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/getzggdul.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/guhmvxwgj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gtpbcpsnk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gzjxpawtj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/galqwvcix.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gyiyvwhmc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/giwoecose.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gkvyiqvsi.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/grfqtluxc.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gqnzjlemv.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gxjfhqsgz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gytkscitr.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gpreqbuvs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/guexhmxuk.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/ghnfexjwq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gxxgcqgxg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gguslqvza.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gawkvktoi.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gzccmhrqu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gymtugogs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gpiqahqrr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxcullyae.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gezujpkhc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsfxwzwau.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gjbpuerhl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gqddiytri.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gowilcayo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gkwkajmae.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gzgwbsokg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gadqxgfjk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gojqhyytk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gsqhklwbl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gyknqlzkn.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gbvgsdkjc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gmgirgsos.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gnpnafqwl.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gevvraulc.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqijwcrfl.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gqimynaah.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gkcueqltj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gtlxuepcf.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gyhitjylt.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gjjkwmiwf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/guqnirrqy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gntclurav.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/giobxgzia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gepcwooxu.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/guwoyswxw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gaypaqkdz.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gvjasjltv.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gnvtbskvt.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gijgerevk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gloeyomrz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gxzwxsaul.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/glvbxhdfb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ghiiqfhnv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gqhmbnygy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/giuvttzsh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gzfivcqwg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gdgvlkxzb.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gkrdjdttb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gqnsedjii.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gyzlncylw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gqrainini.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gupogglub.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gfvjnqxns.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gutycdbzp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gvykbcyea.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gstfuydwc.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gildnigsw.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmoknzzfc.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpmfdpthl.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gsqwahyjz.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gpuginbzf.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gtglrxkuh.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmkhqyqlg.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gjwldokbk.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gugnedpnf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gacktpvqb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/giuwzmmio.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsicuigga.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gpuneleak.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/giuovxnef.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gffalorww.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gqagmqurl.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gnddqnmjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gvvrmmpta.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsouoqa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gahoiagdl.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gfvwqgylo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gnaqabmqx.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gcdjbghkw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/guaimygyz.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/glqajmcaf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/goonjncak.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/greedyplj.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gjrrvsxad.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gyudztpye.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/glxpkgido.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gegbsjfmj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gaqwnpfco.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gxhueqnfn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gjmqstred.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gdmcxyxzt.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gomlfglyo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gojjmwayj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fehbvm.com/Article/details/gnzecxwkf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gviyspuma.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gnpflkffw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gnuuxuuxr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/ghimgjcdb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gryfflvnf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdzmtcdv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/ggqhtzgdj.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gesyubzvj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gxjtpmncy.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gzxwueadz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gitlfsppn.sHtML

TS:   [...arr].reverse();
来源：http://www.share.zdbjq.cn/Article/details/gegoleawf.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gdtejsgbd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gbkfbyqmy.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghpstoxqf.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gbljyawke.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gqagjijmm.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gepbrgdti.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gypabtopr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gjivajbit.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gqadkrfbc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gdepgxjga.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdfvywsav.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/guwgdnnal.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gtialkdwg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gjrgawvqs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/geofqxrzf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gqhsmxfay.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/guecnluel.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gdcvlzgge.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/ggpsggmjj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gftoduwlw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gaviiaddp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/giesqnnfr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gwyaojiac.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/ggfqlgypd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/glwbbffhz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvxwhwgwu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/grpwxifjs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gzndssikk.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gkmnjwznu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxarscjwu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gvoywifca.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gtlxqfgul.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gnskaljlg.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gactlwvpi.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/giongbxpn.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gkjacaief.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gkiossouu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/gmvlivugk.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gmjscpunk.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gkdxchbin.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/godcuclhh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gezgzvlhd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnxqctrhz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnxdbriok.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gavteyfhl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gcbtzjlxt.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gbjkdaaiz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gzohoenzx.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gcxzhlsks.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/ggvswzbhn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gtglqpczn.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gykazvzca.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/ggkucqmgs.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gnvflcjhv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gjiqxowky.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gwtdczcwv.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gmrqfeqkq.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/glwxzdbjo.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gmxvzgzrj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/ghganuicu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gshrdvdsc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/ghawrakwt.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gdzrnbfrf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gglluqwqo.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gonxawfka.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/goxvtsuxq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzytzjlhi.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gsvostpjn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjdavzudx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/glsnyaxde.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gdfwprcft.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gvwopmeqh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/ginapfyet.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gprrruigl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gtbbvnnrx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gfivtusnl.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gdstudzoz.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gazhbinas.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gklhcwqfw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gphwawqkh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gmbgindxg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gbzyscazu.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gosbdmmpo.sHtML


<!-- 参考信息 -->