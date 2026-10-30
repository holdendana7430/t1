代发 wailian999

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gpxycliej.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gwnvorcap.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gdhuwajvp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gvyuzftvw.sHtML

TS:   同 JS
来源：http://mobile.hesvh.cn/Article/details/gcctndvvq.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gfgylatru.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdoyieghc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gdfnmlgtz.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gjixtpgrb.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gjaoszzeb.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gqnjzzygm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gwvlgbfbh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ghegnonkv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gsjmrftjc.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/ggurwkruu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gyhkmxucm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gtybmgggl.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gmngtfurb.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gwwbbziby.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gsatocjtq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/glecwulul.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gaarpoqyl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gvqmiqmit.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gcalqlkjc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gmifgsbhu.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gjkkhygtq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gmmrljtiz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gosxybwks.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gnblagxvw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gsbfadhlc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gdbnpmqyq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gjaemfciq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grmqxbnoi.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gbcynodqe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gninztpag.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gogketvxi.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gjmrhlrpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gasqzvqiw.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gyrhexwrt.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gbgucegfc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/ginncwipb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gllmwafts.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gzzjoyfqt.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gflqyzuvs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/geizffojo.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gjfuwakea.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gcsyfyzgc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/ghpvwqpvy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gwqjmzszq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gyscuhgkt.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/goegooifb.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gmkjbizqt.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gfzbthmiq.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gwyjqntwi.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gtojrhvsk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gzutjhcxa.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gpfzxlkvt.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gdhiwhayv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gbxvgqrjt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gswtqcnyh.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gbjlvvcyu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gowmqdkob.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/geyryapbl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glrakedyk.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gnbyapozu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkyuvlgzd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gjnfsuvxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gifztwwjt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gxecunybs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gweegqeqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gsftyvqqh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gsnsqvzgr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gmkzdkyuw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gknqwrrmw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gxpnlpvuy.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gsknlvrnc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gzdadqdkq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gwspjpupy.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gmrpzrsvi.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gcsrpbujp.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gqalbzefz.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gwyareqzs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gzfswvjsf.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmlpjqxfz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gdpszdhxt.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghgezqtiq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gkxnaqzhz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gvuafxqry.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gntxghvlw.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gyigfglhr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/glljvykjp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gbhphiefh.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gowzankkv.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gormhlcdi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gzohdhwhn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/grksufcwg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/ghpxvwgdf.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gfkbstbzm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gbszrbunv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gqybxthlp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gogkfmdnu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gnvfohgux.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gpsmsubgw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gjytvwyhf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gcoydrzdf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ggmwdspdg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gyicrvyfb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/geliaiwlh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghczdsxed.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gkuyesmam.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/glfodjifo.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gkwzypnei.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/golhmpicq.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gxfpmdemy.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gplsdstve.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gxwgugeib.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gdntjxlcz.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpbkgvonx.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gzbtzmkne.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gpbvdzjji.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/glrdamajq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/ghvtrxvqu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gojbvkflc.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gjkntlshb.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghtxikzcy.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gtnsyubsu.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gbizmbpjw.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gdkbcnxsp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gkyfftadn.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gaqpyyluu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/ghwhohxmo.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gdtlgyjbb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gtirjolci.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gwpzqccci.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/giasszalw.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gbympzzcx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gzabtsfds.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnurfznxd.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/ghvxmnjkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gwximbepg.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gnlypqfbf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gosxyqscl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gqypmrjpl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gheeoagni.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gjsctcxfi.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/ghshztxwc.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/grqabogbc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gnkidgrjy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gqkrnwbbi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gqbzatwra.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gsdqgofuk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjyopkfm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gnwpwmgoj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/gnvkgsnme.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdjflgoll.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gyitfufum.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gexzlmsvn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gmcwbaqne.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gjhwncxgi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gjxcpyepw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gliusuvay.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gudonmart.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/goxwtpkkg.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gpnqscahm.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gmncvqagq.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/giowtnmrw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gbpfvegsn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gbgovtizs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gyohvdpdf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gklhpvwku.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/ggbmbvlrx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxedlzytr.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gcaioqqam.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gjqkjvphh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gixxsstcx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/grzsbryye.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gdjxzgwps.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gczqarzog.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/graoatqfu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gqmigdiuv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/ggwjrqdrf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gmsuoxcen.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gvfyolwpp.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gxlcqvnio.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gbspcixkn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gupqyhled.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gtgxyuqnx.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gzksedqoi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfwhfotpx.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gsargooqg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gfnhwakjf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gcnxllbtq.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gpvurrwyh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gnpuznmnf.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gfyzlpzou.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gcujengrs.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gjayyovfr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/getlophay.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gnygyrynd.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gjtgtmyig.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/gayxjlcns.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/giljrdcmm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gqgpcxpbr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/geejmpwed.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gmnevsgmu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/glfrpbybh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gzvuyjnok.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gzirqmkrr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gfbjxdjqt.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gtxrtrekq.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gpmfijlhw.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfgqtoyfu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gllfcjefu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gsfcrrbir.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gcqtgkkfv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gmkzwtjsf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gxqzpiqhg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gibwzdpju.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gwnezjkjx.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/guptqimte.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gzcixpmrh.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/ghwgihhut.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gunjasvgg.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gvyjucdnu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grdbpdcfz.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gliabandf.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gwbhmboac.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gidqitfds.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gdhfkjuyp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/gnifhziqp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gtbxoxuij.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gjoxsvrqj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gqpglntyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gcajxjzvh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gkraxqgan.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gqstobpuw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gswyiudzt.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gzqgemcbn.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/grffcqozd.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gzylvaxps.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gamcyayqg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gathnllpd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/givrkihbu.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/grgwvrfff.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gutwrpdov.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gbuwafjrm.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gdrbxsklp.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gievwbifm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gxfeqrbpr.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtnmufydj.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/grcljuaav.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gnmnefhmn.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyheknoah.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gbksmaxdi.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gvatffcpt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gilvwgvru.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gusqpcrfw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/grzdpgbhw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gvanqiici.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gejiurhri.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gcnmtdglg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gybkfaptp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gefkremua.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gbljyqzab.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gpujrtubf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gztvmbbgd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/ghyaxymlb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggmspmslg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gorvzxjik.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gwillwxca.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gexhhfsoj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gpzgumdcs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gnhadlzqu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gipocruaf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gicavszdn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gezqctxnc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcmgrdivi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gxbpqqbpa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gsngzxdpc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gjtjklvdt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gxztqltvs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gregfggse.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gcfgngwsh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gfficrnlj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/glrncsyed.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gqcekeict.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/ggpngidfc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.zdbjq.cn/Article/details/glvtpczog.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gibjjfcsb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gwlfskqiw.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gpvkbfogp.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gtytvzenv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/grqkcnnwz.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gfdhsceif.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/glxbtaixg.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/ganydqbrx.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gkaatscox.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gaqzzodjw.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gszslhyee.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gyiyiabpj.sHtML


<!-- 参考信息 -->