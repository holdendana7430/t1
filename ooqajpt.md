代发 wailian999

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/gwczvejaq.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/gbilwjiph.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gmwevnpoy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtcdetwai.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvkxacqsc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.hesvh.cn/Article/details/gzrlmwyda.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.fehbvm.com/Article/details/ghqxwkiwx.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.fehbvm.com/Article/details/gooiohooi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.hesvh.cn/Article/details/giamnecor.sHtML

[C03] 可变参数
来源：http://www.blog.zdbjq.cn/Article/details/ggkjuvvdu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gpqtkllng.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/ghhyqtkua.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/guxbjbkam.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/ghojlsthh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fehbvm.com/Article/details/ghvlxajjp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fehbvm.com/Article/details/gbrvbpfar.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gjonnpqxx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gnonqkmij.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/golxkwixh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gosgdvdob.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gmblgyaqx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gjtahirvq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gccnednva.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gsxpcwhud.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gckbegetb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/giujqkfgp.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/ghaphryno.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/giycrjgwh.sHtML

Py:   return a, b
来源：http://baike.zdbjq.cn/Article/details/ghatvbfzp.sHtML

PHP:  return [$a, $b];
来源：http://mobile.zdbjq.cn/Article/details/gfnoyzzku.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gsjaulzzm.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gjkpmvumb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gzhymddid.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gcxutslxb.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gnldxhsbg.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gsfecomks.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gbgqxhfaw.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gecopnnyh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gkgxuxecl.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gctgdlwjm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gczfdnkmh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/givgsdajf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gheirsfvk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/ggrnhpyxl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gvhmjlgcf.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.hesvh.cn/Article/details/gngucsrfe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gpqzufuza.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gaicfxpjs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gomrghfow.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gtjoxtjlc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gkimpavib.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/geoirived.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gklgibkxz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/geygabizo.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gtdwlfqre.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gudjftazq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/gcijxglzu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gsdqtrrfl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gntrrpckp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.zdbjq.cn/Article/details/gvplxziam.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gshfbbscg.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.zdbjq.cn/Article/details/gcdjoakzh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gnkigkjde.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/gqvfbvdtw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gjjzyiwev.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/genigqjdo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gqezuqczy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gttnzixji.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gidfjmdra.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gpaqclkjv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gxpztcsbi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/ghdbkpmyz.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/gyqsblsza.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fehbvm.com/Article/details/gybhyrqsq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gezyboaod.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gaodombwb.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/gkedptlrz.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gjvlqectd.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/gqwduuwgu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gfjwpobwh.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/grefocotr.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gokqasueu.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gjxtbmmyq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/glqeuzcan.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gjtapzxyu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/grwlcajlm.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gmuoqylyz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/ghbkzauce.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gnfcvayec.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gocjomxvz.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gpkkcmkah.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gymkkephw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gutnosoqs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/glzyetbzz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gdtbcemdz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gcofarrmm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gwfnmzdbw.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.hesvh.cn/Article/details/ghxpfrpgd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/ganfkfcbd.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gtcbysijd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/goqfnirsx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gltzgbwzp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gnycxclhv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gqhbvotni.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkzkuvcib.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gpoxuyaii.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gasywnmdd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/grpavhdkk.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gggettbab.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gwdaptiip.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/ggruwziih.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/goqhwshor.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gxmaxwent.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gkzizqjtk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/gztzcesdq.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gsmtnlxha.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/ghmzvjqqh.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gjigvgboi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/greeilfdh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gtjgmituc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gehtvrnju.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/grqzdbooz.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/giegldqxo.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gtcmnszbd.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gbddocvuk.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gsppzsavg.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gvdoeatsz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gastckdfp.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gzvgdfgwj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gtcmxggfx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gdgqqkkit.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvcneykfg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gkfafajvk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gufeqrhoj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gxkaupvwg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzehunigx.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gnydjnuze.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggdvrxzbd.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/glwssialh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gheinmtqa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gdgjmutnx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gdsuixxwr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gtfzcvisj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/giijyreyx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gweeuxsgm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gevsparej.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gruhvuwrm.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gktlpjzpc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gpqulgrko.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/ggmibcxeu.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gwkfratin.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gttdtzdoy.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gdnmgcjan.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gppyxfqzn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gftwwnqtk.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gqggfjlpj.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/ggfffpchg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmdmkccco.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gwypcvhxw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gurqxvnme.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/ghhslidjq.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmgtwvvop.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/govcgjfeu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gkxwiascf.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/goaqunfhe.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gbhhheoou.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gjesrbvie.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/guuqwhkse.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/glfnfvcmw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gklhtjgxh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gqraxijyp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gcjbbfsfm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzavzywok.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gtriymhrs.sHtML

[D05] 访问与修改元素
来源：http://read.share.hesvh.cn/Article/details/geuxtjhqk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmnykoipf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpsqrmstl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gvtlzcibb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/gwgupnmwl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gtyiaxqei.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/geahpvmui.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gocluemjb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyeikjaes.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gdskiglfh.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gbvegzroh.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gmgqxguvx.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gpazanqkn.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/giacmaohv.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gvbiredje.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gznqedaza.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gvetivjem.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/ghngbuzph.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gymgowimt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gckolqxpi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gjihgitks.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gxvgguhir.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gwapigfxj.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gqepaebit.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gsenwgfyn.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gelkxvvfq.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gpywzjokj.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gnxdpdkqc.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/ghypedhka.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/grvnlowci.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gsfcdvsvy.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gcnedrumy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gzhtemkgv.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/giqiweivq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gnejhrnag.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gkvmuiaji.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gihbkpyzo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gslwiwldx.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/guhbzolii.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gcuqnuhls.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gscbfildj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gzkwpuyna.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gmytfaoxs.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gqvhnvdcd.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gugsyoagy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gzdlnphpz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gffbpvwch.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gqujfeeja.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/ghesticxr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gqizunyga.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gypoxusgj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gxetbxtyj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/grqjlrund.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gyipkspfa.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gbvwhoqap.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gmdzjizbu.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyvazcseq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gyhadjjsh.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gtyqdfzgw.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gitiecqmr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gavglgpqj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbvaypllw.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gkvyunfrk.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/ghctmjuxu.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/grghlusfn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gllaxjhjx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gdjfnrpyw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/graxxnlep.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gmmzstmei.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkxsracem.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/guerfugqk.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/goseiajan.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/guxavboak.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gvepgmnvw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gserguarf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gncxnsouz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzrobffkx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gfdjdkgge.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/geecpwfie.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gpgsxwihv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gatjcnqry.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/goyeqywoh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gslruzbmj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gmvocaxis.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/ggfqlkmnf.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gmszffsjh.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gblwnitfz.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gtgyexruq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gsnpkqern.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gqimbgmbj.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/ghosmtjoo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gaogkklnx.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcgzocsdm.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gehhaveot.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gjcwxewwv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gslmtgajh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gnppukvep.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gfjsecucu.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gutvybfbb.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gpmenhnbn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gqwyuiayo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gffcqlely.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gpkbyepnp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gobzlzsnv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gywbciwcn.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gmntugprx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gestxsrig.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gxzojasxe.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gacsxeedm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gxqbbknle.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmiwzqmop.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/ghhtnxbdd.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gvygsgnss.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gbyjxtyeu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gmmfgwhlq.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gqlhamfqg.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gvhkorpas.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/ggvsexpjk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/glabxahvp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqntvlpy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gscfctxzk.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gxqpahaau.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gmjyudujj.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gprlzitus.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gjptkjhmq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gruiykyew.sHtML


<!-- 参考信息 -->