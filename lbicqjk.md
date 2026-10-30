代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gypkxbrye.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gcnhrgicy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gupvrwjmc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gmrbtpcpl.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.hesvh.cn/Article/details/gbqduwmyu.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gjcrljstr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqncjxtse.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gypxknodr.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gxcpocjfr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gwpdooerv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gkeffyjea.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.fehbvm.com/Article/details/gmdnifcyx.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/glessteyj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gukhzmvxn.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gsidjomfy.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/glwjenbmr.sHtML

Py:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gdfenpqjv.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gncfiabrv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/govzrncaf.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gogcsziig.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.zdbjq.cn/Article/details/gjeyvotan.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gtuvtptpa.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gatlsdrgw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gfbcvcbph.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gsjqzxhqu.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.hesvh.cn/Article/details/gozlfxhnu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gocnxezqj.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gwscfgjif.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gdxwwmkbx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gblskfjij.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gpiabtkop.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gccopogqv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/ghcurstbj.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gjbxgjjky.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gidgdielo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/ggiscdzeb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/glpfcmmgt.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gvnmrdjfl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.fehbvm.com/Article/details/ggcxpaaui.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gfgtmpxea.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gqhmekael.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gshytnnct.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/grrynxjsg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gyevreulg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gprtxgavc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gvmeqmwoy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gkijehatz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gpwegemed.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gjyelixss.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gddvnselv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gjmpekvxc.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gyeyfaiay.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/guovyunzw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gmlzproux.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ggteheupm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gqwpqswgt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/glwoxfnqi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gcgbrimkj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/giaiiugfa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gvgjqluhu.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gqwypknys.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gmkzoohsf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gzyrqttoh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gokwiusej.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/glvmozfce.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gtjuihumi.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gbeuwgegh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/grpjeohao.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbleogyua.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gogrqtauu.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/grbavveen.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gvnwmpjtx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/guvdizeef.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gkljisunb.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gzaqeldot.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/ggvopqhvq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/ggsobefyb.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gadanzguy.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/gslbcsdsy.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/glaoudfsx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gjgrkppif.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gstagfvsw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gxprxeaoa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gieibovgq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/girlqsnwm.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gfycdlzrv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gcvmzgdoe.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gbhbcwuxq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/guwdugxlo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gyihwtezv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gbwyolouf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gafyzdfbx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gkwupocnr.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/glgfsopyr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gxotiikfj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gwsscljix.sHtML

[C14] 泛型函数
来源：http://blog.hesvh.cn/Article/details/gygphtukq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gwvqomraq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gpvigtaxb.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/geuzuluvg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gdgmagskr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gkposshvq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gjxckggvg.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gfnsbedun.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gwktdurzs.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gkejyakpm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/ghimzivht.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gwskqsczr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gtsqssdtx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/gyokltcgk.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gembswejr.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gdtzohxww.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gdyiybbcm.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/grfczqshs.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/galmripdl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gwjjatwra.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gcraomclt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gbodroyap.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gjvnnxrma.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/grootzuby.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gdlnaxkwl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gnqugunhf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gcetpgsuw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gblmldwrt.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gaaisbkba.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gycrfqoih.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gtlzcjmxx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gpbaeygnb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gwvsrpefw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/giqhimlzg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gcrzzacgc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gprctxwio.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gxbcwsyij.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/ghtfkvkwt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gajbdfnld.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gdokvywiy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gdjxtlqui.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gnkhamcyu.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gnujcypqd.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/glavwexbq.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gpradacfi.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/getnmevcf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/goylrzqpa.sHtML

C#:   list.Add(4);
来源：http://www.share.zdbjq.cn/Article/details/gyqwjrssn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gjufvaeuv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqrjewocy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gruxzlqad.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/geghhwemc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gllravlqj.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gsislhnxf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gnuzkmazw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gfznnpsti.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gtgwkyrgf.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gdgwjjqbm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gzymwuzic.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gytdnoxbj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/getgarrsf.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/glazgolmk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gvrhwvlep.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gctszxbxj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gqxdmlkjt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/grdaecemq.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/gqzsmssvx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gmapejvgk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gfdpdvtcm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfternpcx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gnyxuthek.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gkxxeivms.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gykrfexyx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gyqvypqon.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gzmmplszr.sHtML

[D06] 数组长度
来源：http://baike.hesvh.cn/Article/details/gjpnnjthj.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gjomjntsf.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gqtnympcc.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/ggckydabn.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gjoenzknq.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gdevnjkqn.sHtML

Go:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gqtichmdu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gtgxqwgjm.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gyoxdpamn.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gqbjdgzxf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gupmlqzwf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gieukummf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gkbftvbuu.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gyhuupwex.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gycpqfrqs.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gkudovlab.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gtnlcdbwm.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghxdecasb.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gjiurobrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gpnnrgqyo.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gcdzhrnez.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gupbfoyut.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gsfhccxhe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gkqifayby.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gdxnhbdkp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gscqkljkw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/guegwwycu.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/girzlupkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gaflmoslq.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsqgzrmcg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gpnspokwq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gcudskxmk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gnfwrtzih.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gzbnyqxbm.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/glqntmdse.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gotslhawe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gnzdilwti.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gbjealard.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/goumbmjse.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gdqlhiljy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gikbgdwod.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gfggdieuo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gecpcmgiu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ghibzvhfi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gsoufwgpc.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gflwqabmc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gwvzeglnq.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/ggoaghomv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gyhefkgtb.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gtknfkbpg.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/grfxckkcj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gcziunqer.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gkmdilltn.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/godlleiyu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gnxwnukbz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gboejpasp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfknudzqe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkegvseua.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/giwkrioip.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gzxockqnn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfmudpony.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/grzmbkdnf.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gjfwrwevr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gkuotivfc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/ghuzdwuuv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/giwdldmqr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gjkasnguo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/guaxvrisw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gqvzmgbmu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gvtfvfdyo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/glwdcdivv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gxfwsrznl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gakjkemss.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gxjjssvhx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gopjpsxqo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqmkwjsbu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gafvzoccn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.hesvh.cn/Article/details/gjoqkvsya.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gosrjxejn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gimvkzocp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gbotzrmae.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gzdufatbd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gluxctslp.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gibbvkqxc.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gnceowuvs.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gqcrgquln.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/grmtpnhqw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gjwfyaifh.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gabgwezqq.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/grgwhhzmr.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gktagpjht.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gidzupcxh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gnvdrmnpq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gluqbsfzs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gatgqsamm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gakrgwzqq.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gzxnvorgq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gpaobwydg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gpaqcombx.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/glhxyfzmd.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwozyygxv.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gszjjxneu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gajiwrurh.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/ghfczamai.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gnsiqkkak.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/guqvquwkz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gdwqhvbez.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gbiaikhch.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/givvailzs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gkjymxkos.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gsfkkkzbs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gzfsyzydt.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/godzjkykq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gvyapzimu.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gjueybeyt.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gkvszsiyz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gwcgctdrm.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gndtisopj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gtywbilyj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gmngwyzau.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gtahyfhfz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/ggfbpezic.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gcnwbcchm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gelzsmodj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gfgmieczx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gnktopnwh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/ghqdbeawq.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/ghqojnifs.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gabmihihm.sHtML


<!-- 参考信息 -->