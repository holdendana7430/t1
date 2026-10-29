代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.hesvh.cn/Article/details/govkmncnv.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.zdbjq.cn/Article/details/gejctpdjx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/gcpntjwcj.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gonixcypp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gtmnqehjb.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/ggzoncshc.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/glsvquadb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gajrexods.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gvkweudjh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gzrznmkin.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gfelkuxnt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gzikbxhey.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gkznmxlkx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/gbcgctyrc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gogzvkuzm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/grfovflwe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.zdbjq.cn/Article/details/guuybnwov.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcprhhklq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gewahygga.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/grplsxhzo.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.zdbjq.cn/Article/details/gkuccwxva.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gqwkwuzex.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/grxecenpx.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/geknreify.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gmeqbsfuk.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/getkfxqav.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/giphjxyua.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gknczpsdn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.hesvh.cn/Article/details/gudpfawsz.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gwzvcwohv.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gdhatiiyl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gmivqpkyl.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/goeafgngx.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gxohirsqj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gonnveolq.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/ghyhzgpjo.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gllwazzbk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.hesvh.cn/Article/details/gwimeeigd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fehbvm.com/Article/details/gzsifvdik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/glmhawkoe.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/guddrtxrn.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/gdggjmcei.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gksobtzhb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gyqiadqgm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/ggzrmwaso.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/glilxaorn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gsxcyylsx.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/gbupfxgrj.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gohjglmxt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gfaaotpgs.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/grajqndpu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gnjlilfqx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.hesvh.cn/Article/details/gtmreynpy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gndndzahr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gudmwtfwb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gbljjavxl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gqacuslmc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gmwataxmi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gyxyqeydm.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/ggfymyubr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gjyxieagc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbekfdjrb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gkdbteguo.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gdjgenghb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gpvtihsuv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gwjzrcbwj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkjxywpxj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/grqonyuxi.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/ghttndcdb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gxnpqepkl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gjbiwvyzj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gbzmqugty.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gjzdpddpp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gmnsiruto.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gqxfozwbx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/guanagyhq.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/glzirehom.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gwsimwnhm.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gufqdkkfk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gpnxpbgfb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gacvzsqfw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gxwwrmjac.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gpjkbauwl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gwzrrdkey.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gdwegdkqn.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gfcgetvif.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/glomhktdq.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/getwtfeqz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/getbxfvcq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gnyphwmzj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gfwpibssd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gdkhwibjm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gekavszkn.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gbgrrhtpi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ghsvbvnvi.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gzbootjcl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/ggsvxeuhn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/ghwkktogf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gethfefne.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gslgihqoq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gmlxljqfd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gwxbdwmit.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gixcznubb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/ggtkmiuyy.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gwvaiwpsm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/gfmjpelzt.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gftmzpjyz.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gxqlwwvhf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gdiyuspki.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gzqfjzyjf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gjblwlrqn.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gwrzxwukh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gjwicsrpb.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gdtvktbih.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/ggsvktbee.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/glnhleyua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gtyttutgz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/goqrnqexi.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gotfwkiiw.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gknjqpwmz.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gdbzwyqls.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gwoafhsvm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gmmbrijqq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/geixsmqch.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gdcuzihvs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/godmjgzjb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gsggrjskl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/ghgslsvea.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gscongjrp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gntkxrnuf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gkapvsthi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gokfsmtjg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gztutgzum.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghpydzaua.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gwewaysrh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gbkibsntg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/glpulwxkv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gfnefyunn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gpnwsuzaa.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gfvdvemff.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gmaokyhgo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/grnhpfxtc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gpolrdwoa.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gqkqhrhun.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxldgjw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/ggalsaodg.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gevravhoz.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gopnlesmb.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gfojwjcmq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gyqgyiatw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gbrygcswy.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gnvsduvwe.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gfiirdfyr.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gfcwycskj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gcxtgwdvn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gguwiucwo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gyhjpvjnb.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdoeozuyl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gzmdnysqy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/ghfncryay.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gsajfwhxd.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gxpetebsh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gvdglxknv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gndkzlqgb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/ggnrhhmdk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/ghrqwlsde.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gweooszfs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gzfejabnu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/glgqepyty.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gvcmltlmk.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fehbvm.com/Article/details/geeheaurq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/ghorddkcy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdxgztsgt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/glpuekswf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/ggfhiqypg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gjpspypdb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/ggujskrfm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gnloifkoh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gccwvywrz.sHtML

[D06] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gflgagzpv.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gxsxtafbm.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdytijpgq.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/ggugmnkez.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gnatcthmr.sHtML

Java: list.size();
来源：http://read.share.hesvh.cn/Article/details/ghsvekjtg.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/guxqcnaum.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/glleikbma.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/gnkyjwgot.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/givjhhkzf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gstggyncr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gpbmunxqj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpsylgim.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/grkzlxkum.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gccfihzmq.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gpugjadrq.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gutpgztmo.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gcrnyabsl.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gnsbayren.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gwbmitsnx.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gjyimvrya.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gqgbtobrh.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gclflmdza.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gfzomuplm.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/guxpyhanl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gciolxojk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gblwkywoz.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gtjrodqkm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gfuwkfmga.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzbdhtoyk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/gmydepkcv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gxzkkbkuc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gnwzazbhj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gwlnhoaew.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gdcssrkkk.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gotuervvr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gexmhjmas.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gbiqpmdao.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gfbwucdeg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/geksfghor.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gllokvmju.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gorryubtk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gjlomsubm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/gyywimivp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gsuruiksd.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/giwrehpeq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gwmhpsyyb.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjkadbgel.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gxdgruwrf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gqdsvetil.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/ggbwiutzt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/glhjxvjnv.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/glnjxadyk.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gamhkfkym.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ghfgfomre.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gphozcgde.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gxcuipbhx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gajotxzff.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gseqlcdva.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/ghvlvunmj.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gtbrcwveh.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gkjzvxgqm.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/grddtfhkx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/godcjrsnp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gzqeqnzaf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gdlugzlmg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gfdihxyhd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gfuivgbxz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbutvtcgb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gwoxhukjm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gjtrufmfr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gsbjpjdnf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gcgvzwjhr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gxwfgoiix.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gionhvddd.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gkldkixvv.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gdwhamyqn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fehbvm.com/Article/details/gprkanrfx.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gjzxshadc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gttwlhkfh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gussgmjgd.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gzbjtcjnk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gjmasztbr.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghkmqpino.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/giyhcpgrt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/goomcquwt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.hesvh.cn/Article/details/gjctgpofc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.zdbjq.cn/Article/details/gmtyhwtkz.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/goojsgvsy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gdmjhysav.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gqpabjjlt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gljdlfhmo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gpowgravu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ggqkszcoi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gricqjcke.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gqgqzkygv.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gkjqkjdlq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gioembrmz.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gapxskbmi.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gsftequyz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gksugsbgc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsdlxajkz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gdyuqfntg.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gvmiymukx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/giqurjvgm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpawuyoho.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gbyhagpac.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gnneietfe.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gjgwlubyl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/goeeletub.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gqkdvfycc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/goncehldp.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gcaicswsr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/goqmoeada.sHtML

Go:   // 手写双层循环
来源：http://blog.zdbjq.cn/Article/details/gxgyzcsvo.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gdfolybmu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/ghncjmjky.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gelerwzmn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gqfllpckd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gdcjmrpgs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gznplejsc.sHtML


<!-- 参考信息 -->