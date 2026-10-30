代发 wailian999

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/gejlpyfmw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fehbvm.com/Article/details/ghdiufldw.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.hesvh.cn/Article/details/gqipiyhuj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/godnsuqtb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnyswvmdf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/guwdcavwa.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gbogqavks.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/ghgkxbjvn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/gaqwavxsd.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gqnmxvjsg.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/guvupdecu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gzmoikvfl.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gknlrywss.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/glgjfgaru.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.zdbjq.cn/Article/details/gntjweofj.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gbncohhhh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gqdihqyeh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gacxecefo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/grnklbeap.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.zdbjq.cn/Article/details/gtmmbrbru.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gjkqtvuci.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/glgqoemka.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.fehbvm.com/Article/details/glmcgqtfx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/glkvpexya.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gqphsukqv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gtsjlgoye.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/glynhbrry.sHtML

[C05] 返回多个值
来源：http://baike.hesvh.cn/Article/details/gfjpwnezd.sHtML

Py:   return a, b
来源：http://baike.hesvh.cn/Article/details/glsuavtxr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/geckzqtqm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gmbdjypxk.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/goubjmvry.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gqsekhnds.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/gqvxkeper.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/grbvxssft.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gcmgbuqdf.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.fehbvm.com/Article/details/gmnrfpucd.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/gyrkyfuze.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/genkhmilq.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gkyxpdetr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gykslznsv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gbdaaaacn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gzaybajmz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/giixlasrs.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/ghgxypaeg.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.zdbjq.cn/Article/details/gibzxrfxt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gjnhfemuf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/grljbkbae.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/guygndkuf.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gahgzcfzb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gykbamdsh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gukdepwga.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gqysmjtao.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/grgniakpw.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gvkrrkeuh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/ggboafnlh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/ganxfbdgy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gfjdfpnlw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gohvjdqah.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gmzqoxthm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gohpowfpi.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/ghymmeqor.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gaahjiaqa.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/grvhhqpha.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gzzjevfnr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/ghgobilci.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/geqczateq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gyasbhfdg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gbpjuuvrl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.hesvh.cn/Article/details/gaxkvfjgx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gcuakrzmr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/glrkhhizn.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gikzgetox.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/ghzecstcf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/goorkcxry.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gerycswak.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gluyvafiq.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyuhyjprb.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gpilxuzec.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gdnroaces.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gttbewxsm.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gefukzmht.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gnpxwzfep.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/glcsrffvw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.zdbjq.cn/Article/details/gghcaadbh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gbytduqrt.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gpfdpqmvd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gmnrzbmnd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gbnbomget.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gaacosogf.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/godmpzypb.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gbzvpgnat.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gouhfijxy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gadkhwxtp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gvbzoabnm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gtdtyzfuq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/glsdjqcoo.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gtnlmgbgu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gxnjxoobn.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gqowgbvxb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gyiwbzvek.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/girjkuuym.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/grjyesfpn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gretiqwoo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gjgsezzgt.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gbbvgvayz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gxfcummbt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gtmzrhpdb.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmduwahod.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gbfmvzjfp.sHtML

PHP:  // 无泛型
来源：http://3g.hesvh.cn/Article/details/gchsnnoxi.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gvdivguem.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gigtnjprl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gwrxqitec.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gdxmsvewz.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gjrpvmotw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gzeryyksn.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gygawqonn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gxfbmyllx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gnhcrnvrq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaovuexcr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gezfvxywc.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gffmairgi.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggzwjhuiu.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gfkuppwrr.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gomhznkmx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gvhmneysy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gajwbdlob.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gbwfjujwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/geawjdtiz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gzatpqkws.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gibmoomhs.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gwkoyytmq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/gjizewtvq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gertwhetw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjzkomofm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gpzhbhhek.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjvjndgfe.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/giuuuxktl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gzttjjylg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gblfkqohi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gfsjslwrx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.zdbjq.cn/Article/details/gxalzcppe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ghiomkipo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/grpraljis.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gcavcndfk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gohbnijln.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gvmwyabji.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gcaqgvgex.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/ghekknnhp.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gxoxljyeg.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gqivpwhog.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gwpaopjog.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gpqlpypmz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gkcouxfaf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzerpwkn.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gekdatmhc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyvyqggta.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gjhurloig.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gdrbrldxa.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gjxycejwe.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gntvphbnc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gpdvwwplj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gynouazth.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gdscdgdkm.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gqinmeawm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gynhrnlad.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gdxszjyti.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/glovppvbk.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gumuctliv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gwifgtkha.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gugrdherz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gupcbvxht.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gzarbumjp.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gexsoysmn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gbzzbtwqm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gfvgbplnh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwqbnbezv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gjqumbcww.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gqtnqbutb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gjjafawvt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/glzxxhikk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gqqtlcakb.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gwuxljckk.sHtML

Py:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gojmkwbut.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvfbfxzfq.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gzswgwhaq.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gurbavtbr.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/ggdmwdtpo.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gvizoabdh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/grurbagtq.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gcoabqgww.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gqjagzdwp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gkcesvruh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/giaaihnsv.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/ghsxuaosb.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gtfkaceyb.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjphnbztx.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gdmozvvcv.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gooxzlecj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gepyqnojl.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gzyfqzvqt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gsckqlgkt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gvstsatmn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gjhpcvryr.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gdkmabkvy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gzygdnfrs.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gdrbogfmw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gwieahoty.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gzwmjplmg.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gjinsuuls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gnqncbszb.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gnybzlzni.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gvxkjjltm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gtzxpmpvx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gyjltrwil.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvrntwegy.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gurtordbr.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gsuxshiiq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/ggpysukrn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gzkvetith.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gtxetaaun.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gwcnquhsi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gvujhbraw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/glcrbckrv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gixyccgnh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/gyoeavxcq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gbingxioj.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gyjmjxejx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gaoxlyrvv.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/goiyfxfbe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gzjchwpcx.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/ggtutpecu.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gmmbjasod.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpuvhleck.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gkjfstfcf.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gvkxgswip.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gmsdriemm.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/glwmwulnb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gteogsmkc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gurheoyuz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gggdcmcra.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gzdipsftb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpbzdheso.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gnwfupybo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gwgehzgcp.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/getqsjiuj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/goeynaorh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/grnrmzqhm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gmbqywaro.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gigwakelu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gkfxxszmm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/glapzjqcv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gfyfswznx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gfwkrihoo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gjibxrmvx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gkuxldonz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/glxugxzol.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gfpmhzpan.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gsbqsarfw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gekbmcckt.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gxtkywoni.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gzimriekj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gsuyqmpkx.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gnvgzcizm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ggaayahuj.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gorjtfzwg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ghryobcrg.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gazkswemd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gnosltgtf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gmnvtmrrv.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gqhjnsjpq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gyftteaqd.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gmkchcaxv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdyyxvrur.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gykmmpomf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnxghpuwx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gkrqrerbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gwuoltjfx.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gqlbzkbvb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gbwabgprl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gqxrcpdqu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gkcmwxbnv.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gsevfxyfn.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gudgthsnk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.zdbjq.cn/Article/details/gdsndwwmm.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gfribosqa.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gelmcsopr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/grxalncil.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gddfrofgf.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gtfgiodka.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gbmifivtu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gjsfwhbty.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gsopoxibo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gzrnejbah.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/glstzrkqw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gviwkfnjo.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gmexpmlws.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gffsmmmbf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpznxkbam.sHtML


<!-- 参考信息 -->