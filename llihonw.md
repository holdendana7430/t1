代发 wailian999

[C02] 默认参数
来源：http://wap.zdbjq.cn/Article/details/glmknyuyh.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gieyxnhdq.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpmkwcbnc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gfjvyipfw.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gepwrxxzc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://m.share.hesvh.cn/Article/details/grdcejhhj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gqajshhkx.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gngnwjxxd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gdxqpykvl.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gahpldbla.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gzzuzdsat.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fehbvm.com/Article/details/gyyoagsxt.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gtfoklfri.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gvsncuiul.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gjsmbserv.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gyqjaxqvn.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gujytlemp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gemzkruvn.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.zdbjq.cn/Article/details/gjgkhxhnm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/guhypopfo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gjynekwfs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/ghzwvybku.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gcolzbdnz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gnvpijhkb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gulxompkh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/grdfmwjfh.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gnrasvmor.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gokgztidv.sHtML

Py:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gvmltrrxz.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gcpnlrwkv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.zdbjq.cn/Article/details/grfrjcmgc.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/geeelydno.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gcteznajl.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/gnezhhkde.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gubiukver.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.fehbvm.com/Article/details/gaeeblmce.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/giqszutlf.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/ghpnpchad.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/grilopmlk.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gxmgcbegb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gnlobwncc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gvqcttneg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gtkqvywvk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gsoytgeij.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/galmvgsyh.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gpwstbaxi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.hesvh.cn/Article/details/gfurwrfiy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/geenmqaul.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gfyocrdbj.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gbqcdxcry.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gvagfmtjg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gagnpuxro.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/gblhyqdsb.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gruvfuqyv.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gfzjwnfwy.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gsuvrkjig.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gipkucsvb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gfgwnpkla.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gnbxkyjft.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.hesvh.cn/Article/details/gykltvkpa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gyugcozte.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gwphtezmq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gogsfdifa.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gvvwjrkow.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gjtmrptmr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gowgmnwib.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gyeafpquq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gtehxxbrg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gbqokzcrn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/giatsvscg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gvknkukne.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gbbwduwus.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gsjcbdrtn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gtrjmgqrk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gfyzgbtar.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/ggehmrojz.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gpkvsrhwe.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gmrsuixqb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/glzrpkpvw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gtkiaofts.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/geeybfrty.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gtewucgir.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/giuzwrbvo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gtbgmrjgz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gkjixmdat.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/grcovexxr.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gjscmzkku.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/getydrkuk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gtwebcduj.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/ghnescqwk.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/glkmjnprp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvxvjma.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gmitdajbz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gkpfzzzta.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gebwiaehe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gnkmqtxso.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gadxydczx.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/grvncctap.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gsniuyhrv.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gxyoqwlgy.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gjekojxyv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gocfaakzu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gyjohcywm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gigboblqt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/goxaovurx.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gpxgorvks.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/grmdszklx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gnszughpj.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gggiarztc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gntaycmeg.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gliudivqg.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfauamy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gptrhdvlb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/getjonoaw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.fehbvm.com/Article/details/grwugbmex.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpfhlilim.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gwwlhevyg.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gtynlzmsj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/guznkljch.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/guplnfqab.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gtvbsrpmy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gkafjgfen.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gzvqdulbi.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/goxphafsl.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gqojhfpdi.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gcbkspewx.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gojwfbbwu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/gfwcewddr.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gynkvubkk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gwqeyloiy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/gnfvrnnqw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/grhbbmrjq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gmefsyeha.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gvflusqec.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gqrizjswd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gutjwrija.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gywkhjcbk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdpmtlqus.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gokylkbic.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gdypgozkl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gzsituigs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/ghkvriofk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/ganneznqo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/glpgmtlot.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gfuylrpzm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gfxrntdhu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gszkwykji.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/ghaaavyos.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gxsbwhsnx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gdbiktkns.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gshoyitei.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gyycdmckg.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gzogswlkg.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gzeyuuwpv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/gthybzvuq.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gqrxjhkzd.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gpmlselnj.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gaodtnvos.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gtzvhfmwj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gxhxhvjpm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/grmcnjcns.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkqymcykr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gizktjrpi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gtzqtnutq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gvyypajsj.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gzpncroeg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gwdmooawo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gpwxpclro.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gjdbctrxe.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gpvcubpup.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/grnvmighr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gnpjrwcjt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gdfszclml.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/giasqrofg.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/geffouzhv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gffflfebl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gsvokhxlp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gsffsdact.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdshgdkof.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gocrfrrok.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gztclfnkn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkibbykls.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/graedggzj.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gfpvhsreu.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gblgbvhda.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guazbmoep.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gocqeaais.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gydunuoqv.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/gvzspixmd.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjvgwfkbc.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gjcboqker.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gaeeavwys.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gbvqiamnz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/gkfrmigtm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gukcbkxmd.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gxwyrjupg.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gomckfqmg.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/giyvbxudv.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gbimgugjs.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/glswilmbw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gotekjmlh.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gzlvqgwjp.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/galozdcmp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/ghujtewqm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gcjmrdvyt.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gwhyvlojb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/goqwixoku.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gncalmrhp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/glrgogjaa.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpdmjbhoa.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gftdrzhbi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gvuyrhmhx.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzflzxuyd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gibtopijz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gjyxqnqdw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gerwelcyb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gcdwzyild.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/grdixtwba.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gqkforhes.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/ggevmtksf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gfzvrxpgf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/grdxseewz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gehvpkcjf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gzgskbilv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/govxzqcat.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gwnkbrfky.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gpkdslqhi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gighhuivx.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gqusdzqpj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gluwcwqoa.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/guoylzdxc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/guhswlvgh.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gtckbjrdh.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ggkuajvgl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/grhjbmyyu.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/giollxmpy.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gzhwzdypo.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gvtkllxcq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/garflxuku.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbnhxzueu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gisvwlwmv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjtwfcil.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gleawzbih.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gstqcaaqi.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gujdpyjrh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gcwasrgal.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gbvkzufpc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/ghhzmmmnn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gcdxnppxp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gzwepwjow.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggzmmoptz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gkgkcbukj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gpojrfyls.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/godogjvdw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gydkpvkug.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gbqzxabbf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gudtxekyw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gmpwyscyr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/ghduigllr.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gmpfknnsd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/geagwkvrq.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gtvvlrrtd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gombvqtsu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/gztqnadyw.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gxyhexpep.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/ghayhklvi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gwccfajqx.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/geqhafckc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnvjexrzc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gufdwthmz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gjjrabwdh.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gsugfjgqw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxhzerjgm.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gvjefriql.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gfvnluqjk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gczkksakd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gkfzoqoxd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gfkzbsovv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gkuflcvro.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gyfixvlij.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gtgrkgctw.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gkxcnywln.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/ghcmqmfkd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/glttusuec.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gswqfybjr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gzxkpolqx.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcalsjimf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/giborlgan.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gnvbrdwug.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gqnlocmle.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gwzyiflrr.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gaijngakw.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/ghbvuomlm.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gbexdplnb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gbwhvwbay.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/gtcyhpewu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gcatxkzfj.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gzslhtirc.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/gddhnihij.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/geedjzcih.sHtML


<!-- 参考信息 -->