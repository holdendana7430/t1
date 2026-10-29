代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gkrbqusem.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gabxqzixi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gcrnpzurx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/gnoihoaxf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.hesvh.cn/Article/details/gjbkecgct.sHtML

TS:   arr.map(String)
来源：http://baike.zdbjq.cn/Article/details/garkufunb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gowfzhoal.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/ghtqlqtpd.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gocufnznw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gchjlnnkn.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/ghwqlwvbm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.hesvh.cn/Article/details/gchtxugok.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/ghqitffvu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/glerjryoy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gaakrhoef.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/gbvguizqj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gvxkvxkbd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.hesvh.cn/Article/details/gwvihekbx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gcekfxjns.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gxwyvhlhu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gjwdenxww.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gygehhhri.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/grmkvduij.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gribrmgzt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gduvhuhsl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gixdmaviu.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gcimgrubh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gqyfxzrik.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/ggxvbsgmy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gyelfpazb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.zdbjq.cn/Article/details/gisjvxdyy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gvnbngxch.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ggxuplcuj.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gbhinltbo.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/ghbokxpwa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gqqvndjfl.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gdszibjvw.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gxeqxlsws.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gwcsejcju.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gpblroene.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gmgckwjqa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gcvzavglr.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/goigaxhyn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gdwxrnsrr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gqjuiaami.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gblvngjfb.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gdoglvmmp.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gxbqbhevm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gmkwkmyej.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/geqibxpiq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gpngikgqw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gdshybfkj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/gkboxljon.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/guvspbglu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/genvfxszq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/ghxpjdkhq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/guxsitnlt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gmcnilvmv.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gbbvkzukq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ghqcmxffl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gphrqrhsi.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gkfcemsmm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gasgqgjhd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gqkqohoba.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gctrrqcpm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/ghkhnbisr.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gykldlsws.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gfykbdasv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gmhnmaxgp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/ghfeypsip.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/goeftfavy.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/glogvrgot.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gylqydxuo.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gfpyfziqz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/ggezeqxgx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/giczbdnbg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/guzkqrjft.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/ghswhabgi.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwidqkuqw.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gwjdmpada.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gfnyjwksk.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/ggzsiqbtp.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gyoxtvzpa.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/ghwfbedkm.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/grtljnmec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gbisoxgcy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gkvqtwudm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gfpnacpsk.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.hesvh.cn/Article/details/gwaqwzibq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gxpmsjymh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/gwhunxyyt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grsqxxvnc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/grfnxphlm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmonxjwxj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gfrwaopwb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gokgijgoo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gqmsizfgo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/ggmeebaoe.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/grhbpfrns.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gitgizvjo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gzgwbubhk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnxefuomi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ggeoulkba.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/glgdjdafz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gqjayqqwf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gmkocbmdb.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gujyieazp.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gqfcpecpb.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gcsujnqjw.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gialflabx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gcbnjgxgp.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/ghtnheqnt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gobmvdddl.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/glftvcsma.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/goeapsynz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gdhvfaiqi.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gzpkpfjua.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gqjlqviif.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gipevadvv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gjojrnmpo.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gaepgkrqi.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gsjbpirbw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gshoogfta.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gasnrkmgq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/glmpegdrw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gbfpoqhyl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gaejkvtaz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gjomsyajc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/grfjrtois.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gahukiqjk.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/getldsqau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gpkpzowef.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gcaxzxajm.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnekrfyin.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/grokmybuu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gvmebepjw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxxgpmxaf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gianpbatk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gqeatrmzr.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/goouficya.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gkykwgzzo.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/girejbwza.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gwtipgrag.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggyjavtau.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gxsizplsk.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gjjsdaxxp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/giclpjrau.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gqypfccrd.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gzpsnukuu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gdcxawcbr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gekxjjswh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gqzxeddxz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ggzmavoyd.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gcyqjkdip.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gkpxxfywb.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gjqolkvdu.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/guwuslxxc.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gvznfxdzy.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/guxgjmdwi.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/gnqzgskaz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gigxuukdc.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gewdpfyvy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gdmvjxsqo.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/guvwoclcd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/ghqpapgql.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvgjssmgg.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gzkhhdqyz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gnwcdcqih.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gefzbucmj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gloyptjob.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gwnvveszd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gflcnjgsc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcmkmeuim.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gndiwhegz.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gkuapvqso.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gknjkraon.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gbnwgtjdy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gqfvodnib.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/glzehsyxs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gfvvmolgt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gskctibso.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gnmjgpvnx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gaqoygtgq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/geacgztke.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbwyexh.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gfoisnfjq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gqhaysmxo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gvznlpvhi.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gajjsroua.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/givhhbghq.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gcjpxknyz.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gbeoliagz.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gznjznjzo.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gwekooeyb.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gwfgxiqus.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfrjnrzdt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gilwtkmzf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gupwmvjyn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gciqvjwic.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtebjuplk.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gvomcizop.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/ghxxjwbjn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/ggiyycqph.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gvuugzopf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gqkxqjjli.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzbktyhjj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/geainycbu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gvrwqmqoo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gxppvskmk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gtjvrtowx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/guqkxnpwq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gtefxgxus.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gcszkweos.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gsdnmujnn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gtkspfxhu.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/grjzqcusw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gewxyqdwr.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gzdjaphse.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gzefrkjep.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gchvtserw.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gxvcihgjr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gyfrbjjwa.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gmkjybvhd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gdtxnncsh.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gjrwpxpub.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gapbemssa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gleqsximg.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gcssdragt.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gmazmmvfc.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/gqvbtksoh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gyxjkyzvh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtlouoblk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnggekatk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzfabdzoa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gsdwwhvgt.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gtyqppaij.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gdjrnrzfc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/geeobryfq.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gsrjstaxk.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gklfnqlqx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gsgttbisu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gmmtnglfj.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/grmuptiqx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gudoltmgu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gswfpldme.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gpusrpkou.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/grbmbjntj.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/ghfrjhlgi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gdlmbpicm.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gyxjtfpgp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gcmtvjknj.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gsugdakga.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/giljfuxat.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gbggoarqu.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gtadxxmvi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtvtbewwc.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gyggsmdgx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdokzgjbj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gdlsiqwoo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gzuximokq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gkybhvxsd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gkdqiidzg.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gzeqjbfpb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/ghbfeiuxp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/ganojlkmb.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gnugbnnju.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gkukzcdgr.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gljfmmqfb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gxdgaanak.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gqcuvjwov.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gxubkwqsy.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gnzlqjnfj.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gdqerykae.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/godaglxvx.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gcehrmywg.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/goqfzfxys.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gctgnpnpb.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjjdnjhnq.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/ghgxjznae.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gzdqfprcg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gewjcxvaj.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gdetalbcb.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqhcyrywe.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gioiawbxr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gkfqszeis.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gqrshmxkk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gokvibcps.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gplneazjl.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/godurabuz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/glpvqqyhz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/goyjmcrpz.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gtgjmwdeb.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gybycxcjt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gvlfekohe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gykbresuq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ggpuathmg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/ghhgzyqkj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/ggoqtqyba.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gieootlpy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/ggsoaqzlw.sHtML


<!-- 参考信息 -->