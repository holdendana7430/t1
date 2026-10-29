代发 wailian999

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/giuadncwx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gbtukcrqj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gefiyrezk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gbicwecll.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/ggsxciscb.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gwnzieizf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gerdcqtri.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gxsvlyeox.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gqztqrykg.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gqucmhtnm.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gasjkkezs.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gwhhdjxqb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gcikoocvf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gazaubcfb.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gddaqsqjl.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gftbjdpwc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/grhdmsjxx.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gjepmusdn.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gwzrukzfq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/ghulawugm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gvoerxrvq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gftwgpmrh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gpiiutnbe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/garhjldsa.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.fehbvm.com/Article/details/gclurvkly.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gtwfeumzq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gmwxskvtf.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gqkingtlm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gnitmcjne.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/ghgfeaiar.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gwrchenmq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gjmcpkjjg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gitufsjln.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gwoiyngxk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gprzuodms.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gkoupvebs.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gtgjitnke.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gvhetmeei.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gdwgjnhmo.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gwfrghjgz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gfzwsvwji.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gsnatpzwx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ghyfvdtqx.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gglwakdjr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gqcphjhtb.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/grxkukvcu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gprcevfhy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gtetexksc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gyfzlhtpc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gtrafxvhm.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gusdaxocy.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gshzihbrd.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/ggvltejfj.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gpaiurnst.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gjpkketmc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gfoxckvqx.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gxkrvseiz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.zdbjq.cn/Article/details/gxqoaaudt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gxnksqsqh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/grnsojiee.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gppbumcyj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gttlnovqo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gojutxgrx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjbytfffz.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gfexzdjir.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdycvxuah.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gksrekzwh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gmsjrdttt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/grmjngtzg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gegzoyqko.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gmsfrplde.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/guffmthan.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gjrjqasyf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gfsybegej.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/gwsgqwcur.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gozymamib.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gjjsuhbbd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gjlfaffxi.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gufmcqwzd.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gqznhwsky.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gpivoezag.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gwsawpvjt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gygjuvjtz.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gabwsxnbg.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gyxymbpps.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gstascfyf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfaxyvnyu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gsbsefcbe.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/grbxagpyh.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gwyealcju.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/ggftukjus.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gzbbcblki.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gsgcrhzdo.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/ghmbtupol.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gxlnnkesz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/giurvizcr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.zdbjq.cn/Article/details/gfdxdyrjw.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gzcpenrje.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/giqomltex.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/glogquwtz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/ghkputnvx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gpwnilwwd.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/gdecwydau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjwbrwoyq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gpbdgstij.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gdaqldyev.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gnswqlhjo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gkottqsbe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gvhzbmfab.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gkfaxxrzd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gjzbxhbwv.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/giwfffkio.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcqjnezjz.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gklmohnbi.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gsmuipplh.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gdlwmovpp.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/ggaixxgwf.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gzqdvmkxy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/grycqxzdv.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gkixgsrix.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gmppkbzil.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gbjmbdqcl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gqukfupvc.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gzshxosqd.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjqhojtuh.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gyekpgebs.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gedctrmsx.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gnzrfwdux.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gfzvkkaai.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/guedvkvnk.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gkkqdoorc.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gahsvlsfk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gvhyhvmxu.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gxftonuth.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gvzejzgwf.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gqddtefqp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gszdicujp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gjtkxpltp.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gntkbmbrg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gnwitwkgw.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/grqdhbmld.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gwwrkyfnt.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gedcrtwgl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gvpbymkns.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gjfdtpfdm.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gckokxhzh.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gyjzlwttx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gaqecjvaw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gxcoegrnl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gzkyiiwxz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gxrgfuqzs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gkpwfhvaj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gddhopuzs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gllznwoad.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/ggvpxdrnm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gkyqrdtza.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gzfnierwe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gpyitesnj.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/grhdfeyls.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gsogthxpj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gftmdaulx.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gnmrlhzke.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gezneoizi.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gdyuvnzow.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gmagnxcbt.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gcntpyifc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gpcsuifvi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gsgiyejhk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/grwigvlpk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gnfivfizi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gsqtombgp.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glmsyfpwd.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gpcnqkduc.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gikbxopqw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gmuxmmhsc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gcvdijdse.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmwvjfega.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/ghcvaglpp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gcscdwyum.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gleuglkzq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/ghzhhikkq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/gdwniuclj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/guipgixrb.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gejkkqswz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gopozpult.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gtyzvztem.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gdfdvgxfa.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gqexstncx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gipesabkr.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gpdxvowrp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gbcimdgqz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gfgmzyrpi.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gztdmsomu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gcilfbvdo.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gcsamnikw.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gtlpzebic.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gjtzkggna.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gwhdibqxv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gbtqgihyw.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/ggyacrpxy.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/grafcedfy.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gjvlfmhgn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gpueghstp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gdjvgiikd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gnhudqefb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gcgzlyptw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gbplnhyai.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/girtqiovk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/goymngcwj.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gqpavwqhk.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gpwotqjzm.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gbavnngik.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gizfvdmow.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gauxhmzti.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gxsoopqzc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gqnzwrdjs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/guksivcdc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/ggkmohpsq.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gxgvhcmtn.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gnlpyxixk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gkithnsyc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gbntyltxr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gbdlyvtmt.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gjdiveozx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gveluvznl.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gjazampyr.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/grokfsfby.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gojfkocgx.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gdjkjyvar.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gqdflnppw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gpitbywcy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gnvtqphbm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/grtwgeiyo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gnmdytqyu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gdsrgltjz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gbztzrmeh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.zdbjq.cn/Article/details/gydlbyzot.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gwmgxodzq.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gfsgjggvt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfbbrurtc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/glwvryjkd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gehpvnjug.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gvouhufgj.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gtpztpbuy.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gqyvwdfsa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/grijfooru.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gybrgazly.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gjmmapsbs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/giysgqxjl.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gjmxuuldk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgnoankk.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gpwtyuifx.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqkamgmps.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gdgrkaooh.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/grhtslawh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/glqxlhlwq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwjezwaej.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/goxralelm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gosqjnrls.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gyudiilht.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/grybnrdvx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gxbsunzxd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/grzfawqgi.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gcrgwdhyk.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gohhmcqrk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/ganpvjjrx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gdnxguxub.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/galnvqbup.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjxdjtafb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gporzguxs.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/glljwdwie.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gyvpovsle.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gzlbivqfh.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/gpsulpnvz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gtdqxuqrk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gvvtfydbe.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gajrfurxg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ganjqbawy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gmcudsats.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gwutatfbq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gttdudbzb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gegrfstaz.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/godeqitdu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gfcjnhejr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gdqmnxabq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gcbgkiyxu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gaufhljkn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gaehonaai.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gqsoripwg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gxtqywdea.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gglztoyoh.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gfwzzgkmv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gjjjnfuaq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfxmjzyqw.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gzmxyloiz.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghuholdsx.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gikmrvkqr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gmoituwtr.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gndfrrwns.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gugsxhkdg.sHtML


<!-- 参考信息 -->