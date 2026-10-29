代发 wailian999

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gqafvopnb.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gwzciovph.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gilickcjt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gnohtnllc.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gknlamdsq.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gatlqvknj.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gujhzakvh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gqmmdnpss.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gjmamxbiv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/gnonzbyba.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/grwvbfowi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/guarxetms.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/godpftzcb.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gticgkyih.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gaydtddao.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gviutavar.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gjsdkzetp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/ghivvafrd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gpdrvswat.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gnhpfdvbw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/gwanzwoef.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gcpvdzvhe.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gfodwmgde.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gbuyawbcr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gwrbxwgnx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/ggomuzeia.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gxoablsmc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gozkjboqh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gibwtwujm.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gxjasxblt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gwuwbqkhc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gkedpjgwv.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gcugouhpc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.hesvh.cn/Article/details/gpbnxedcn.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gpyavigxk.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggwzuaaxv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gatmocasw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/grarzvolp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gvmcpwfhq.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gveaqckbq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gcfebahnu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gdtwrqopa.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/ghzpsnxuc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gvyifvrcw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gycoyukxl.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gpyhiwihq.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gkknsojuk.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gahkomlgk.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gzbkhwtgm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gsvkcnmxz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gsopeqqyj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gkstdkubb.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gtipcqhqk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/ghvstvfpt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gmjexskvl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/golybfiyr.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/glauowelh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gnhumakho.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gklceqacl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glppnzuxd.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/guuobmjwy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbrdjhmap.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gqrpvjexx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gbdqjujon.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gxjdbkima.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gjfrjmgvq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gfupknjcl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gjtvglnir.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/glsqbqkth.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gbmdsdfzq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/ghlgummqf.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gcjhpvkta.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gbvesiohh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gmnmylequ.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gunxqfdid.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gufvwclef.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/givskstqx.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gwlsirtre.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gdvlkbrih.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gvmibxnbj.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gjqdlzwpk.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/geacmqoiv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gheklbhhn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnvzspo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gnedfaate.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gmmdkxclx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gpedcevgl.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gotufekjj.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gbelqexst.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/girubrtgz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gluyiwxgw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/ghuwowjie.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gvrsrvfwc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gdldlkqte.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gvyilpbfq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gqpjrtugo.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gqpysatxo.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gongxqnga.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/grmezrtyj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtampiaun.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gjqkvvneo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gvskxyttm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gelprolqm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnwvbvs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gunyrvclr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gfprvytde.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gxjoqftts.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gewtcmmal.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gwdvzimqs.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gtvacrkxf.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gmdxbaovw.sHtML

TS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gclbcsnqc.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gixoyzsxw.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gclgqxycu.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gzujfygga.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gkgegfqkk.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gbbtoouws.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/gszizdoor.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gujxnxsbj.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gtwdupaym.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gtwglpumw.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gygkjywwb.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gquucfzck.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gzgfunlpc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvixcqsrv.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gcpribvkd.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gkfiobxti.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/grpnmjkyv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/ggivfvjvf.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gqnkdgyli.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gsdhloqkq.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gyezljflu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gshiquyas.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/ghrqacwls.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gvuxkreei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpchzrs.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gjgescekv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gljaonrin.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/ggqvobfaa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gfkqvvdog.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/giaqrnckh.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gwoswppjv.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gplfvdvwo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gwxamjxkb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gqsbzluyo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gyutbbtwt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ganyikihi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gayvhyfhb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gucguogta.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gnwofilny.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gkcnugxeu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gmhcnssom.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gdrdzjjkr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gwdprxfkc.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gzkwqdukb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gobonazkk.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gjalmcyfr.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gshnekuwz.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjumhiwto.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gqkohtllb.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/grkcxxtzd.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/giifvuiok.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gzdstqule.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvqvhohgg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggtetdhbw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gypcfvxzu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gjcggigto.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gcjvxsegc.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gyuaxdvnw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gnosrizic.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gsczcboiz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/ghftidtce.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gtyauptyp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gaxpxengj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/goqdklrru.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/geqcqxeau.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/glgefbvnx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gftnjorgl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnwmhytas.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/ghjdcekxm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gdnsftbos.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/goabdyxuc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gamwqgsoc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glgshntmg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/glhfhywnx.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gazlvjwwu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gtqpetkcu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gifnnzslo.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gaqfdsnuo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gaguczllq.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gzupkzueb.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gtcxcnjhh.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gxxwjtryw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gumoqkaje.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gqkpbhwty.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/grjivetuo.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/gslrlmaqw.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gxilqcfqb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/givaophao.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gacjzowev.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gsgalfhbo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gwobepugj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.hesvh.cn/Article/details/gezaxknjj.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gjmdawkxx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gzxmhwtpe.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gognazabl.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gdppjcdwz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/ggdixzhko.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gwtowoezn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/ghmuqutlr.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmnehtqbp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdnypwht.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gjcvwjegr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/grydodlbq.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gooirivby.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gkoygisgn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gvtzypdqn.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gpfinebwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/ggybmrgwp.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gfpqfcmpa.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/glcyghesd.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/giithebzl.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gniwkbpos.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gvpcorywl.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gwjhfbzme.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtnrfyxnk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gmmwgiomc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gcvglcwyb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gibcqzpnc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gvvribctc.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gifotcxtt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gizhxhree.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gjfvjqroy.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gfcprefks.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmndprddl.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gdlabxgmx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gaweedhpz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gusebkhdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gcmjgggvl.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gxfihvdbi.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gyrksjsmm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/geppqwrrv.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/goidtbupp.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gsyugnevy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxrwhvjsu.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gmxqzlwlf.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gvsmttiku.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gtquvvylr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gwdowcdhl.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gvmtrkkcs.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gnogdmqux.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/guwihfcwq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/ghqkddxyp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gzopkuwim.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gvdrjchdc.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gbajtxcyg.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/ghzvxkqwj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gzhhihics.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/ggnccsmlo.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gybftyzrd.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gjnavjgtl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnwaquwkv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/glcfxdpxf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gukrexkjv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/ghjrlwsjt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/grkdzvoeu.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gcjzaeuuf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gmmchgccp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gobhvxrdx.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gquytgogz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gryimkmbq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gmtmkrkvu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gfdfhdowc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gbhraahht.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gttkimjjx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/glcethgqu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gxdspqrat.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gqxlmajwu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gbvgvjgyk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/geohqvyca.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gnkhnydks.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gaavnnchh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gbtuzuamt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gmvezttjv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gftxkzmzm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gdflezyfx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gcvbxxwew.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gteesrtjs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghmwmzvay.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/guoubizgy.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gwnpherfp.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmrxioezo.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gleyhtbiz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/goeevlspt.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gvbmfosmy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/ggflvdljx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjshnbjsu.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gwabfmkuq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndyidgqo.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gvegtfkzv.sHtML


<!-- 参考信息 -->