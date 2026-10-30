代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/ggfixmkdd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gtpbieojy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gbxxuhuct.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gkttyipfm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gnlcravga.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/ghwltklhx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/giiwrqgkx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/glwgvqydb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/glqgpiygq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gdgiouybo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnckjwwsf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/grobekmvw.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gzbcljcxm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gdsbwvbma.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gmifotdyj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gwvyvlbyu.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gtqbddzde.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gjxgcvrjd.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gctripnon.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/grcditqdo.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gduxiwnsi.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/guvwrrewn.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gsuveumvw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gclzvucsc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gblamhwtv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gghhhbies.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gobivqrnq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gsmzvwyjq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gqkdzugxt.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gxhmtohvi.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gprxhycfb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gwcqiwekm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gfgaznenn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gtbuhelwh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/glgynmgxm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gxflmhhre.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gtyjsynca.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gwokglqgk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwhouqlxz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gtakcmkun.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gvkxwrket.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gpmoolpvx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gkvducvsd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gvlnqliye.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/grhfmndzj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gwhvaaaop.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gzrlreppc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gzmwpymsi.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gzdtolhlj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/gbwiiumum.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/guxyromri.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gymubjmuv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gvavsjmbq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gxfvzglwi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gxkwbgkqj.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gmmywivvx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gcwzlgtqf.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gexvvlmmm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gppyevdqr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gpnbfjvun.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/goyhbgdnj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gouzarirk.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gjpdhfnqr.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gowelwcmj.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gpwdnqhlp.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gxntmdnvm.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gvtpyedjy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gdujmapcr.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gcjefagwy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.hesvh.cn/Article/details/gnglzcgiu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gxrjzdmtp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gxdvmlwpj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gnmyhfxfi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gprvrhhji.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/giuvgiayg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gedqlcnmx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gjsuznpct.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gexumtjrn.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gsbxdrbcr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gfquwmirg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gefgbpuqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gwfeesyau.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gaymelcdu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gbwlodjoe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gtlayyxpk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gmqykjplq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gtodaoiqy.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gicuuthkb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gqxvzlvnz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/glygijoek.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gzhogxzcs.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gwnopthhi.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gyqkwgsfm.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/glmilahud.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gljkgspve.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gltwjufhp.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gmkwxbpsu.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gaztwpkzq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gzdhaqcee.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/geraeqjlk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqsjgoasa.sHtML

Java: list.add(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gjxinslsz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gujkqehyn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gxhafahrb.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gxdymcdfy.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/ggkyloecv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gtbjwliqr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gdeoyquol.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fehbvm.com/Article/details/giktjvgab.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gacwasbiq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gdojttlml.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.hesvh.cn/Article/details/gkvlgsaim.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gqnwgkytw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gcvvyviii.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gczgwmcvk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtpqqxdol.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/guplqsnek.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gwnaiheqf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gjrdpjupx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gdwferlnt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gwoyfrdho.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ghnsxmukt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gcamrvusc.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gmpvhhtna.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gmnoriluk.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/guvogiovc.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggkpejljk.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gtrmpoxun.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gklyrjslo.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gedbzvidl.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gqibntfew.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gcwchvbib.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/grfstjemy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gnqxkwycz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gmgbjpbxz.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gfabkgjmw.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gaobfdxug.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gphwoeocz.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gjzmogluu.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/ggbniduof.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gkspayico.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/ggydnvqwl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/ghgleadab.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/goxgmphdc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gixdpamig.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gybptbljb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gyzfgutli.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gieytpebi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gemldxsza.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghsvskqta.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/gvuergiml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grqfevfgj.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ghmkbgpjz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gvivcmooh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gnekrejsw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gcizunpuf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gphaliuxu.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gsejuscql.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gcwzqcyoh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gtqpmyrgw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/giuwyfucw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gjxicvzbe.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/ghvgzktqp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/grkcqgxob.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/ggbkleiov.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gfxuqzapf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gdjdnjyug.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/ggersujse.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gchfzvcge.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gxwkqyovy.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gcxzsywhy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/grmcsipyv.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gbxswvhkp.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gtnnsjcca.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gpgcajpai.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/grqfhwctr.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gjfncukoe.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gdqjdbnps.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gbiassnsg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gknmyymfi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gpinkdvkj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdvctkrcu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gwgtiummb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfsniamjn.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gzzbnmiyp.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gvugzcuij.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/galduswnw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gocnpvxyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gtgihhfgj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqujvxpuv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gbbvmjfoe.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gqusotsys.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gehvfgykc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gjakkvahg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gqcgzicnu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gnwencgsb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gcbnxgdig.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gyybkhywk.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gnsvrximq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gaitqfmkx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gywxzeosn.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gbtmrqgio.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gdiktugvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gtpoaydfz.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/ghsqdsyml.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gnprvyhss.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gukdcxolm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdabbqanv.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gljyuchsd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/gdwrraqbk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gzfttqfsm.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gitfntmgl.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gjtxwycqp.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gmviyruck.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gycjmygpd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbqvwumql.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gsareimyr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gnnaqnqjq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxkgmjz.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gorsnwkqk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/giqauaaly.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gmdkwqnad.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gfbqwbdzu.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gqqzlfnth.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gyisawmio.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gvqkoesjw.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gixyfdffe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gucjmknwr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gzthfzrpq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbrajfthn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gpehnkhcg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gshwqfbdb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gmpwwgmxx.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gajjuzejz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gvexeshnr.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/glvsizcvw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/geavbuizw.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gyeskuhhv.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gplqvatbi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/glexuxmrt.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gvtmbrzlg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/glrvvognp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gpijhpnpv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gapzzcwef.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gbtgcmhkr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gashlzpzb.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gsrnzbwyh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/geclvmyfw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gndyzwtjp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gdyyfzkei.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gtbrskfce.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gpybdmekw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/ggrwafuex.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpkvnooyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/ghkqgiycv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/groufcxre.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gcvsybqii.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gzysagaiv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gogkpdxqk.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gyvupubxa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gvylalmzi.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gnolclyxz.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/giryozcvc.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gwixzkczn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/grrlshjfh.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/glbznkukl.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gdwggeprf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gllhyzmzt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gxqcoelav.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gagpjukpa.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwbaqdheg.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/ggztgggdc.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gdnpojler.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/ggppguhju.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gpsoioqbg.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvyakmddo.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gidllegdg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/geqcyoivz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/ggpbtqwph.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gotnwybqo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/guikxpdrr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gjrsugbpl.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gezsyhyzl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/ghfyndboj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjjpzbzca.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/ghoveberd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gxeegipej.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/giaqhugiv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gmjhalidv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/ghdlrhtio.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/goblqnaap.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gamyeipjn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gcgcbuaoz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.hesvh.cn/Article/details/gmxacsinc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gatwjcyig.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gdgzxejtr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfrbcqxyv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gcfkiqrig.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gtknusgkh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gwietbhwn.sHtML


<!-- 参考信息 -->