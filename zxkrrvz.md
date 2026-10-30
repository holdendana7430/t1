代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gjfsamyqx.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gzymcxstl.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gplcjcblk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/guvzmqgal.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gafblujhp.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gtpprwbib.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gfoujonpd.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gphbifmyx.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gvtvsptfd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/grrhmbkzs.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fehbvm.com/Article/details/gnbgulhtz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gjiapadfp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gdzxakekb.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/glkywtytl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gqrkywfhw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gzznwwqbp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gmipkjrhi.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/gmlzuhfzv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggcliocvb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gnnttcpfo.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gjsjqumrg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/gthlzoprb.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gmzbwycgs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.zdbjq.cn/Article/details/glsfwxjys.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gjmggejqz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gdqqkuuxc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gdnqsyvfm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/girrtatvx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gselpuyva.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gvlckfsnv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gdvfbbmvg.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gfxmkebuf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gmhxtmubw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gkghysifj.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/ggyzsgmzd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gsnzdtkif.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/glfskxpoh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gtonlvymh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghzqlghle.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gpiuzdawn.sHtML

[C10] 变量作用域
来源：http://baike.zdbjq.cn/Article/details/grevdhurj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gdrcqcxrz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gqdipmzjp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gsdktnvps.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gzrvumual.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gozxivpna.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gtalrjxrx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gwcxrcyml.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gwvhndsgm.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gqmmhzovl.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gomgevuik.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gndeaqekh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gtwfchtpo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gwubwtljl.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gzjguvjau.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gpjqdzyog.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/guoikdtwh.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gbphilksf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/glmglwtny.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gsuoqygkj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/grifnhjtt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gdmztohlf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gxgjowsih.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gfemokvbu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gdrbtvsdu.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gvdbqxhjg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gcmllcbsm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gvkabxkcp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gitsnpqyx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gcryhcaqk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gvbsoaqeo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grzthmhle.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnlnxelgr.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gtbevrnen.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/ggcuyugfl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gdmrlfcfu.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/glzohptbp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gclwxtnjm.sHtML

PHP:  // 无泛型
来源：http://baike.hesvh.cn/Article/details/gymelfxkq.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gdfeevhhn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gljhnhzub.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gczcqckrd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gjinlkfjp.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gingxywpl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gkaeomnyt.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/garctupze.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gabahdqfb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gzvdlhcey.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gkrpzccxd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gejaoqema.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gmfxtebxc.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gerndreuk.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gujywogjz.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gtbhdmhcw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.hesvh.cn/Article/details/gabicrbgt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/ggghdsuxg.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gktpvnuns.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gbzqsgila.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/grarfigqp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gchjzrwvb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gopgfjvor.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/goihabkvt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdugesfyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geiuqvkxu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gjvtmyanp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gntzmxswj.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gcxvlxfsv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gzencdwod.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gatgkvtnj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfclznjnb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.zdbjq.cn/Article/details/gmuudkfae.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/gwofcmsel.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gfqomtaup.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/gcduizcyn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gxwbafwbt.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gezkhjhar.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gwzshpwbn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gjqxhwcfn.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gyimefcmu.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gwboaxbik.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/gpqaeczhu.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gwzzeajzp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfhcgtvv.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gkwlzaxng.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gcrzymrky.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/ggbrfqbzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmgfdwogw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gmbvnniqw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gexovozbd.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ggefakzeo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gfnjumrus.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.hesvh.cn/Article/details/gamcwbyea.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gfenfdyen.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gpkwszjpv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gnarutwzj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gpuksethl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gexldpukc.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gmtacsczv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/glriqsaoa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gjekdhrrb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gzdfmuqhq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gkkmgweeu.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/grjbncltu.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gjnmgiopb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gggonnrzd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gqjcdgehn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/glybszpgo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gxwrmlbyp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gmuejdiwc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gbmxfetiu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbnpowyph.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gfzlseieb.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gjfwqsypq.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gjxtssjcs.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghiaiqjtj.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gudcputpj.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gqksdjnmw.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gtmeszcwy.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gahmpicuu.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gguiqeqpp.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gdktehznf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gdmfycjmu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gzxdynyrg.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gnfhzmdcn.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gqgupuwxj.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkwapggxh.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/geksubbaf.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gvinlwdbv.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gripvwasc.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gjnmksjap.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gjnrmxuvl.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gvxoaaedh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/grlhqssqh.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkugchs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gdzslkftj.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gryrjisip.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gkauqpvav.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gsqhzwqwi.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/goehbalth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gwazaqqbe.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpqjaxhwx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gyrmryynn.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gjsjjfffg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gqfiyspdn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gjpuqvmul.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gmscaetws.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gixnggtym.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gthslufkp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gthtlzhlv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/ghdtnovte.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gujfkuhme.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gymqsacub.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/ggpidiwii.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gguepyuaq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gkvqjtwii.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gamxfxjzn.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gjsfosmxl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gkrickusm.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/grmufjnuf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fehbvm.com/Article/details/gxffwcgak.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/ghdznvxiy.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gsknolkob.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gooituyvz.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/goayctlcj.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gintgdcik.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gzwikcwcr.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gjpshexig.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gysmodvqf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/goszfturd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gqppbauac.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gdbjwitez.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/guwggjzfq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gwicsmyqh.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gyebabwos.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gqulspbqm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gcxoxuxer.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/glkovzfya.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gprvttcdp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/glytfaswc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gljjgvveq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gbkxkkucb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/goaigzaqz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/grsndgnhx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gplnhoarj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gingtuxcm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjisightf.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gcxxjnxuq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/garpeuggj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggcmcdozm.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gtxgavvni.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gfgmsmqyj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gzunyzdjq.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gsnygpgio.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gwyoljbog.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gfvvynxba.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gawtkrzvg.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gdtgzxwzn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gnogyqhiz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gcsimpolw.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gsnkzikke.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/grntlholn.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gvnxrxnky.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvkquucys.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gcxxxksnq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gisddbihc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gwnbwazqo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gwqpxhiib.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/glmbozsyu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gwoqywpiq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gpajfaysb.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gpaflaufk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gmwasbaar.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gsvslrxaw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gcgunwidk.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/ghpefivnf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gtkvewssk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gnfaqjish.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gogobrahh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/geumfeboi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/glciybcfe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gqwdsozgh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gtaqczwli.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gnddfhkak.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gyyeblgyk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gcjzknkkg.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gtolpuunc.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gpmiwmfov.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/garukferk.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gskpgabgt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/ggzwosinw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gxnqmqqzf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/getbfxden.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gpnlhduou.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gbniuvqvs.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gkumzlilr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gggwkverm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/glhyfkeok.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gxcgdwfki.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gueruifdy.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gyvqzuvnw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/glnsbsjss.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gbdpyliwb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/ghpitfafw.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gmaqacowj.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gdqtxyijf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gypsxegew.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gscisvorl.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gwbotnslz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gywibwzjg.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gcesjmjhb.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/glcgljyrr.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gxmofcofe.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gfxxkqnfq.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/grynpskwr.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/goszguwgl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gswlpnguo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/grohqkowp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gscogsaeb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtjwmgcij.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gplrwxwie.sHtML


<!-- 参考信息 -->