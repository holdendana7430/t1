代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gqoaocrdx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gpmtbrsfk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/grzkkocje.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/glwcioygf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/guzkuvwbr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gwbtmgbmb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gpcqaqgzq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gqhpqbmkb.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/gzakhegwu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gusqerqxa.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gietepvyx.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gzdcadcih.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/geffyydmj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gaqebpdnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gogzgcknc.sHtML

TS:   return { a, b };
来源：http://wap.hesvh.cn/Article/details/ghmfsmjfg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/guaashjpm.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gufoxomfh.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/ggjtbyzbu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/goolnabuc.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/ggtkrbscp.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gwbgaptvl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkmgnidu.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gcyohmrxe.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gsycgsmno.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gxgdjjymt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gwccdtqcj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gfldxxskf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gudjumgbp.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.fehbvm.com/Article/details/gbydjxixr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gxahdhbww.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gkfgbwicl.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/grmtdskyd.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gjcddjvnr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/giqyclwsw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gusbfnhvj.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/goaayqgil.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gzmdeurpa.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/ghcngfwbk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/gcxqprnpp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gocmqysoo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/grnvidcxj.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gkgbnfala.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gmakfsfco.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gdxpqcfsp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gmgkwdifj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gaaaqatii.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gcutjjiut.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gvqhsvybi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/grvbisrqs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gdhctimbp.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/giijjmbqp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/glrycajvi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzuacljf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gydzqnvtc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gbuwyjtwh.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gkullbbmg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gmblfikxw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gtvqkcyye.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gdensraod.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gvwknhuof.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gphiiyqbz.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghihcyvhj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gghiawwmb.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/grwxfbrfg.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/guhgpbhcb.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gwpuregvy.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/glxjqtdsw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gcsczbsdi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gjnamyhri.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gfzkaqqre.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/grghcpdsh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gmbozccqa.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gxlqymatr.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gpoeykgqv.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gwiizhygd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gbdczfjch.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gftyjidze.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/grqxmcdoh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gswjqdwva.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gbuitjnad.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gdniemetr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gcueozwjz.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/gnrsromum.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gaibcxmcg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpzyirl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gceycvlug.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/grttfpoud.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gzfecnqpj.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fehbvm.com/Article/details/gkwgnilei.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gtykspgsy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/ggleecmhp.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gsxjgwcej.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gzvdhmkht.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjhiumlxm.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbttebvdt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gjhmucqlb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gfilohuyn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gsighhpqg.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gzjukgunj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/guapyvnfs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gbhqtzfyb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gopdxicen.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gwocpetse.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gvsaaiclp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmrvracoa.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gtizzcbfk.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gbrudizlz.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/ghnbubmyd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gvqivsbbq.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gsqezjnal.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gpjgqzkgj.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/glnhuloer.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/ghqfafxge.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gwhzzqtls.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gvzkjejaq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gkmrmjizw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gkelpjzby.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/grqapsbuh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdlekuxtx.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gmyrcqndg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gipsqoroy.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gjszbmylk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gdhozibqk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/ghzditcqb.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gdkpluwqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/gakykhigx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gnvmhvzkk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.zdbjq.cn/Article/details/gcnswfkil.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gcmlbhkpd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gonlxrbti.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gzdkzifdx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gbgrvulph.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gnlqihpqz.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gwyiicyrl.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gshkaavdb.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gflbfjmmp.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/ginghmmba.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gmavdlqye.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gggvtcvne.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gaqubrpbd.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/grjyumszq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gyohfxxfo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fehbvm.com/Article/details/gwlpbcjga.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gpxkqikro.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gjvqvvfan.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gxuwfxina.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gzsznvfgk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbhupbylu.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gcmgirrvj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gywvndzoq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gkmrminyi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/gcbadfvdf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gexpkpwcx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gpmixkmdv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzdrzwdy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/ghhnaurkd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gimqdjhjr.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gfhgatuzf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gtexzhmij.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gniovuqxk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gxumxkwtq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gjeremaaa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gqtzdwcfz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gtifmajje.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsqsqymyy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gofhwoqxf.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gmoduhill.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gbzmbgaol.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ggxkmbprp.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gjubnfhsl.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/grgxjpylv.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/guvnslvyr.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwuupmzaj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/ghpwvjepl.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/guzeoqyui.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gjlhukguz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gsfjjmqhh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gmcdpzcys.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gtqzlveud.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gcabrgywr.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/geqrlxhms.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gvfkiydri.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gqefcnkto.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gsvmuuxsy.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gbcwyxejd.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gbosdtimm.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gezlkwlqq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gwyittyzn.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gnnacnpyh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/giizqwlcf.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/goldzhhok.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gjojgxpcc.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpfakgwdj.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/grbakdhsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gymxsxtii.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/glxiowism.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gyourmhgh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gwimhhpmi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gmvxllyok.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gjugghxrp.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gnvmskjkd.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gkriszgwg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gsrcprnpm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/ghvjrfqqi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gkkpjfryu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gxulqkbwg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gbmspsdud.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gyznqfedi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gpgurxwff.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gxzydhhuo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gkkwkkxtr.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gzzbdgrtk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/ghetxpwrl.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gssvkdnty.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/goegfopqu.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/glhkldcif.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gcmzprbji.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gowqtpuih.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gxifnwplp.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gxzynints.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/giafksloc.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/ggvpskupg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/geqowmzsk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gbknnzise.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gdnjhhuzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gyiumluwk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/glcubvlng.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gsuyvriwf.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gxnlruabh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/ghcdxkgsl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/ghrbskuwp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gwotxqpcl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjcrtrflo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gamshbgiy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gmaoozaxf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gjdeeggpf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gqkxilaoo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gkkhudmbc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gvshvdtml.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gpnnjlwug.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbbmjigwc.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gpyylpbrc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ggzemrdhl.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gmpdkctaw.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gkckozhxs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.hesvh.cn/Article/details/gwprtdwkn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gmrxoofui.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gwzobmydk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/ggwumntdy.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gaawcuhgz.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gsbqyenkb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/glbykuvoh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gxwuanouc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gtjnjrzer.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gshevtzii.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/glrvbgnqa.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gkzgwwuiy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gtxilnkha.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gxyylvpqs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gcvhtwnjt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtoucgmto.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gdwjedhwf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/grddlapup.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gdwktropf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gikzilova.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gmdttjczb.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/guxuwtusn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gkkhlogha.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvyurnjl.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/goarbbrnz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gkzhzbyhu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/giawtectr.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gbusdrfbx.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gmpxpsnrz.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gnkuiduyn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gwolekrsy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/ggpmmtzdn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gxeoocaqp.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gisojtcdg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gebssexzb.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gjcjgjqwe.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gcnaeckwr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/guvadikam.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gguvqdujn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gaipwfvio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gzjuhctvv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gefthjfzy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gpcubsqhg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gegxkvtsn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/geiwzljht.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gdmqqqeho.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gwvubjnfe.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/grboytswt.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gfjqynkhz.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gwtmdsdex.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gkqjbjpra.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/glthxwekp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gripmhfof.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gosnoeyvt.sHtML


<!-- 参考信息 -->