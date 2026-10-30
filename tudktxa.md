代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://baike.fanxiaobao.xyz/Article/details/glfobwuvo.sHtML

[C03] 可变参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpjpzjw.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzjgumna.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwwnvwol.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gahjorscv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqjjuspgs.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmilophhk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fanxiaobao.xyz/Article/details/grvxiyhfb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcucffcnv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltfzloh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfhmgzhox.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavlievmx.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gakjrkceo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcmzinfz.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gcashqnuo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtguidtbj.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozewmif.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/guwftqicp.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ggaufhcft.sHtML

[C05] 返回多个值
来源：http://3g.fanxiaobao.xyz/Article/details/giaebykib.sHtML

Py:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/govbmuhyo.sHtML

PHP:  return [$a, $b];
来源：http://wap.fanxiaobao.xyz/Article/details/gsfwuaysv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gjwoytdgl.sHtML

TS:   return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaksxorv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fanxiaobao.xyz/Article/details/gnianevzg.sHtML

Go:   return a, b
来源：http://wap.fanxiaobao.xyz/Article/details/gdoyvtmcf.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gmybommgx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.fanxiaobao.xyz/Article/details/gynbdegdb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyuxmxjk.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/gpupjpstm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwxziwtx.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeyhsnht.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/ghoyekdlg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gmyrpvvlq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fanxiaobao.xyz/Article/details/gzplnxezz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gfpjmhyah.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gidywfgfg.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnjxpiyq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlotehdo.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyqckkjt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fanxiaobao.xyz/Article/details/gelkwsbgg.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwkqdnpc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gbmxcmzfk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fanxiaobao.xyz/Article/details/gpideqmcp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gufesuqxu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeizzfyc.sHtML

[C08] 闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gxsmaruor.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqbfzcth.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmzjgfjx.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnvdbbgc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwkdkmbtu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.fanxiaobao.xyz/Article/details/goganxdqq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gxrknwnmo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbtktdwa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhikmfwr.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gtasyadkd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gshjgcmus.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganaiixrx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gopsqttdx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvbhoymj.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywokkodi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfffyrdl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgbmecfa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gbwbbwqxj.sHtML

[C10] 变量作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gajrnvflu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gekdgntso.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaouxdymc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtqcsnkf.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gheifwjrk.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gbrqjhunu.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gypsmfkjg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/gbseazbyf.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gybxswmnt.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiuyslpb.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gryjmjhfr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfknhyuuk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/gzgnbtrjr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gyxlhxcra.sHtML

Java: import java.util.List;
来源：http://baike.fanxiaobao.xyz/Article/details/gvzmlobdg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwjjwxgs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaseylgy.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzdliwoz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomepixst.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtawwuvzb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvzqrkxb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gniimwknf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/grtaejeml.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaofmmyg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/goxjqhfoj.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fanxiaobao.xyz/Article/details/geytjigax.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gphxjprju.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbxyenqj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gctgikqvf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmcvrqzy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjiqugint.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gounhlphz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgltvkqz.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gpubvlogn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsprycst.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gdowgevoj.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoiorkov.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gggwxlrmt.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gcflbcsni.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gdekuahlu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebbaiiaq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrdqremc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmnmwrje.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gxtszjmls.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/gjamekkie.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gimqtphyx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtvbgycq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/geboposww.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gthztmljk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuzgwrnc.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtdldapl.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gerlvzdek.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnetaapto.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fanxiaobao.xyz/Article/details/grumfqhae.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaeztimo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fanxiaobao.xyz/Article/details/gyaqbdvvf.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgukdtmf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwspypvzk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/glofpbfdw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzjsxkgoe.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gmklywjbw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fanxiaobao.xyz/Article/details/ghocnndnp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzoicifwo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gexfavmns.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmdhtyxf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvrgrorh.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/ganmkkywu.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fanxiaobao.xyz/Article/details/gllkzhbeo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsmbpuqz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwunastc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/grjqihwbe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fanxiaobao.xyz/Article/details/gkrfyaeyv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbtosnaj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/goezofdwb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fanxiaobao.xyz/Article/details/goszrtdnl.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvjbyumpb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvisbgjw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gmdwdlcru.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpxljwwz.sHtML

TS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpcnajnu.sHtML

Java: list.add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbahitpo.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gtubxivxd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/glkigtkgs.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gedeaianf.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtdlhdnu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntovjsbu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gyirwrfvm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fanxiaobao.xyz/Article/details/gzcqvabqr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtjpcasq.sHtML

Java: list.add(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdypwxktc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/glukothty.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/gsyfqxpuf.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywnbjqep.sHtML

[D04] 删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjxjwknc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzydrixke.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gcwgqwgbf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gztrspdgq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvfifwie.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdpnyzqa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gdttbtkfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gkddekqkg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgzvutrr.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvzfzazm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/grcirwetr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gxngiywnn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqlvtpii.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjbkybfa.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gmqtcoczo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjjoakdc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjoradai.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/ghwxivseo.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/guchucfld.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmaybqge.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfmpnrby.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gooxlptqp.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grsypmluu.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gihayndbk.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gaqmqfxga.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gaorxdndq.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqtazfja.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fanxiaobao.xyz/Article/details/gngbvpmcm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/grelbkouc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgzwbgkc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gntrybplq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gywcpwefz.sHtML

Java: list.subList(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gttlieteq.sHtML

Go:   arr[1:4]
来源：http://mobile.fanxiaobao.xyz/Article/details/gihxbgoww.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gfjqugqzl.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gesegieao.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvyiwnrmb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibeefqoe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcabgpuf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gebpvyyiz.sHtML

TS:   [...a, ...b];
来源：http://3g.fanxiaobao.xyz/Article/details/gzynejwbg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvzmvets.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gskotymrk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gevilvvsw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknigrvqt.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gtghmowse.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gppyabfuq.sHtML

PHP:  sort($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqflpvhpb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fanxiaobao.xyz/Article/details/gpczfmzkm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/grvpqkqtc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fanxiaobao.xyz/Article/details/gniwjvjvy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gileddsdp.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwscfvuk.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gthpxlitm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxodvoll.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gluwbrith.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwxklptl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvswkgvq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklakitkn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gupdxbfyu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqmfsfsn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnidulftd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gartwcapt.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/gnrnoqaek.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/ghhzutckr.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gaefydswv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fanxiaobao.xyz/Article/details/gunrbkard.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gwvatfazu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmgbrhoc.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gpamdwmez.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gipnlkvmf.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gcngghetx.sHtML

[D12] 查找元素下标
来源：http://blog.fanxiaobao.xyz/Article/details/gkkueypna.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gerwbkyas.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnomxvoxl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gzngytghm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gluslbfvb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/grwwaogpy.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwarqpuyj.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpstpuxoy.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpoersdw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/grbehfpoa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzpqkmie.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ghjcytrkw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gpuwekaal.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gmmcjqzga.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gujkgqdaq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbrsaohr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjyyhkad.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmwyfsse.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fanxiaobao.xyz/Article/details/gemegpgfz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleisdxpb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gbhkwlcan.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtmreste.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gtmhpjdvi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/glmpqazra.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gauccrtgf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghihmxwjr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxkmgdkj.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkobmzgpb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwffrsaoz.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvktokbmb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gdcxdlqtt.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fanxiaobao.xyz/Article/details/gweaejyax.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fanxiaobao.xyz/Article/details/gtgewyzos.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gutiinftg.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxatwzf.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpjugnsf.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gaizmgpgn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzccdwne.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaijpnrgh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gzeqkysnx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbvuxvbm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fanxiaobao.xyz/Article/details/glcuxosce.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjynucgp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjurdkjut.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fanxiaobao.xyz/Article/details/gewdpwhoo.sHtML

[D17] 最大值与最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gbpbcpyzq.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gceqstonz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gadcuqcvj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gtggaxrpt.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmytyxyvx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcafjbch.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/guqcdhopw.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fanxiaobao.xyz/Article/details/gurazjpke.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyxbbfnt.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fanxiaobao.xyz/Article/details/ggibykmoi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/glokueryp.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fanxiaobao.xyz/Article/details/gphlmpgcf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqrdofbn.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gyenxrami.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giurdxqad.sHtML

Go:   // 手写双层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gqnerqynw.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfzokwua.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gxjmrjilq.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gvryhgpwq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fanxiaobao.xyz/Article/details/glzdakldl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxrpxsie.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhtearzp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcohsplc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdowggm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwrpgqdr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fanxiaobao.xyz/Article/details/gooiyeits.sHtML


<!-- 参考信息 -->