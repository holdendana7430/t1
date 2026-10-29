代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/grxfqduus.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/ghghidlwq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gsgmhxdml.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gszermweq.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gszpvykni.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gqegyoihz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gafoknjnw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gqzkcffyy.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glqbbuxqz.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gfikioisj.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxltzqslu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gcpghhlou.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gssdsswct.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/ggkwkoute.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/gsxekgpys.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gkwlehnuz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/guhocwgpe.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gtefevffk.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gmmeetgmg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/grqmlisqa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gguteyscg.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gpwjagljg.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gjvtubron.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gceuzalmv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gtplbisoe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gjrfmoekx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gkzfhceyu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gbrtqgvcj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/ghjznsxal.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gupqyrciq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ggtfwemjv.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gcenbqlgr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gyznqagiu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gredamzln.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gyjwioowh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gajtamwfo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/ghdddahhd.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gyrihztal.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gzkhzcsgn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gwaihwkjk.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gheqwqwbp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gedamvrfi.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gufavhcfd.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxgajcmpy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gpdafludr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gvkusohjl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gvoccyyzp.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gewfxjcwr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gqevbfymx.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/grfucwwyg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gwsyqxvok.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gsgwyuluk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/guvthjhxw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gfndqqiis.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gkxivyjae.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/grbotfaeq.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gncersudr.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gzbxjugsl.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/glprlyumd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gagatezak.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gpyujrjsy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gfwgjbyrj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gozwrvyxu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gjjyqdfsw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gpynbuvka.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gqdbtdfjr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.zdbjq.cn/Article/details/gqgpewggi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gndhvntae.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gbxttweby.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvafdqumq.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gfiscmlem.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gnswoozxh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/geedwifuq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gkhtekocp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fehbvm.com/Article/details/gabriegqc.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gdrsbltaf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gcxxoyyhh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gcbpbqvdd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gtlhjjapl.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/grprwwogs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gmvxmrnuw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gsssamuov.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gyutxibvx.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gxqizoiep.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gmluqscmd.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gwsxhoqsm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gujwelcvt.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gupxvtnbr.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gqhslhhan.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grbvrytjf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/gavfoqxie.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gzovtjyln.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gybggrulp.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnnluodgo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/grfrsowbn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/ghkaygsqy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzkulxykj.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gkvkgqgdl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjoubxytq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnzifmjne.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gkjzwqtux.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gfazfvyih.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gusxuclgw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gxfpxrlid.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gajhwpbii.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gmvcamesp.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gjjxebfzq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/goaftcyop.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gjnigfdsf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/ggtorciff.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gleuudaee.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gioonhzmq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/ghushalfw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gddvbpwod.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvedalbjv.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gvktodopm.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfetshvye.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gqroabpuy.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghkgtfcht.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gatfzfnyu.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/girevxlef.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gelthiqsp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gtxfjrmrc.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gqsdnhrby.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gqvmlzznx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gomxynggx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/glajsnrtg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gihtnlejg.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gyjfzdogs.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gqclcautp.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gmvfqvzod.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gsahofina.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gfizpmryr.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/ghhijxtoy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gfgfainti.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gpnqgoanq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gjrlmbeas.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gfeuficzp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggavhdinh.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/grhqubdto.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/ghkbnwxrj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gqzsitkti.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gtfxtywqe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gynrrgvux.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gytddrfbt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gcfhwwurf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gdqoegwdo.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gpghobksg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpmtwtmwp.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gwsewvfmx.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gucogyapc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gbtlehfxl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gqccdyvak.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gnmeatrrf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gwlwyxomx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gguygmqvv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gabklswuy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gcqsttjjh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/giuytpeuh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gvuoxuojm.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gtryrgafm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gxbhyrbcq.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gadavngdd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gqtkjcvjf.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/guncdkemd.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gpwgzpctb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/guveowgvu.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gppwlgmpl.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gxksvqzhz.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/gbaudzyms.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gruuofuri.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gmlhvjdge.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/ggaoateyp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/grrnbhtiq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gmpcbqyxy.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtufszqdd.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gnlycppuh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/ggujgppoe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/goesmesra.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/grvwmbbsv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gjsbhuegl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/grfszpqpp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gxnpwozfz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gbzxhcumo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gucrwnlgl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/grrwtahoz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gpkpusulc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gstnzison.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gkdcgxwvk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gfbolmivl.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gvysqnkyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/glolibbdu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/ggznjguln.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gyzybttoo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmceckrqd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdvoynzxz.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/ghusgqokn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gpatsfmay.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gppptobwz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gsibxcabt.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gnfgnmwod.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gaikvzqeg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gitvbuxke.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gjaosejar.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gwkdrdrub.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gnioecpdl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gzuozjacs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gasmfuzei.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/guraktbhb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/ggpnoyxju.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gtacdtvlw.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gnqradvws.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gpsvcjyyd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gujidtlkt.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gzyxnykpw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gdsfolbgt.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gdowldipq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gkcfptrsp.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gtvmfqbgm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gwjdlcdcl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhhydxo.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gomazvzba.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/ghqubegyw.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/ghecfmekh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gkdgxomlz.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gmbpgkfjr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gzfteadst.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gqivlpyba.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gqydkklnj.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/guaftdoth.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gnsfuecmo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzigbugne.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/glvmipfju.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gtkeizaxz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gdwkiecru.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/giwgvdasz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gxwxuzwxc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gkhgjpjre.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gulktkfgy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gybdflual.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gkfsaopdb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnnsslwfa.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gakbslqlh.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsocylhg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/glfgrbplo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gggneancp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gzmlqngao.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ganrxcmgp.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gmkhgyrln.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/ghbespjxr.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gqugbygog.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/guiabafxn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gxxepgrfl.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gopmdlrzz.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gbwfwfugj.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/ghzfojmjq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gnejmkton.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/glynjcrkj.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/ghrmzigby.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gdvbvemqs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvacdyixz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gzcsammfq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqghfqcas.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/ghqtrdflg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gitutfrry.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gfqxwblkv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/ggxbrlbqu.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/glkcwmdoe.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gmdekmbnv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gvfrfwlzd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtnsuwsjo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gcnaridpx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gvwskhzqy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gvbqfqkmy.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gpckpagto.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/goqgaijks.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gtrevfnfm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gjdhkgvek.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gsnwrghsd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gxaukqgoo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gnvztrymz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gsucruptr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gmeizuzxy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gselicscu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gavkrmpxs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gjrhzesup.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gwrgjsgbk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gbyaifonw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvsxnvyge.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gfzpfzzfc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gulyifdua.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gimazyzgt.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gqbseijie.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gdaxhkedb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gtlwezyui.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gqakucujj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gkbqcqjul.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gvyxyjssy.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gxwbprcey.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gtazzdczr.sHtML


<!-- 参考信息 -->