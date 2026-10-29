代发 wailian999

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gwvagdrfu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gjnbuvufy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gydhqxhbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gsavmmhuo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gfjgyxhos.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gkedscrez.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/gjnbxfdcx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gocbtkicl.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gtwmlwasc.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.zdbjq.cn/Article/details/gyvkjrqbj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/glyureshn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjjcxgare.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.fehbvm.com/Article/details/giuvkmurk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gcutrsidy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gsskzqkkl.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.hesvh.cn/Article/details/gmjrhjryp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gfguivnjf.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gqxftpkqv.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fehbvm.com/Article/details/gfgxjakyl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmbflnhmd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gmpdzlvtj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gatvbzype.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gdxjgernr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gvdixkgdb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gcikhvqtg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.hesvh.cn/Article/details/gyybpjxhk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gzaxegtwg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/giqcrggwd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/ghlqtjsyi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gdfcptbmf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gughfilik.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gpizuppsu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.hesvh.cn/Article/details/gcesiujaa.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gqwkvsolr.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gjdvnmphs.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gcbzmloix.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxsuwoika.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/gleuwkuir.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gfahydifj.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/ghpeimlvs.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gzjvkoljm.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gkibhqhsq.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gvwbbiaep.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gjlkfaphv.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/golmydaca.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gesoyeigk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.fehbvm.com/Article/details/gyqzeycgt.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/ghorhdexg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gxdakcjxx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gdkblukgg.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gzvzmytdt.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/getzuiflq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gtbqadcbh.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gdfxcprmu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/gnmqssdas.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gldbvavoo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gackwjfnj.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gcpzgbdcp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/grpcehkcv.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gyyjzkqha.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gsqxztsma.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gqwosgbfs.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gtapwkpyc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/giukenqwm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.hesvh.cn/Article/details/gblcywtec.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gbztuqjnf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ghzvtkikq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gagbmjyrr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gorgoeheq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gzzurpwzw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gcjhvnwbw.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gnerlkirb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ghzjqirwa.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/gqqruvbph.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gbleernlj.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gypknoqkm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gyluvrelh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gbjxlaljt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gsvnvojhq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gqukenfcl.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gzdntjuks.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gpitrkrzk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gfmfbtrqy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/grlcqnbol.sHtML

TS:   同 JS
来源：http://blog.fehbvm.com/Article/details/grnrtvckg.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gzkjxnyqp.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gurzkazki.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/gwqwklrue.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gvzegksot.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gxhyhsqau.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/glukxgmiq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gltuotyoh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/guwffzahj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gptzghpab.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gndwarapr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gvyuizlem.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gwineyyte.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gtwzohwho.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gidkxkeos.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gcjycloyt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gvujygwur.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gehtjahjd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gocpzoudr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gvalnajcg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gpyfystll.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gvpjlayll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gxdwjlfiy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gkzzhdbun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/gisvmsazf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gupmasrhs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gqgcngufm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gcpvpaggo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gxqxouleg.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gfoemmoib.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gwvankehu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/giltyddqs.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gywjztejy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gylicpxmq.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ggmiixsgk.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gnsdqlkap.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gherwyrge.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gdxzgirca.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/ggtfrrnak.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/grkzozrgu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gxxwfodrv.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gttagqjaa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gxfdvyhgk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/geuuvkzjz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gshplguzq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/glsxnpatg.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gbktssdca.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/gdwrjprpp.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gdjdaavbl.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/glciibnww.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gwqubxchc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gljlroamh.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gybxtvndi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gywcemdcg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gsodsbfno.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/ggkuptckq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gvpxcesie.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.hesvh.cn/Article/details/ghkxufssa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gtfstmjwi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbhcegcpj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gsvrhjfdj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcwlplbjz.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gapkjubjn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gxpmgslso.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gffkyqenw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gefozftij.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/ghyyiqkhn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/ggbzqvmgo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gudpadksm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gcysikcxp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gmyemdple.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gnjfjotkt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gpyeervvh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gvctbpsvp.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gduxcurhx.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gswdomawy.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gtvfnpjuv.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gvpbkkurr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gsakcdayz.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gawjpojpd.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gzldpglbe.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gabzwthng.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gdwrrpqqm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gxgfmohmc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gvadspzbj.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/glezglxyv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gmkdwgktx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/goboksplm.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gprnzjvxc.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gvsjghndw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/godbutwry.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gzbygxtpg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gkjzicovi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gqzgpexpl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/glolxqkic.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gblvzfean.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gfxzylwcl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/getstpsfl.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gzotqgjzy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gjwmygqre.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtmohfvxc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfroeoaux.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/glbzbvrsf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/ghqgwakkl.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gctorntig.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gojtxkmwl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gjecpuwzu.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gweodiyrn.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gijrwpfhv.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkseanopl.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/guestcjbc.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gmjcondiu.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gvdzpdiaz.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gkgpfrwdk.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gjxkoppty.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/genxrtcra.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gojzizewk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gekuhksui.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gupejvnxz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gtecauhzw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/grokslnan.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghutxcitp.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gbsthalko.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gkvoguahy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkpwawmjc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gptlvfher.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/ghecxracy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gppzhyftu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/ggrmiyzfx.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/glgxnrtct.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.hesvh.cn/Article/details/giimfjrba.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/ggegtnizk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gupptzzko.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gkravldpl.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gievegfir.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gvhkcmozu.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gblzhnmxw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gjkpxirtu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gvjpmrbwi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gkmlyenwg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gshlzehqb.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gvuuagvym.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/guhnsrjsc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gzqvlppok.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gogqbegpr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gcmgbgkvm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gjdqcdehc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/grpsyectz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gsmlfjufb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gjflhpuoa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/ggerswaeg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gfbekfrao.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gfrfskotz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gfhvxeigj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfqlcaojh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/glvxsalwc.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gtrnrpfdg.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/grevhatai.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gixecvifj.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/giuealppq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gimqwvcjy.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ghchpgssn.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gyjkvghak.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gmprwryeb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/giywygtdd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gsrdtmdfh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/ggjyfivqj.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gksarjxpt.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/ggwztgufc.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gcdptnnjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gihjwkvvb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/grfuozrxq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gsytigyfo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxbvvhze.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/grfpkpbuo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gexohsujp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gqfmlvngh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gdfriehnk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gftadzbal.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gtbaiaytv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gbhjyzkgz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gxifscsbs.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/guhpinqfc.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/ggolyjarf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gsydhdlzy.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/grncmfhin.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhmqazts.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gleuckzpm.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/glougdhbg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gjuvkgneb.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gordwzzus.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/grdpsghfc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gflpugmpf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/geuidrbkt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gtctlsnoe.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gqmedzrhk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/giaezpygn.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/gqixeqzhm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxwgsplwm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gfduazjwn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsicpvigv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gueuqdote.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gdubpadix.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gpuoqmfkj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gtrvsperz.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.zdbjq.cn/Article/details/gisrbrpkq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gvnmlihnn.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/glxywurse.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gigfyxpcx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggurghwxx.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/grvybfwee.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gcdyjxzlt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gfqctkias.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/ganqzzbbf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gokorlfnl.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gsgonxcun.sHtML


<!-- 参考信息 -->