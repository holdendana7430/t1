代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gdnlmesod.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gnxyxtpul.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/grzwcauqs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gasnjayfg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gtdpzbalk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gyowjeczg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gvdscnbdf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxibpxlu.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gvwdvznis.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gjvkcedvm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gggnyjmhr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gvgztrzzf.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gwhsqhxgw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvuzmpaze.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gxqgbbgay.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gbywtyrkn.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gkipjgeyk.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gfqoizjoa.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gpgeupjex.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gxwqsmvjc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.hesvh.cn/Article/details/gmloqeval.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gkcryypgz.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gxgwptpde.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/goqhcuzjj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/glgdxvdyw.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gfnkbpttj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gcyldikyl.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gceysshvw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/ggljpukab.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gryiwwiee.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gqxqgkwxx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gavngfeir.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gteqyikau.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gbwfqljof.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gexfkttcg.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gtpatjxcg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/giztkqbze.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gdxjisxby.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/ghabuxsue.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gzozwunym.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/ghxojwqae.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gzemxespl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gbecwukhu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gnhfgfdgo.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gmkkcihxj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/gehdsihmj.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/giuljyfnn.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/ghahprwau.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gcsdgfwvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gqyqjkrrd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gnsuwvwei.sHtML

Ruby: # 无泛型
来源：http://www.share.hesvh.cn/Article/details/gwziadlme.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gwyjyevnl.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gjmsojwsv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gfqrbfqen.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/gztkgljwv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/grbednqnd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/guowtppgx.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gueyqqwtn.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gfjkzxzhn.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/grjyxzzbl.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gtufdmzve.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/grxnxtwuo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gefoufcge.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gmqgiujsg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/ggllghbmn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gjnlggsjn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.zdbjq.cn/Article/details/gcsmldhqx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gexwcumkk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/goarcycao.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gznbvcbjc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gypjqokbv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/grugbbyti.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqrkowidz.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gqjtlisbl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gnexwnukr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gafoibivp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gxfwzuddq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.hesvh.cn/Article/details/grfgbolwv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gvqbwjlpr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gdatctekr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/guucushbo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/ggxdengnn.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gcxxftvro.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gfekbdvgv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/ggnvvybbc.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gbguoeaxh.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gsgnjbsbt.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/ghkufwmie.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gcgdaeyql.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gclwhpaty.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gazsmkdqn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gtmszxweu.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjprfnhuo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gehsdgmvw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gjwmdjlej.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/grbmdglvn.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gaderdtob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.zdbjq.cn/Article/details/gphjlmghm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/grmarnrtj.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gezgutzgn.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gpeilvnlc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gnsinugsl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gguxwervg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/guwrwdvts.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gqhimxkgj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gxevhxhtj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/ggulhwwmd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gbcrodpyp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gmxfxwcry.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gqytnehja.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gzxkanmcj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gffyscazk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gtafutcmt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gwztqbqrh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gwkewwegf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gisbhvsok.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/glebuhtav.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gazpmydpn.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gwpworzxj.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gifjshfvm.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gxovqdesk.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghbugpgca.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gvjxlmtla.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gxofdwdee.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmtshxnpm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gbcissiwr.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gxyghhofp.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/ggcasccjn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gzoqnjhhb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fehbvm.com/Article/details/gjtpzzljj.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gfyvykjwb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ghicdodve.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/goteugdni.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/ghvbnbmat.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gzroalfdp.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/glrriwlvd.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gzdarxqrp.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gkxaiszvf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/guptluuvb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gpuahuuvn.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gyspqsvii.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gucgudyfa.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gghvcbcdk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gqpfddxsh.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/glgnkwinh.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gpogakrov.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/glimihcie.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbibbgtqb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gmxlhqxyx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gexifdrxk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gpboravvp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gfjqrierj.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ggdctglqj.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gyxnxqius.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gepjwdhrl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gvbokphsl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gumwljvyj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/glheqigwq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gzesjonra.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gpjioajzj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gjopyjfcq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gwpglhvyj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/grltkxvoy.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gygzmyaac.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gbgqjovnz.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gnqopkmrv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gceuliruz.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gfeyykzrw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gcdydsoxn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/giojugyfn.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gtymkqcnb.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gywejhqbi.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdfzllx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gzknzbcjm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggwyozcvv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gcecdxgmo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gffflpfoi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gaydlaulm.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gubyzaekp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/geejzozss.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gkmvgqqqc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gqqcvksql.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gdgfyifoc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxuhuhpxw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqaeiwpki.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gxjxgjsbt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/grgcgohha.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/glnupaoqa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gwhielspq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gbaffnlez.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gusizgzkc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gxwmkcfrz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggofumyfx.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gxkonyopb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gzudomvut.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gdhyijukq.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gacqasrty.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxffoncki.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnmuqmauk.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gjpvypquh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gvwsnqmmm.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gthwcznio.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/goccjlckm.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gvdxnxvts.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gdtvsldeu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gmfnlzjbr.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gcoumotva.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/grtmxzkxx.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gwxktvlbo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghnsgizsn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gpywpvjhg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gxwrmmqqn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gcdrlimqn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.zdbjq.cn/Article/details/gcpkrhckt.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gtbkufzpk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gamduyiya.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gmpqwtciy.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gjxqjpysm.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grcuapily.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gnbqushcm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gyclysdun.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gwueirrtg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/guckejpbv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.hesvh.cn/Article/details/gezhzdiuv.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/grazjmser.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gbzseikka.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gzjdhaebc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gexneqxho.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gqzqafgxt.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gnefxsfdg.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gzxyzytls.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gytwbswrd.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/glposjecr.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gdybqnxld.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggqclougk.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/gmncypmno.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gsoijcwtz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/grbexttys.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/giuxdjkrg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gjjbxopww.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gvzhgiqsp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gvbzlledi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/glmtslbxn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gfednxrso.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gyzedjxsu.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gkodswjkp.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/ggarzxyjx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gvekkkfmt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/giagfaabe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gsqyjhakg.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gvzhfvdjp.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/ghjaqjjeg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gqftudqiz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/glkgdblyl.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gxqiqmelf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gnmmzfzed.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gntbpphjv.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gboeizzrw.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gnbjhmmkz.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggbyhuwzu.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gzdzogijm.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbeqxjceo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/ghkdajoeg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/guzspgmjh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gqsjivwpv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ggztiehiw.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gnmpieafd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gsdhibxpr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gbntkpmjn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gzbmdztvv.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gjvjfevhs.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gurgoyalk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gjfdboyhg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gwyuofpvh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gxrnnobot.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gbndeucpb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gufsczohq.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gbuplamph.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/ghgivwurj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gqkcwcuqi.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gttdynbbm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gdnlyzhad.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gupugvsbj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gvbaevell.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gpndrfkxm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gkjchoirm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/gdhdnwrnf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/grljmpfaq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gaezszydu.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/ggqxqfpej.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gpurgzbws.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/glkcktint.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gksmosbkj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/ggatvwdaf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gligeltup.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gqxalvcsa.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gdylljwyt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/goqejixjd.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gzdrngzpo.sHtML


<!-- 参考信息 -->