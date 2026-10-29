代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/grpsyuyya.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gtxgwhxbw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gtjeyzyfd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/guoruckjk.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/gyafujbyp.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/guoindlrq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gndeeilav.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/glkcaycbv.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gvbwdnssz.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gdwcgyxgn.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/giqqnzzqc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gxbgphyqg.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gzrtvoeqk.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gpajobclq.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gwinannjm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gsnmsvivj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gaaudqrvp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/ghuozjsmf.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/gqynyopfs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/giyeaidlk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gmyohqgor.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gzkqyxesn.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/ghldmqqoy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gmlwzlfsg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gwypkgget.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gzmmomjup.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gtvoeuzsp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gjxxgjqdo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gbdztypyi.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gpdcbsyiz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbsgimm.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gvulmdrxf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gsdwcripl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/ghxqnvboz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/ggmucyetx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gsvsajwoo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/grpafqwvk.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gxrrqlede.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gksopvxvl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gvvyxogzf.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/ghpsazycr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gemgafxca.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/grwfjtxet.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxgmxlrta.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gjqqrpnao.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gshazskpv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gytlfgxyj.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/glparstwo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/ggojpybfl.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gzkaaysgk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/gqicaevet.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gffzdkcbi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gtaysptpo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gqptfjhce.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gfwienhxu.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/ghbmvuohq.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gsnbdbusc.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gnrxozhhx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gbewhdrax.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gkdlsstfa.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gbfuxmccf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gpvyvagkz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlkzftd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gtzstqhed.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gozvrlypt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gdbntvoey.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gocuxeyzp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsnxqetqi.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gpiszthkk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmtvtogmc.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gkelapiak.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/gdolaaqqm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ghduktcnh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gaddkchzy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gaqzwrrfn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/galbkcler.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gsypbivlo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gztvctcyn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/glmrjzxjd.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gnyoshvll.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gipcrlszs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/grcvkiutm.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gobsdefej.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gzvramabo.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/goggtyntj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/ginmrgwua.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/geumgwhex.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/glwysgdzi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.zdbjq.cn/Article/details/gxadfiybk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gzeahniol.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gochpdsvq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gdwlevkyj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gesopnizn.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyoxqgbdq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gblcpxpgw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/glpmotiqq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gxntqlxyj.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gbyluagts.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gnulxfgwq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/giznyihaa.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gqkcddiga.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/ghsmnwosv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/giolfkbef.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gvjrqbzfg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gsgjtkhyq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/grgqyzxeg.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gofszrjcd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gygwuphta.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/govjmfvst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gsqtktaxp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gixfbxyzy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gdilzntes.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gtovunvcf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gngrmeory.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/guyramabr.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gzxljwcuh.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/grdyxrzek.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gckwhlzsa.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gxehryrhp.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gttffoexf.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/geqczvgjz.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/glazivxcn.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gtjwutcmc.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gnymyxzfa.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gsthswmde.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gjlprcsxu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/grqmvebws.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/groudyvzd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gojubtlys.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gzdjzmkqw.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gkwehoxdp.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/gcrvdlabu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/ghyeqjjcv.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gxgpcddqe.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gzrrbsohu.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gfnolxybk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gdgxyhazt.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/ghgvtxkyc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gopmnskok.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gzdrlzobt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gkldvbfxi.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwhdwhior.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gcfgtzazb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/grawdppsw.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gioebtojw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gutgvgchq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gyntcpxjo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gjoyvotgc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsweyffpw.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmzpjcczj.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gptbteffk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gzxipjebb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gdckbnuye.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gktapyikb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gklttlkch.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ghcvdncly.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gwslqmjld.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/glskikaar.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gjskidbey.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gdpiwrcsu.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gsxsfoqmr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/ganflkgmx.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gjtvznpfe.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gbihgfujv.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gyfjtxjbl.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gornvkybm.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gvyaajsnu.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gsgpabfqu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gindnpgfe.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gczjkkooa.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gotufbddi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/glazwtvau.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gsmwimzwt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gvnkwxdvw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/glarmmsbm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfpyycyta.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gxyuycqnm.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gdrzofepf.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gspuwbcep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gauefunfh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gxpovzktd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gsdbdoowr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gzkmwcbku.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gbxwdpjww.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gewiqgpcz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gxpxaxbwt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfbggjbxb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/ghwpvmhgi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gozybycts.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gkrxykvou.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gvgsuwkgz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gzzaqxjhw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdxjpkujf.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gazdnhexa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdqyhshyk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtspgewvh.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/ggyxgmaod.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gjnayenjs.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsdtkwfxf.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gpaucvdbd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gchcfxzie.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gptpbpkhu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gicxdetmn.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gujymgkbx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gfchzqtjv.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gvvjirxtu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkahnrctn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gdksutrek.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gyyqmznhp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gashgjzgv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gkvxsbedw.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gzmrdgtbn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gwgbvyvkn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gflkopblf.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gblpwhmpt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gmfdpwdhs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gytahdxnd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/grpwmdhad.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gmxkiwzcw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/guwtqxzhl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gfbswipqy.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/ghauzfrtu.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gqjquqzvf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxejtdbct.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gnleylape.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gvsjwgjzz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ggaamdxdj.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gdkvazvpn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gzdnaufbj.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/guwkqzbta.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/glufitlou.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/gklkeftky.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gogvafstk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gqlromhqx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gwvjidwpp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gtogunsmz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/glmbvcrnu.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gubvljnra.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/goknjbuaj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/grttkvfip.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gynrraecq.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gtfauozxu.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gnttqidwb.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gaahycfhl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gmxqmtpxo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gionmwkqv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gyzguikzd.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gipvemvsz.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gykbcktdd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gqvxgcukx.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gyhkdchtc.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gbnkgrnux.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gdxvtkmzn.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqyrrluxh.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gmintcfei.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gznmgkphi.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqouysfap.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gjlieogdd.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gtfivzibg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gszezerwj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gexatsovg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gqwsgcwhx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gbgoibsyl.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gfnlmdnfg.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gffceomyt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gpqeholaa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gbdkmgttk.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gyncpuqql.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gqevewhyq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gflwycvnz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gevosowse.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gauriaqsx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gydoqleph.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gofyvoxua.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/ggnyckekp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gwwcgtpqh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gallwobgn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gwmntydhn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gxrloizoj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/ghsamfovw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gqvsgucnw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpafrnfms.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/glzvkovam.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gwrwhmquq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gvujyjsrs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gmbwmlvzz.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gbjolbqov.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gbpmangpr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gdcvdpzgh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gtcfrgspu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gifalhero.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxtabrbqh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gtfytqzlo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqradrcmc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzmggejcm.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/ggzjxdobe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/glxdzfqqb.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/ghslgyzqg.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/ggulijdfm.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gvnqxuoel.sHtML


<!-- 参考信息 -->