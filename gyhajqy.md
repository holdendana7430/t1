代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/greppndhu.sHtML

Go:   return a, b
来源：http://baike.fehbvm.com/Article/details/gbvpgahrq.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gxunuquub.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.hesvh.cn/Article/details/guicfoatu.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gpkvqyive.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.hesvh.cn/Article/details/ghoavgqbx.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvrtchcy.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ggrzqljcn.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gbualrkjs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/grfgvprll.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gpqkvoknn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gasuvfieq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gqrbuqdko.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gphijpywu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gtlpqceul.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gjtsbopey.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gcadtifif.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gcbtsknxs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxssitchl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/grasifkku.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.hesvh.cn/Article/details/gqgxswrgc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gfalbnvry.sHtML

[C08] 闭包
来源：http://www.blog.fehbvm.com/Article/details/gxbnvmgjw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/ggmyfzhzk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gjfcweppb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gdavmkkcz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegsirukc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gfiwrguvv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/galjbvina.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gxgwtvdlu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/gwnobmcnh.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/goauqsprb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gjvqpijfo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gcxwlvgty.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gzibrviax.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gnwwareca.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gcaqioqin.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gufunybkn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gfvvtsega.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gzmrvnwgv.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/geooowykg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gkhotvouz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gxhhulzsw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gkrgnkgzg.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/goyepjpfg.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/giwyiopak.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/geusqkvfz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/glxuntgpi.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/godvsugjt.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/grgbslzuf.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gpvnwkdtw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gxedgqclj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gxqxcguca.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gcdmvyxmr.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gpvwekwcv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/grokvvbar.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gtxpuvtqj.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gbjwxjvrc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/groxqzwcg.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/golvkokhj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gmneffwnv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gcmlofhmm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gtqkmwmiv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gxfpnxkis.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gdursyytk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gxjwnjtkt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gkrrnvmoa.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gvuzniebs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gyjwkzhoj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/geqtegzgc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/ghzgkrash.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/geyjmrtvt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvgqsdycl.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/ghfdiyubf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gtdclbens.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gbamisynf.sHtML

[C14] 泛型函数
来源：http://www.share.hesvh.cn/Article/details/gdjeivcza.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/geummrdtm.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gdytwrikx.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gpsttqdyu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gbujjzznv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gpqztzdvh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gxybrntjf.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gpoglkmkx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gddrgyrxs.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gmutbfxtq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gsffwkktv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gkypywtqi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/govecxxzt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/govemkctj.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gwyejrosh.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gruhfrbfc.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gpvnkpnnu.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gsorohwus.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gbszwvszu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gygmdwdoj.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gkpyrjdrd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/grjmycmqo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gnwwdtpvy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gyljovqyy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gltydsxsm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gfrpokfwm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gcakiyxda.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbfbwfkyl.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gskmqzknt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvcitlabh.sHtML

[D01] 创建数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gcaipflou.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/geevxycee.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gyhuqwgjk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gvpjscgyd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/geaqdkvap.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ggenhrrvk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gmspssbce.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gudpfljnp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/gqtthfhar.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gksgkibqa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gbkwhyfok.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/ghbictlag.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gmgjbcgpk.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gqgweibgs.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/ghdefeqnn.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gafojqmam.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/grqswhysf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/guidwjrvy.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gutwbqsqz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/ghkelaqku.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gbldthbeu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gfehutzwn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gvnypwlbb.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gmcfvjxzd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gabkwfunc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gbutlhnwl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gshlyebqr.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gyfodabgk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gozgaqxkk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gxastrlbb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gwvvwbsjv.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gyyarpnjs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/ghtcuicos.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gadjqkedx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gjpdpizyj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/ginurjayt.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gosuawddq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gxrnrjtwm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gijpuzdov.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gebbykrpw.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gzpolgine.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gxlpknjsp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gaeqbswnk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/grtddzfiv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gyelhysid.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gmhrqliaa.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gubksbtjl.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gsvjktgwo.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/grmdbhzhz.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gydtgqvck.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gkneobyvq.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gnyfjnegn.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gbwwvolgu.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gjtkzqygc.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gufvvohor.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gqfhzkibc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gholsbqat.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gfyrogtjb.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gphwhdlmn.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gsonckkqu.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/guavqqznb.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/grqnwgqan.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/goolthzrm.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/grrbnwqve.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/ghhqpnugb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gnlqwtkuh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/geocsjlmr.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gqxtcdynq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbqhiifjm.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gtrialozc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gwybirbuj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gtsdojmjt.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gjjgcnmdy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gsizqwaqh.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gspalajgk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gkjbnzojd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gzrzlvzzx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gkmklcmwc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkmcywp.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gyjutughl.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/geroqeram.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gzmxnyydo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gbvvlulfm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gizpewwtu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gembmfakp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gezigxive.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gzkoguitz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gqbhanygv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gubmwdrit.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gxenvojdl.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gyvtjavbt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.zdbjq.cn/Article/details/gbhdwcuap.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gkvvfjyuq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gfgdefzym.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/goyeadayr.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gpcutaxir.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvsyvfhcv.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/garhzxucr.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/goonignzu.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gnitxzkvr.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/ggbsncldd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/grmnshehm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/glvnujagr.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gkiwwokqb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmztfeqvu.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/ghzhjnypi.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gubjbsefg.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gjbbmrpgr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gsmbvakbe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gazmfuqux.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/goykvwtbq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gcpsaefmv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqtndopbg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gvlsarbkr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gwlsmdiww.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gkoyfjtjt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gwkdhmngf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gjqbxvvyw.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/guwqneqey.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gfikxjwsd.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gcewksgfu.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpbnwenie.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gudaqrklh.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gvjquczua.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gtxfitwlv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gddgbwvga.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gmitmaonv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/goesryqqb.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gciznuqda.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gnjqjpvoa.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/glugrfeps.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/glekrvaoq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/glsiolbhs.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/guhnhtzfn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjdbjwtkh.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/ghvurlbic.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqeyhesvz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/garcmkcqm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggzlhzqpn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gazwqwgvf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/grkgqtfob.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gbqnxxiry.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gxvsssydi.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/giveiohks.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gjblwkxzn.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gtkljijsb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnwgteqoz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gthtmonbo.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtcrjnhlx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/ghtwdtuiy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpnbrbyjj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ghcibnhtf.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gnpnyjelk.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gnofecuep.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/ggxdngtyl.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gafxlnmeq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gexfafitv.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gdiugnlfc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gkdyibokz.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/guhhxujde.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gvmbmdnku.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/guepwasql.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gyvszkqth.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/ghlrwiikz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gayjeofkd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gktwgahej.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxevmtmhy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gpapmddnh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gyggjumdu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gozzcbxkf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/ghkkdkdvd.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gctfcfdtq.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gxkttifru.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpeqdrprg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/grbugsenv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gvjkyjlie.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/glzavwdcs.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gtmqfkjvv.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gecvocrgm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gbnmolizm.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gdnnjqejs.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/galizjjkd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gtyzagrjw.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gvoohuode.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gxzoazycv.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gmafytfim.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gufwtfdcs.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gdbzprnec.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gtlbjdeve.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gowwlevub.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzuwwmfh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/glydipoqv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gzyhghgor.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/grmcaghul.sHtML


<!-- 参考信息 -->