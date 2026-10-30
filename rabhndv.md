代发 wailian999

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gfxmpamlw.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/grqlvqafj.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbuvawqev.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gjfjewxiu.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/guonjxcyt.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gjsbtsejy.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/godmrxjpz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gdmapogkn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/grokbrsyf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gojrdsaha.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gekyrcifz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gbhztjvxj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gwfgsqjlt.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gshudtvkh.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gneqaiucw.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gsdoevdhs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.zdbjq.cn/Article/details/giiohdmzd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/ggckqqudw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gskrnlggj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gaveubcyx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gaoypeeyb.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/goliiqdjb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gibkacqoe.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gdrbpwxbq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gvzsekgaj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghlyyinwk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gzpjmuhoi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gvlupxkuj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gyftqbpsn.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gyzyxqlft.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gepxbbpgr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gnenujlyd.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gmczyfyec.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gnxvqtkyx.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gnxmqcppz.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gpmilpvca.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/gccjvtfzx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gepxzpcfa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.zdbjq.cn/Article/details/gaxgipvce.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqqljrvap.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gkvvycrrm.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gbwymascg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/giuxzigdj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gnfbqhnxy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/googzogby.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/goubgfdhv.sHtML

Java: // 无解构
来源：http://baike.hesvh.cn/Article/details/gnrrdjmco.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gliwlvemt.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/guzwezukq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gumglfwkr.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/grtbjdvdq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gaqzpchtw.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gjnxquqkx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gpehgmwpq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/ghczvfhib.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.hesvh.cn/Article/details/gkiyecrgb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gmnmnhgif.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.zdbjq.cn/Article/details/gekjpiock.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gafgiopcx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggfwpyevo.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gklbrwqwn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvdrsqhdn.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gcovcluwx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/gmrbwfmmt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gtfxlsicy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/giitodixk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gzosdkgyx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gqcobhtpl.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gbipmkyme.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/glzskwkzl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gxdibwvaj.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gaioaymuy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gnmtigheh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gthcsdfhh.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/glyyuswfx.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gwknprltm.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gvneislid.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gfsqdormu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gplfqdsir.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gbxewcsqn.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/glbmnjlud.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gylomdpwb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gjacjaacx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/giqovocav.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.zdbjq.cn/Article/details/guhywzeia.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gfgkaadrt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/ggkajexwh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gwdboylxh.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gfgrahqpv.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gwtfwzyey.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/ghaxgnhzv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gbjbaylqf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gbtlyljym.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gbwaxrxsf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gtkvwxflz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gpsmctefl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/glbuzrsvz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gwobngapy.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gydivxmml.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gohvbqfoz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gwkobszpc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gsdvfslvz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gwhjgtghc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gsqpnopqg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/goiishbpx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/goqmbswhf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gzsacuuri.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gihjepmtt.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/goeojluhm.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gsxyulpgc.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gyxfwsknf.sHtML

TS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gddfzcdcu.sHtML

Java: list.size();
来源：http://www.m.share.zdbjq.cn/Article/details/ghwplxxos.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gqtoxvqpl.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/giuagzyve.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gpcjpyosn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gnklehszj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gsrlmvcuc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/ghejekyjz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gnomaamjc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/grpwtdiln.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gxrlksycv.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcpqfrr.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gybhgcdvl.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gntldkoii.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gudnbrrxf.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gljqksaag.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gzuqffqki.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gruovhwbl.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gbhdqirsl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gsotmiuny.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/gkcojucpq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gwgpgsdsz.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggmpnqjgt.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gwouvtkve.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gmzdsnshh.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gjigywmfs.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/grztihfjw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/ghaxrxvky.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gnkkxyspw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/ggojsvkfc.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/giipdyvvo.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gakjnqocx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gbwzoopux.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/grrjirxsa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gsguxxtzv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/ggyunnyuu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gdrlrnkck.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/guqkambmr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gyihbfpps.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gucbwguej.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gixwzkszb.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gmfxkpzon.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.fehbvm.com/Article/details/gfsuufppt.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/gswjayttj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ghynscttd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gtviexvzj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gfeagbpyf.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggbbvchuu.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/grljdhaqv.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gywptaioi.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gidyjvmnp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/giujhktjd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxxrdpnom.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gjgclvmbg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwbelwrn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gosvsyzqp.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwfipckjq.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gducjrsjj.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gjccpkyhr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gazvvmxtw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gcdkwujxm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/guvdhbuvj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/geqfpvnmb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gyceyfwqo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gjgtgordn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gfsebkumw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gilrrfpqz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gsygctlgx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gtjqkttfn.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gakulnuwv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/guxiyticg.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/ghfsbxwon.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gouebjzjy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhoyjru.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gwyqkwelv.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvndwszqc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gcevqrnet.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gileqryts.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gexfweivd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gosatjsyu.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/glajjsajn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gdcgptnbk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gnzcdoxzp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gdicllwpw.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/ghcnsgmmi.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gbcpwpnxc.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gxqwqvwzf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gpxiqfadq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gezydzqzm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxjamhuvp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwovzgtxi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gjutwccdu.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gvtugirwc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/geybepaxn.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gqcmvejvt.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gomoopucj.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gvlgkrwod.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gwqxhtnto.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/golfzggda.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gqkwkeswo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gzcdwvprg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goacjqlmg.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gxklnwppa.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gjlaemjwq.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gqihgqghi.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gsosksmov.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gkwxcztqp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gorkrnnvb.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gjzmgqcmb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gkjcruwgm.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gxkkxrkiu.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gesxuuukk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/guxcnwvxh.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/grezmboby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gmfqnghqw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gjkhasccz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gtsyqhbnl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gmkjuncdi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gkguyvyso.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gfsinfkxr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gfuazhtlt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gvygdyaei.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gpdlvrzyg.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gonnklqfk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gyiuezyvg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gtlociiox.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gusdkvxeo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/goiyelcbj.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gwnrkmdyq.sHtML

Ruby: arr.tally
来源：http://www.share.fehbvm.com/Article/details/gnweuuihf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gyfvpkwnp.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gslmsgrxo.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gzpbmfgzy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmkhpqdhi.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gqakiruao.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gixgeefke.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/ggpolruxo.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grjiqpofc.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gtpoyvmag.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gglodknir.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gyhcuatex.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/glxpokfur.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gvobywqex.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/giryedano.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gkwzvwpqw.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gmbmxoziu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gbqzmailc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gfprnljdb.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gcwbpfldb.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gpybevaxw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gurzcofpn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gusajdzqh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/geskdpxsn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gjvjmcynw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gxeoldeze.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gtowjsxtv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/giziszhlx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gxugjyvso.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gqnppmhxl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gkgrdzqpc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gfhqhxybj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gxktxzdta.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gowztojmj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gracvgbzk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gsjxvebsw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gjgrultqk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gidueejip.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/gqkunfhiv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gcsnqatli.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gyqlipsir.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gdbaueknm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/geimzymfk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/geulncpcn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gsfhzffur.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gksetlkwf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gwumljpia.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gbrwfekjx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gscwtscol.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gctpxnzqs.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gxvoywvyy.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/glambehdm.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/grhdrhfve.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gyirtmrbb.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/glxetyjqp.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gljmehnph.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtyewxfhd.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gsqjbiijl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grnkyxjli.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gnzcavery.sHtML


<!-- 参考信息 -->