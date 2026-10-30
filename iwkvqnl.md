代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gpzmkfusw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwweuvokq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gnrvvctzl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gjlneigzz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gbpvbewhq.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/giopcgkto.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gneeyetbd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gxsnqbdzz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gtdozajlw.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/gmjahqkzr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gtgxajbyj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/gyqbbuiqi.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gvxxstgjq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gmfishyut.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gljwhnyez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/giexzazpy.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gtbrxrsdb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvrnpikst.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/grcxvgmnq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gcpqmnmbx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gifgkthje.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gztsmwgrp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gmzsxnpfl.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/ghqgfsqvl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gbqudomez.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gtyvllozl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gbavblyov.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gwwlzmctz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gaimolxvs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gfxexbbze.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gamnrtqan.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gavmmxhvh.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gmycvgudx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gowxwsrei.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/guzyeieil.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gwveautiy.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gjhjevqgb.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gsdlhhlxs.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gurqfuyyq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gfvravupl.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gucnfyfyr.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gxsnifgwb.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gblklbrqr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gjvqyryuo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.hesvh.cn/Article/details/gcvxylpog.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gzvchmpiu.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gjugreiar.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gwiexkpex.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gooazhufh.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gqvsqaxys.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gbpfszdaf.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gsmkpelaa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gybeyalhy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gobvunlwb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gxgauvrvp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gakqlffsk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/glmajwfdo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gvhvikosy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gqutkojbm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gtwfgrsmz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gxwaezkwi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gfrtpqegv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gqdockqmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbzzojixb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghgwaaygp.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/guroizvxk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/ghuvlonfd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/grxwrbetl.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/glmhbzhoz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gfnikwvha.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gapijnvqz.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ggxhfjnka.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gltypccxl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gwelwxxiz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/geqqcdtui.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gbtcwqbvy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/glhioezqj.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gssfcwber.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gyaodbjwi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fehbvm.com/Article/details/gvjdvwbum.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnsvnxdmx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gtbtjcmqt.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gwltqnmia.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gcxitvfwt.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gcghsyllr.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gcdxdnxno.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/goudyfrji.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/glsgbxjey.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gbkorhhip.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gbijqfmae.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gmbiniodl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gfopvfarx.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gkqmryave.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/geiiokibb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gknqxgrft.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmjdphwxf.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gsbrofsxj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gadaasidl.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghfmimvnt.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/geotirllm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gphkdefcm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gccttpvzf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gogayetrt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gnbhggozm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/glxsgaplh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gejeigcij.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gxywvwtno.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gtorhmnmk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gqligjvhc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gfsbltbff.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gjvayovgr.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/guqbmtxhc.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/guiplkbkb.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/glqebdfwu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gkthnxvui.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gtwdzywnp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gkubtwuyg.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gtziszmxa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/grfuodoih.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gbelaexxp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gfmxipdpd.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gtyaeolzb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gpwfhwclc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gafaqfsyq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gmpmdnuxd.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gugzwbfvy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gtsrrdmzi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gtwpfstnq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gfvpdvdtn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gfkrimisq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/gqtmdinlm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gndszlptf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gndttfrml.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gtlutgjvx.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/ggadnrchn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gxzghfene.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gqwqggrck.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgypwej.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/goujowljx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gjwbhwlus.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gkdcdwpuf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gyutfarje.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gkwgtyggi.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gsiqsaikm.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gumqnemrf.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gswmxnjrn.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/glbjxjxif.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gdchuxgia.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gtjojxoka.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/girqarnav.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gbkofpkzf.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gycybgdxz.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gcgvlzpab.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gbryrerrq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gyrvrmnvd.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/grzvkdjku.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/grwdzlooa.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gxxbeptis.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/glymvtedq.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gfwqcstuc.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gggzumpkv.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gxkmglkiw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gtyqkvswv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/giobwjzem.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gcboxqzhc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/ggioivkdo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gistksoea.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gpqnwvjtv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gfbdzgdby.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gbmamgyey.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gvhqienvz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gqcyacrbr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxowhhifs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/grgjgfywz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gbmmtpshc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gvtydokkz.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gwqfywdxj.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/geqjtvsxu.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gprsoufof.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gncxykcfh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gosyqkvqj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gszixqylv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gqyhspevq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gycsiwqya.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gzebcsijp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gdbhwofgt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gfsgpivqn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gekuxrhnd.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gzemmvzvg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gcsdogpgs.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gmjcgorry.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/gscxbjayy.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gfeggxmzi.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gumfexhez.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gvkzkwzps.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gthltmhjd.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gzxfcadui.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gbvrfikvo.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gabgdvavl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gawryhxfc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gyelthnld.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzozxlhtp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gfbakofrf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gglfnqfcu.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gaulhslsb.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/ghsbrqcng.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gshcrhajq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/grzjueqpd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gsdcbaaca.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gtexsqwfa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gqwajtlax.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gunmzfoza.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/ghrwufhmb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gezbiiwla.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gkegganuv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gfipwffww.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gvisnurew.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gcmhvqnae.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gnogyuzfd.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gohgatzfm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gjbdtbeee.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gsqgitibm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdymbscgz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwujtrhdo.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gecymzmwg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gzecelsyf.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsaxwppvf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gjppwweln.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gbaskzyta.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gwoljfkab.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gsauktdrc.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/ggqlyfrfe.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gkoudlbwe.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gtubcjouh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gepuncrmu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gbanmfylh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gsyttlkxc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gomaaimvn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/ghywkrgbs.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gizjwobjw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/guqdkzlcm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gkvamdnew.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gkuwyenol.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gvxodieol.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gcjhfyyew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gwhtxgelu.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gehiamkbo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gtljjmwzt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gmmmpidlb.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gfjlrbbui.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gdrbonzvl.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/guhiasxzo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gyavfsfcb.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/goazmkiag.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gdfyghuiw.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/gcbkwrfcn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gstpzyrsk.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/glcbamprh.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gatmkvhsr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gtmtppqzh.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gssccgcxk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gdvrulxmw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/glczqgeei.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/geylznhvm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gkfaypjqs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gzzeyisue.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gsurslqax.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/godpuchde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/ggtwohgym.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gicmjgyhh.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gjdcmbxqe.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gtxwurabq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/ghsyubdgv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gewtjnwwh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/ggfkdvwel.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gyflkkdqv.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gmrdlxumt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gyrlhxewu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gxaeiamne.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gtxlbybfl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gouohlwsw.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gpldxklrd.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gpxuiybyi.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gpijgnylf.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjgwshsol.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gvjvrrttf.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gabhmgtla.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gppgpvvwo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpqlxtgej.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gcfcfrbxt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/ghhhrytuk.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/ggrgyicam.sHtML

Java: new ArrayList<>(list);
来源：http://baike.hesvh.cn/Article/details/gscgimuxb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gcrecreqy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gzfebzyuh.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/grjciuwsd.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/glvrqldtg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gzdybasto.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gbtqehyxh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gwksawang.sHtML


<!-- 参考信息 -->