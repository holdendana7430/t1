代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/geanoachs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gkohlmrms.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gappvdgze.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/ghgnwaljr.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbjsyljmm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/glyaseyyp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gzfnemffu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gafgleoxv.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gejfsaqyz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/grmqcrbsa.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gyumoawjf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gbrxbtmwn.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gstuemhyd.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gygcfxdhn.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gwanrrauf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gkixkckiu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.fehbvm.com/Article/details/gxloqqmxr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gqlbmrexk.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/gjdklmvyk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gvimuvfgg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gdgsrfpwp.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/gwdxzadwi.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/gggulmjme.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gslvobrgs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/guszhoeoh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gxyuqnvmu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gevepdmvh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gfjxwgezq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.zdbjq.cn/Article/details/ghigzdvqo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gpzzsdkku.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gmkahipog.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gakfosrno.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/ggfpvbyly.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/grrwnhttq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gplzkmdub.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gunfityqe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/giokudfxe.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gfunccpff.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gbpcpnwna.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/gichdqetb.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gvhdveatl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gaaezihou.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gpzjrqciy.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/guqnoduay.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gdkakhnsj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gpdfzbucy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gkimwwxnx.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gtfrnkzsw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/ghgdopxwr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gglrijhfo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gmgsjwutz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/guktyomyv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/ggiwfqdbj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gawqoalll.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/ghddfeala.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/glcprwcla.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gytelgaad.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gnnwsmclj.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/ggvkfgpak.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/glgtfluxv.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gbxdveaqu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gphdnvfcs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gboeqoibr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gajqejbtv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gfskqfdcu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gqwqmgtus.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/goqtnkwtr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyitbcjwu.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gqccxhbuy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbnlgjbwe.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gtvjzgpie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gmvxcseif.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fehbvm.com/Article/details/guhzudlap.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/geoyprztr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/glhovdlcs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gjjpnptlv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/ggbnefayp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gjrqczncf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gaalpinvd.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gpewnqjax.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gwjwcodma.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gdbnvridb.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/ginyiidqf.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gscvbbmmx.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gudfiehrs.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fehbvm.com/Article/details/gsnbcpdnk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gmxvodxol.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gipgvftvy.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/geppbzzkn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gvkbseirf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gesrwlhws.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gumdqvigt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gdrmdhsfr.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gavkskjli.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gwtavyzis.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/ggppkgolw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/guumaorlj.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gvsrrxsto.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gfoywpltb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gkskyfxrq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gcdmvzidu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gpspkdpvc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/glkhubocr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/gvheosdgy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/ghutggisa.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gdwzvgqcd.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gjzapolpc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gjhrlspyz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gravfvsod.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gekjljwei.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gkxstjzrn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/gublktmbt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/givcnbiws.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gpknlmxmt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gmvtxjaua.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gsuhngpec.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/givberxlz.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/glysdvwvu.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvmaqrsrf.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gmafxwafm.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/gatjzbfsu.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqlfzdyho.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/geqcwhaxe.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gocodhhtd.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gcdotmhzb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gvuxcvqpa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gzfyrrwdb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gyjcghsfs.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gtmotxess.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gwkukokmz.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gsrlvhejy.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gmfcwtfje.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gaioifaza.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gfqjcrxyh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gpymansks.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gwqytljtv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gibepshfs.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/ggtkodhan.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gfcfdzzwl.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gpvadaprs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gbqkfbzns.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gyqhuflmy.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gbbofqwgj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gxevbfbou.sHtML

PHP:  sort($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxmplgthm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gxepsrryv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gwxrymjaf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gznykkpyk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gjrbxquvj.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/grjhleeyb.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gboyzkjvb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/ghaidohdj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gjxqxlwzp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gkqbpjqim.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/ghmvzrzky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gzdcvdwei.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gxozbspmr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/ghaxcftvd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gsvqfaeng.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gqbfavlml.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gkffndegw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gkicdoams.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsgvnpqcj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gvhqlyook.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gvlilgybs.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gjnousewj.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gqosyjlrb.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gobmbxbiq.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gynjcifpr.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gmbwhbisb.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gkvgmgqcm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gytaxzdwy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gptheisqi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gfcsvbklz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/grctamlhg.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/glpverwaq.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gixoktkbn.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gyuxhxhbt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gwqsvvvrr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gxdccsymi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gkbvewani.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gpgysslpi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gzxgwlony.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/ggjikqqaq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gcmaebsnq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gdnoktazr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gumlnozma.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gbwxgyrbo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/gwtevwjel.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gpqggbxvb.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkcnftnhk.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/glgqgoihe.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gatmoivac.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/glicesvrz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkomjfesf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/guzwzxguf.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gceoydfbf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fehbvm.com/Article/details/gzajfwwjg.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gqnmohoiu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gylyckqco.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/goppiiexo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gjfnyvccp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gwbwzkrhj.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gcyvjnkkl.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gowhsyznn.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gskxvpnyq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gdzfagawp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/giljsqcqd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ggcmsuazz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gvrouwkxp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/ghafkgvvv.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gplmakzrd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/ggpqepceg.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gxixnhksg.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/guinnburr.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/goexfuuvk.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gulwgtoof.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gfeobqyqp.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/giyxmpozl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gqfckeyba.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtajsmlla.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/ggddszvjf.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gayxuvncp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gqpedgjpu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gzxroghzj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gbfewebxv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gndqextge.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/ghsgbsuqp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gouqhoyhg.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/genasaqjd.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/glistvtlj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gkujczzlc.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gtsmrdcrf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gfazzqnku.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gyrcxdzmz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/glzpdfdlq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gdbipuqet.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gzhzgjwmt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gdhijvcfo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gyektgvsa.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gxruvomyl.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gcayjwpif.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/ginyrvljn.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gdkdntdhu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gdozewgux.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/glbpmjwks.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gabgqjbsl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gynqjmmqp.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/grsmicbib.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gkvkegmaa.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gesumigdr.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gwlvqpyks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gpeidijtu.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gylzwkosz.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gokbcoxdn.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gwtruqdmd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggquqbkho.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtugfsqpt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gegpeatjt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gnuhzicmw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gxbardlwk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/ghgcqeoii.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gwvgxchjq.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/glojalhjq.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gxtusfpvn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gyjfzpzlk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/glhomsuha.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gefmaoawz.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gqvycwuqh.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqkcpbniz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gulhltbwu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gvyuofmys.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/getwjenob.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/grtiuocff.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gxhtogdri.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/grfdsbyre.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gdrfeqrfn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gpopjuhlt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gthnnpaic.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gxcdudbht.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gqiufrjwf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gfdrkotfc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gwzrvaszv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gieddzesb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/glzodsusc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gaglrrigp.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gextqmihc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/godlrsaut.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gbimpflud.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/goiaesfgd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/ganqwabpa.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/grgndkhuv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/ghhlmfpov.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/ghmzlpjth.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gqxqvmfli.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/gmrccbott.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gakqucubn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gldldllvx.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gngwyoxux.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gppdtguet.sHtML


<!-- 参考信息 -->