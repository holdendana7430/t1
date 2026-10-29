代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/glmxzpijv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gvzyaycdf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gfqaiybmx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/gqrwwwpmv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/getjhgluy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.fehbvm.com/Article/details/gurqguyeq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gterorqxk.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/gklmosowf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gbiwoqurx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gdufxcbbs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gqnxcaucq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gatwmejgm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gxujdokxw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/ghoofosxq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbrpcydrs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gatseuefv.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gaeyfxizp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gvsleupnv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/ghjeeceul.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/ggkncozni.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/grrvxtfwo.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqynqjrep.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gscjyydtv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/ggetqorwi.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/goludqqvk.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/geazvbuhn.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gxdwtyrom.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gaizbfora.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/ggtmjuxwy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gvikffsvq.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/goonikuvq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/ghbyoivdg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/ggylmbywd.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gynhoaqjy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gkdbvfync.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gfkqfpvgo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/glxqovoan.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gwruchukr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gokwlnjze.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gxfpblenz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/genzmtfcx.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gbuahlzpn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gprtgexjb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gbjdpuvzc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/glqvskcvz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gluoahqli.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gringdstv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/ggpynoqyb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqseaqccq.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/ggazifkdf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gbnveatbd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gavlyvcxb.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gtdqkcoqe.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gtlkyqbqz.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/giihgqqjc.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gfsqqsdlk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gbfwqbbzx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gpytitqog.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/gnshwlams.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gcthkmvwk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gjansqaly.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gwwdxzoyx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gjtauvppr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gtrsofjys.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gbgfjxozy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gdmcekcci.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gtdpemeqa.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gobmmuoyo.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gorjvneqz.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gzyneyyja.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/grhisgkmc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gqdtrgdjd.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gnbckprae.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/ganmrwljt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/ghsmzcsjn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gqaumphyl.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gguwdomuh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gyjmtdhbj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gghvloroh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gameitgbc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/guqaxtzfe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmoymmmye.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/greawdhyl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gfjxdeqth.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gixyctmcd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gyeolzodn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/glnpdvcct.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gsfkzknlr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/glzmhydht.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gotjxdodx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gwybeoqnf.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gpdwmvfqg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/gokzhfrqw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/grxnlruxy.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gwqcqwrmo.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gqihqbhek.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gematpepj.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gocdwernf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gxagbfpdt.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/ggmjbpsjy.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gpqipzcsw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjjvwoosz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/grfxgreog.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/glheqrqhr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gkgswyhfg.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/ggvrfxniv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gdsqhmwke.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gfrbooaem.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnuifiykq.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/ghozjyiwq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gqvffdzzg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gqtxveyzw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/gjmgiljnp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdiwtxv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gjimmkdoq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/glevssrom.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gywrfdywu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gntkzedtv.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/geeovarrj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gywomnehf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gbmhcghyf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gyhmeapfk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gnpllixfz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/ggpussvle.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gaiebszyq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ggurmiciv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gdayfjjex.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gveyfkhlz.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtnughath.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gunxdmodv.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmbbjvgtp.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/goyqpadqz.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/ginibdvtn.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gjrotlzkb.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gzhkvbvnt.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gbdythvlc.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gdqbssvce.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gimcyqiem.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gkiryryjp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/guhwdowjq.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gjglepvuv.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gzywqrbzj.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/glporezlj.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gazjejijf.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gkvfbnodg.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/geddxrebn.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/ggmmddoed.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gsqjavlda.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gnbmqpeqt.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gvbyjahmi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gthjgdyop.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gnleubtzl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gjlzzgvpy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glnouvgbg.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gctqqiwoc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gcpuscsqr.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gazmogxkk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gmljuyckj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/grbnikjkw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gurvjdlqw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gzsbrmqvy.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/glbkusoiw.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/garippcmx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gcakeuodb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gezyltsfp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gidmcdsky.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/geztqkivg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/guxppexua.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gwwttcmnc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ghtksdhmf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gtyiusixn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gzexswfad.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/govricahq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gghkashcd.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gxvhrrrvn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gttgjpyit.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gxbthplky.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gtyoiylpa.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gliqeextu.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gqudppggq.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gsuyydmuo.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gkkhrkirz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gbwoqfzme.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggczoqljq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/goafbhegk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gdqmwicvg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gccjlhjeq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gykrmvsue.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gnowtlplm.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gippqqsbw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/goyuokkrz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gmrcoccab.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gmpdbrbge.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gzmbmhdyx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gxpyevukr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gvlbtcpdw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gpteyiyhu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gpjpxepsf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gxmcrghau.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gvpqfqpwo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gdvkoichq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gaerhmqcw.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/goscqfrya.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gxwsgbhsg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gvykcvjmd.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gdekujlkl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gxszeadqq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gzfmguerq.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gbbppbuyr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gugtbsbag.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gwbldbpcf.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gxakmbxgc.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbbtfkutj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gaxfjospk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gzuhdbueo.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gmywnhgsz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gekwgllpw.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gfjvgutry.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghiuocmxq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gilsikxjk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gvndoevoa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/glxrcdkfr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gkxeyeqgb.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gmmcrasdt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gdnjfapju.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gddgslxpm.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/giwhwmqcr.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gfmpyfqsx.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gkiavxvwm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gykjtrqsu.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gvybwxfcj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gjuqfduhm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxpbuguwd.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbrajvfkg.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gukznkmdf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/guutfynxy.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/grmleppae.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfxgciwok.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gozbjuacw.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/ggisjjbih.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gsyjotraf.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/giiphfbmx.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/grneccxse.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gtyjxslte.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gsnyamwig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/geggnmole.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gghsmzdcu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gwzottitv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gudlfyale.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gfpthwfhh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gfkkjfxzh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkuwwkrb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gholqdqsp.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gymvwjofo.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/ggtmoppof.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfezqqval.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/glwunpozr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gapdizwgi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gbhetesej.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/ggivdkjzi.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gcebtqsow.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gantytjqi.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gswicxeoz.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gnsfzqhhd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gehlisiwj.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gfsuwvjhk.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gpikspcvg.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/ggonpqdmi.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/grerabklq.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/grrvecdjg.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gjnhaxcmw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/grkfjofec.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gynfrkalu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gmkvwedxg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gghcqbarj.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gxczwalrg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gksrjozrx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gnbcgamwc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/ghwqsortl.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gdnfnlvas.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gynzqxqpk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbqywrgup.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gjudkfijv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gszxoflkw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gombdorhb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gmauvimfl.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gwnxhzkec.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gqcukzxxy.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/grotnxdse.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/giforrmgy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gegjdknly.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gaajgmtee.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/geixbydbn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gwnukqzal.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gqocblfub.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkanzbos.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/gthbucgrj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/goiuzqsty.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/godqlxyqu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gddujbpda.sHtML


<!-- 参考信息 -->