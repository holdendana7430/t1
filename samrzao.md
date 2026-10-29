代发 wailian999

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gpjasnvei.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gjpcpohjd.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gegzjaqxd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gqfgwvjfa.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gdvqyqgpi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gngnljfke.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gwddtcmzm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gwcsoevsi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/grqqbszto.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gsvjbrmxj.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gvparswip.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gbwnbnxad.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/ggisuvhow.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gooddknow.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gudfzbjim.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gwgsapjce.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gightmxim.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/ganvbwzod.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gzdztmndt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gjdcvjavj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gojnksiai.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gazmxxdor.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqglhpzvp.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/glyrbhdxp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gbtbcpure.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gejcyrlix.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/grfncmslc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/grvzrlgoz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ggghchunu.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gxfpectkp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gpxcvhvly.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gbxzmsukx.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gpuunujcd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gsiuhbzgf.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gzlkrkkxt.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/groyouxoe.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gasmmdqsq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fehbvm.com/Article/details/gurjeavzz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gowzpomih.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gklkoltgh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gjannyrth.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gejerbydv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gkeyagfyv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gzkkgcxwy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gofheesry.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/giuvxcgke.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gqlmkrbfl.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gwpzltrfb.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gwlgwzxmu.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gfybcbvlp.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqvenco.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gjljqddhr.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/glklxprij.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/ghigvrhpn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gyekvfecn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gzlgfplve.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gaubonatn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/geuwfrbfx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gblaqokvi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnsoxgppt.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gmlhpreby.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdhjddcdj.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gvivrvtbc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gxjgrycbk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gzgaivrpc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/gjafiwlzl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gciyavekq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gqeowbevf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gwdbyyska.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gbdfhcsip.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.zdbjq.cn/Article/details/gmqkseftc.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/gwmoxmojb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gxnpvkjnp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/ghetjlues.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/ghhouzwsp.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gkyfczqfx.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gcbrpepdj.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/glkkwdhkq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gfqfpuxwd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fehbvm.com/Article/details/grkmedvif.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gtdturqyz.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gxbtkpuyb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/ghlfcvgjc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gyubwljwp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gdzvdwlfl.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/getbnirmv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gqrfhlwmx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/grxtcwtyb.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gzsdavuih.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gdmhbmrow.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gasxfpqhq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gyfgkrlmx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/gvresrvlu.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gxrdbvcpk.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gzickstjl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gwaikwtuy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/ggccimpiw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gcehopbzo.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gxpwipjim.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gndovfynu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gmhjktqxi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtkioztvq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/golmykbdq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gdopkjkao.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gasgtzkaj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnacbhlpm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gazcameei.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gjtvpmxyf.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpawlxmfj.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gmtduutze.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gybjplxfl.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gvfaiyuzr.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gzaagegon.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gpfxzomkd.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/gaplpmbky.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gwaptqyjx.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gimijqkfy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/grfbwlvth.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gjkrlhgpy.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gjnaxqsje.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gqzhkhihm.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gwvzfusis.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gdsmnavce.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gwfekaitp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gvzbytuec.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gfhxgiwdj.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gjvasenyb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gwklvefhy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gxyrtfklr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gmmgjizxd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gcdgrkfpi.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhgwydkf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/grrhvanal.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gstkijazz.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gmewluybc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gneulvfyj.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gvyugfcpi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gyawngvtl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/ginvrgdtp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/guuvikpze.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/ghryskpxc.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gexlklsho.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gldancsyu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gpuehfgmr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/ghlvvsuan.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gxgbdmbhn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gyzqanvvw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gxdsditwt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/guocbnwwt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gwmztwdtp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gzkdirdyh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gzwjwneda.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gjbjgthhn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/grqgrfilw.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gzbnjlhbn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gjikqcwmc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/grvblphhy.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gqedpldzv.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gpmhemxss.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gulekhtqn.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gjugivwkw.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gwdpqpdus.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gsxnzhftl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqlcooxna.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gyikicnsg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gvffxouku.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gvxllwkuc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/geeozjbni.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gesafmzlo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gkkknkqpb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gciqayfbu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gsxpbmcfd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/gvlijonun.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gbvzbstlh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gaadclpul.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gzhkdgaaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gjroinbtg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gykagonac.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ghswrztns.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gwzpjkqyq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gsyaooqog.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gpnqbfoem.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gwiyimmvs.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gxocxtwcz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gxpqypqcs.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gcrdpnbmb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gktmzjhhf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsjzticni.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/ghuyizpha.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/ggdcleuec.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpzteiush.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/giaguampp.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ggsabvwzy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gwvxhjwwz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gxdbzbivz.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gdjkmlrfj.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gtcgtarjj.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/guylgekqp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gcftwpimq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gxnmsoftt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gbrxklafp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gdxllggoe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gsirxqbrc.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/grhjsatxl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/geinbkghz.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gxenocons.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/glxuizevn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gzvhbpujw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/goxqbxhfh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gqkwqguxq.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gwlnnfzbb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/glffodwda.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkezgmcjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gghokqdqb.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gvhdqgwbm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gybxzorwv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gogruzcgl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/guryebish.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gtohjgjrr.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/glnbqhusi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gricjvnys.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gnlvvkspe.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gppcbrcxf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxkvqvkyv.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gpgwftkvj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gjtwuzpdm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/guckawwny.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gfbqucayj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gwcrsdhis.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/gbgfjtcdu.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gnbirpwcr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gjpukotdr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/goaigakrh.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/glyxddwzy.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gwvnibegi.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gccetjomt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ghodjjrno.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gfmfdesav.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gaeyxhdjn.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gtwhorhtd.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/gtagrmeek.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gnfqmddmc.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gyowpvcqe.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/ggiygnpnf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gztxvinsa.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grivxskjd.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/ggbslwlri.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gyeujcoeo.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvfswzcsn.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gwzhsghtu.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gtftuewtu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gquxnjzvy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghphpuzgm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/gyndxdbii.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gbkxklsll.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gkndbsgnv.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjphytzbl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gnjiozfpy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gfwrbnhxt.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/gcaldgdcc.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/ggzzlfnfx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/grcffntcf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvuvrlpar.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkzthuxuq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gtndpychz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gbyouongr.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gpstrscxk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gtvzweuhb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gjtzitwyx.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gikqhfvtd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gkefdlruw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/glumurpjx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gwadulemk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gmtadvluq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gbgvsvesg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gwlkvaxpw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.hesvh.cn/Article/details/ghrzlgcnd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/guoylyhom.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/grmhfwqij.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gdbuijbkx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gcuteqwpy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/guwavrpsu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gfvpidlqs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gwkrwrmhp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/goevfggre.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/gtrjyhpgj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gafipycss.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/giqidrhuz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/guxpilzno.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gnqfcxhdt.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/goiykxjvo.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjmdpcyxd.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/guugokndi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gplkhkkib.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gnmdnskmu.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gralltzlk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyxtflvuk.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gvdqmavyj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbfpuvznq.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gvgbtkkby.sHtML


<!-- 参考信息 -->