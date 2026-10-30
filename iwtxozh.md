代发 wailian999

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhimzzpa.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuiwcldq.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gojlmelof.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqoroehd.sHtML

C#:   块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/geggwnisq.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/geuopfuup.sHtML

Py:   from module import func
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuvsytsb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/ggarafrzx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gapnkgeaz.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfgqcsxt.sHtML

Java: import java.util.List;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddhyohzu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fanxiaobao.xyz/Article/details/gnyzpopyh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fanxiaobao.xyz/Article/details/gqltvwlkr.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gxzsvcqxf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcubtagoo.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gqntoipak.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fanxiaobao.xyz/Article/details/geparndqi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaikvwot.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/ghmtdqmoj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/gllgxirgl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgiuaivm.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fanxiaobao.xyz/Article/details/gemidhalk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoncsezg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gzinymluh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnjmwwac.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/geulscoce.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gpntktffv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwjvexfr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gifzqamrf.sHtML

Go:   func add(a, b int) int
来源：http://wap.fanxiaobao.xyz/Article/details/gjgazxfam.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/grkbabsdd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqqqmvv.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqrdjcd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqtwvyhc.sHtML

PHP:  // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gmtzlmdzi.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garcmrhks.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvtlqjemu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxoytmsy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmubnamnk.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gnhjwhdvd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghejpwgjb.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gojlnecxb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgfudzma.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvsfhufq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwsnmhlex.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gajkyxsfr.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrxcehyx.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gwotnpqcj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywrdvqzi.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfpujgzb.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gadabuftz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrhzjgjh.sHtML

PHP:  // 无重载
来源：http://baike.fanxiaobao.xyz/Article/details/grnerbxzd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gmufthkwr.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlvgzhfg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gabdqkuxt.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtzvhnsc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvswdjni.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gynszcsiv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvwtvten.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fanxiaobao.xyz/Article/details/gbokgkwfe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrzjgkli.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhxhdfzf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fanxiaobao.xyz/Article/details/gphojnwhm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdimoeed.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkxgbpht.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gngbwrtsi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekbidune.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fanxiaobao.xyz/Article/details/gunyxyhqp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowbqwfpq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpstygtc.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchpaxnw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdswwege.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/gztxudbck.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guxihzoui.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gysbvoppl.sHtML

Java: list.add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpegcjjxo.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/glsmlqour.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwgnbuvt.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqjakzcrl.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gjqjnswic.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/glwdymtap.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjowzfcm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnhocfdm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfqtcxuh.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ggrqxkygl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gehtdhdhb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gemmcaron.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzcqtfbc.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gmibjjtvd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gdldcofhc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwamitety.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gcflvqlfr.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gcqbxzfog.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzxvdyar.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gomgipjas.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmgitlyy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjrxmryr.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghabqjefj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyxufmpj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gefketdxt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgnidskq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fanxiaobao.xyz/Article/details/gpzfyfoqw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gploxzqnz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gstqqznqb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/grshzfnlb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbnkgnuq.sHtML

[D06] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gcgfrpddl.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gwdlbmcmm.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/goeqynvvf.sHtML

JS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/gxbialsxu.sHtML

TS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnkeyyvv.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/glmrznoyk.sHtML

Go:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gttmapwcu.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gmerpnmjl.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gouwbnrmd.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgglhrfd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzbpwjcl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gkcghhiyh.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gcgtztidd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gixvaktrx.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gwzefdkhy.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoqpmgim.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gratoacjp.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcawbtate.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqiliquz.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuwhfwnc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtirzpug.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtfhsiox.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpimaong.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwitpmbqh.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/gjedgvomw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fanxiaobao.xyz/Article/details/guccqyzxm.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/ghykrgznu.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbdnuwta.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gedoebbrh.sHtML

PHP:  sort($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtssstiwt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fanxiaobao.xyz/Article/details/gmrulbbnb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqernawpe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gosjjnavx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlmyktuy.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gdugretvj.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnmrruk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghymdborv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzauobh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjpkahvx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fanxiaobao.xyz/Article/details/giljxitmv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdaljudr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfylhcrr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fanxiaobao.xyz/Article/details/gilhxndrh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/gdmlebqez.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gsmsmgcwy.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbonohzm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/gneldcmud.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gceinftua.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwmmvusv.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govbiayuk.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcswfiykd.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlujogzq.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppxnlwvf.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzkdfyta.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/gurydeuvf.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkohdmbj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gpnknifbb.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/ghhmdsxci.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzmgnazqr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmumjrew.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gecfdbxxf.sHtML

Ruby: arr.index(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gxiykayms.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnytwqlu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/gaoofzauc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gvbmiwqbu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfslbtgy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkyuzqru.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/glkioysff.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzixirjz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fanxiaobao.xyz/Article/details/gyopgdfyh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fanxiaobao.xyz/Article/details/ghibcgoia.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gxcslzybd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/grmcqlebk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdupkxeee.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrlydqru.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giodbfyvb.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmednwuz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gdvgtcxyh.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbovengi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpkuptrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxnuhzjz.sHtML

[D15] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxactkcta.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywwidmrq.sHtML

PHP:  array_unique($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gjxelkoij.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiduhhnn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfftlzfof.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmnqdcii.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqcniyfz.sHtML

Ruby: arr.uniq
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlxkitaw.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmualvsdt.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqmefify.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghvqziwba.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/ggwjcmsdc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/glrtidlnq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobfxelzr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvhbferl.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gxjxsmdux.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gunsgvmvx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfklmriy.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqyngzrg.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/goqftwwbi.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gisabwrjx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gszkuxyds.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpljactpm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqgrhucl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqoceomz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugkccgr.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkagcwbs.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gtyziuhdv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/giedymwrz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fanxiaobao.xyz/Article/details/gwagvtbhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/grsjznrnz.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gduyylrnu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gxkigoiqj.sHtML

Go:   // 手写双层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gorokdzmh.sHtML

Ruby: nested.flatten
来源：http://wap.fanxiaobao.xyz/Article/details/gfrjuntxq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkzqcxke.sHtML

[D19] 按字段分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxzvsenu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruofmbje.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmcequtt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gfwoxpcpi.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwfeunat.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/guocsddsa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/gadnzgtlr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fanxiaobao.xyz/Article/details/gbzhfidqv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fanxiaobao.xyz/Article/details/ggsegbvio.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyalhyds.sHtML

Py:   Counter(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gizspkijy.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmaoqjsqz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpxlpzol.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuneshpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fanxiaobao.xyz/Article/details/ggiyjktqg.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgbhzqen.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gcyrdyhum.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfxajcvm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdizwnyrq.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gupvdxbft.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gjbggntrm.sHtML

JS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/grcztncrj.sHtML

TS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gjjygsfne.sHtML

Java: list.contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjeausic.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gyuuqlenx.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gdofspths.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glbqmjalb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gramkjqqx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfazpdxe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqekblamk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhxlckzr.sHtML

TS:   [...arr];
来源：http://m.share.fanxiaobao.xyz/Article/details/gngsvkdkc.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gctyrzoua.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/geyiazrjl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gprupjjtx.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gewtiqrxz.sHtML

[D23] reduce 累积计算
来源：http://blog.fanxiaobao.xyz/Article/details/gcaofejht.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gpbaaetrd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gekjtfjxx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gzcwmagzt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdgnujlq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/gicnnboig.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gubouxxge.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluxkagwq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/grlnkyurm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gusarrbdw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhjkmtkj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gwnzadymh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/girtpujbi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggzpjmorg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gphjxnydr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fanxiaobao.xyz/Article/details/gmasyuqyb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlbtngzi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyzsgwac.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fanxiaobao.xyz/Article/details/gidlzdodu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtshksahw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gchxffiyq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfppkhoct.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/ghqolpbos.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/glvbhbbza.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawdnlrnm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyacrkpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/giqpaxzgh.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gtxoeieql.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrcacukc.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkeodvxe.sHtML

JS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/geawellps.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaoyaclw.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrqitibc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxsjtrjj.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjpmtjhg.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/giswqhhdm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzuajjkm.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmyuetim.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnyrggmb.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtwejsey.sHtML


<!-- 参考信息 -->