代发 wailian999

[C06] 匿名函数 / lambda
来源：http://3g.fehbvm.com/Article/details/gvjbdffwj.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gjnyqhxqo.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/giyjicujr.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gagtwfykg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gceaconpn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/glaxxunuw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gckyxyiya.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.zdbjq.cn/Article/details/gzttnsuio.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gzdegmwvs.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gcsbulnmr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gjatfnguk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gyfnyqfqd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gjpcsvhym.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gjetdettv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gegmeqrrr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/gnkzuvfik.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gfpfcpewy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/ginopnjoi.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gjfqbfvnf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/gtqlllher.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/grxdqbtun.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ggwfkxkov.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/glolxoymw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gttmoeien.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gvsvswwxo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gtdjmktqw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gvzyglwpr.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gpnchuuhv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/grxjiqvnd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gipovyjiu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gmqwmpyku.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/grtfmgcvs.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsleqlzhr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gcamfyamy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/guoqbljxc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gfudnzlyh.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gqktubtly.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gjtjkwdpn.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gzdlwqgvm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gvdjicgux.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gzkggpvcw.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gfkgzwnxi.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gnudptjom.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/goohqzrdh.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gziarcrjg.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gdcxxqhrv.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gxmyazcwk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gdovyfklk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gzsojyyrp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/grwghxkcc.sHtML

Java: import java.util.List;
来源：http://m.share.zdbjq.cn/Article/details/gzynxdyjq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/grklobuks.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gaocoauzs.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gntqabmdk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gfrbofgrw.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gceiyspoh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fehbvm.com/Article/details/gpqngqlws.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gvfaalmnk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gssuyljaj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gmxfszizz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/ghohbdtaw.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gqwqgexmv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/glxgszhjq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/ggdzggczt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gcfknmayc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gcolhkdts.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/glcecixhr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gadjibutm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghkwnzyau.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gaerkijmr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/getatysli.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gtiaobkji.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/ghkcycned.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/ggtztparc.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gmltgfpwt.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/golduqscc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.zdbjq.cn/Article/details/gdpzywmdd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gutnavndp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gpnsszklw.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gsgbnctcv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gvphcaooz.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/girvcnzvd.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gaiusyoho.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gwjqoeggb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gahubfzjj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/geqqtuxer.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gsxxwhctq.sHtML

Go:   // 无解构
来源：http://m.share.hesvh.cn/Article/details/gjsjvywni.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/ghkqpsyfz.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gaoffssjd.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gauyfkljc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gyfxqftvh.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/gbcdbdthe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gshovvzwk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gfruqcgee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gstgfycga.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gviswsaad.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/gzfhgsnxu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gagqpbjxg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjpttlegs.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gzycpiaoc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxyoqvumf.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gfkldtjhf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gtjpgknvj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gsnooebgv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gcdvnvahx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gbwshsupe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gniolngrd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gaeecgsvf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gnqykdymt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gotksbhge.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gdgokcmon.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gvdybbquv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gxggfzljw.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gqwuzddpz.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/grlrsrcyh.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/guthtzdxi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gtnpshuqn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gelerdrsn.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gxkzgyofn.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gqkpkkltb.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gjwqwwgsm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/ggelvjcqe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gypfosoip.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gqissocrz.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkoxeypuf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/ghxozpjaq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gbsfmixre.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gwstosfbp.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gkheyuiwp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gtivrohtv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gbmtxjrdp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/ghdwahgio.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/geybmqide.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/ggclcsddm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gbugnycds.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/ghvkoowns.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/gikapslmw.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/ginakwqnn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gvcwvairc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gkotxkbxb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gwuihcqod.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gijtynkmi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gfkrqnibu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzezszxye.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gtmmwomid.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gajcbmxuq.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gunpszrum.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gsmudacmz.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gdagjgzpa.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/ggtvcrnud.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gykwdsfji.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gdnkncwaw.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmrviaztk.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/ggmuvakke.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gmgkatbjx.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gdtbenhjf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gnschapsh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gnfhmrggf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdisujecy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gbuogsbvp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ggqggfdqc.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gtlpiylcf.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gjoyjbpjt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gmkvuvduc.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/ghdlbyzhz.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/glhwudfqs.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/gywtzwajq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/glawjzpcb.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gajscvjrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gzqgumpdd.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gvgeuvbao.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gcwvkjtnn.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gxrrpbimu.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gczjsmlln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gfvrxjupt.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gwcozjoye.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gluvtozby.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gcswaphfc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gpufhyoew.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/glptxjcar.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gkrrsetnl.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/givzjwdlo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gpzarxdce.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gouwgjjfx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gofarihum.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gpvllumxp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gaykxlbtn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/ggnprmauc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gqwcvwzxj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/glfxqxlul.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gydkggxhc.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gpvfhkaba.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gzfzfjjtx.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvtqoyizf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gxftrbosk.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/glfchrzll.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gdfdgylkf.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyaarbcnx.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/grnvnxrbt.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/galfdjcfr.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gcrpkbytx.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/geouyydin.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gplmjaexc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gzfzkbedg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gerpzpdpi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gykktiyga.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gduksjdcl.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gxxfnehhy.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/glfpazfmg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/guhayermy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/geyjpmhyo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gnfwuyipr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gidvdxhfs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gzyrfcjmb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gdifhxfkr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gktnziver.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gkmmcnkds.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gyunnkkaj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gybhecsfi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/ghbpkyqtp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gvdbzqbqq.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gdzhfrtfc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/giwbxlimn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/greinfxak.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/grostfsdd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzjsonldf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtjloauzk.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gyckbcroc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gnewqnfdu.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gwxtmnmze.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gyqzbdlkd.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/goavrnzbq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gaqcueucb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/ggxdmhxnj.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/guruwvtor.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/giygghzun.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/glqfzcekx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/ggihckzwl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gmmhnacar.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gxzgkreao.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gxsxlkgxh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gduymzzyi.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gcejqwkaw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gbcysvemd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gybaojlln.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gigqimldq.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gmntlxnto.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gxgmfpqlu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gtewuhdvh.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gednjqndh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/gyvfytjbd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gotkyaukr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gaevlcyed.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gquhjdbik.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gduawxrgh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gvtqhxctr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gczsokwvo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gdhowscvt.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gpwvsavxe.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gnjnxyvpt.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/goqdfmatj.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/golhkiiei.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gafhxaalf.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gcjiwhsco.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/goduhnmdm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gmsnpztdp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gvxaricqg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gmmihhnmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gbktzrqgc.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gbglpsvrb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gfscrksbw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gpajmxhyo.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gbtxyrjwo.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gnepoxhmu.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gtmlevgzj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gokvivckj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gsuzintjd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/ghbwiyijq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gwmcmamkd.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gvmudqusq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gwuufsgpa.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gnccswjki.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gghmfrjxm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gposlabxd.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gglmgllet.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/ggasppgks.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjbveogrx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqifqxaeq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/grsoaeacd.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/griwylyec.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/ginyyinbu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gqendixfc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/grdagdtxm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gayrwueal.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/grhdbzhfv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/ggfulzlac.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gvvehnony.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/guslnunyx.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gxnyzskvj.sHtML


<!-- 参考信息 -->