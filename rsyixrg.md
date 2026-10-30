代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gmijdgblu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gvljnkozy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggxtntgyc.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gaaaqkxxu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gblizgzeo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gbuoqdmgm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/ghwfdgagb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gjfyhnynh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/guzjnqilv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gobnxfose.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gvcccihga.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gqyfztcdf.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/girnmcfzt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/guxekrazz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gkgsxqwbk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/gqgiqchby.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gxwpabest.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/ghcdbajbk.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gvcsdnsrd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/geztgykae.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gmgspjrbd.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gsoklcynr.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gxftznwav.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fehbvm.com/Article/details/grkevbyqo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/gxptwhrde.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gfzykyfmv.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gfbkyvkqg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gdzuqfwde.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gjvtqcjbr.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gdkygdoai.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gvndsxyli.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gebfzmzcd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gzpgiirjo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/grjtcgcyk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gymuiasja.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gdvmhyujg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gdhyjztsp.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gbdzrgrmr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gxxrcqyhd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gnzjhxosz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/geaqhggqb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gyhlfttqn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gbtarnzhu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gcjafooeg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gruwyfeik.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gqyrjhvfm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.fehbvm.com/Article/details/givbmtbwd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.zdbjq.cn/Article/details/gvchiuhoi.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gsaebhgzz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/guuzkurdd.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gmarfptxy.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gkqhdsiwn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/giojmmitk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gdscflaxj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gdqkjoqom.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gctyqftvq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gagrrpyvw.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gtondskyp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gzlzzmxqq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/grnusfiui.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gsajlczcg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkoorncdz.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gbclzkoli.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gzhvplrys.sHtML

Ruby: a, b = pair
来源：http://www.share.zdbjq.cn/Article/details/gajqkicbt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gdlzdhyfe.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/giduuirqv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gyajktswu.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gmuwtxfay.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gjjnozguo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gwvnejija.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/golftxpfr.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.fehbvm.com/Article/details/gwjmmvpea.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gidtlrzmk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/glckbebvi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdlsolheb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gqfuskwkx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfaowzpsh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/gkdapxuhn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gxhiaaprc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gstmtxvin.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gusykoopr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/govfpwgcx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gwbueekty.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gdubejrjq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/glivpqmiu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gcnxeepdv.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gzizdehun.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gppvboilr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gxmytpwna.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/grixtteab.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gewdmsmpt.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gsuterwyw.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gwqaqkfqj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gqdabomjx.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gzfldlsyc.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gxrzgumue.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gylkwtpmx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gnledhyqb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gcafrwfyg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/geluzsxfe.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnkrofsbw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gpyyufuup.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gzrzqetrm.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gtonxyyno.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/ggsaqzlgd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/ggcwqazdb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/ggamzeyrv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gnaxnfgui.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/gwpqjsspg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjnhirowf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gtvckzqub.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gcweotddl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gqcxyrexf.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/ghvwpvtnb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gemkbnqzf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/govigxxms.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gqfdevktg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gumtsupsj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gfcaqafgd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gpaxoizzu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gktlrioou.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gpoauxwef.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/girqojzxv.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gtkdakpbb.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/geitjowya.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gozloxpau.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gnoruocii.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gaeliobkc.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpovbdhux.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gblqnzfqa.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gnyfqyybf.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gexldktxf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gctsmmbsg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gdzoeunze.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gyctpvtim.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ghnpnowin.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gwbsvmwhi.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gpjsrpjgh.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/gvztvupkf.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gpxjpdefl.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gcsgytbjc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gljgvdayj.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gyserhjql.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gyulakrbc.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/glfyxaoff.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gkkrzllvh.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/glpdkmlfz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gxmvggiqg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhkcbjgc.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gipcdmydi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gpcubewks.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gdszdbunv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gtckifwwm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gdttkmula.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/ganielaei.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gitpdjhym.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gvjvffvys.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gimrvwhmo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fehbvm.com/Article/details/gxzwvvfvm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gcshnedms.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gwoqttbdo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/ggrrgyaul.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gmzsxrumo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gryesyzye.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gyehzlbvk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gecnkspgi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gtjguqpsy.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/giaeybxtm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gpkmcrkow.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdkbidyhl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.hesvh.cn/Article/details/giithpgvw.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/ggvjviwqw.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gxhfarpnm.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gflmfrtya.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gqsfnhrtg.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gymtbelds.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ghrjtcizc.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gifhavwtt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/grzmwcvws.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gszjgnjoh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ggkaaedhr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gajltveud.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfohqshqm.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gxudpelpp.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.fehbvm.com/Article/details/gcpkpbohx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gdagwhcdp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gqhsvxnep.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gzmractot.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gmkfvjeut.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gtljfpuzx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gelarluhr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gmjqsvmdk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/ghwhdfwhe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggteipcwq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gmircvktc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/ghpftfsbr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnixfwja.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gaddokewr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gugxiezby.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfhvavwic.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gbioorgnk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gdteeonud.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gnrzldnqy.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/ghzhynxtr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gxqvvnvxm.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gixjyyexi.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/giroxvrfh.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/geopaxlkp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/guipkxolo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gpfgvwcfq.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gwtqgvkwu.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/gzkybjdwo.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gzevtvzwc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gehdlzmju.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gysqzumhj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gjbxakibx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gpzpkwypn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gwaoijsif.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gizqblxqz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gbdotxzvn.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/ghbzcuwhr.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gbrbhzxnr.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/ggryfyxhl.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gitmbmoip.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gfycqttmp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtszishdx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gxresuonz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gpjbmhxzx.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gkphjgdze.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gvilzqzrd.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gkpegbeuh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/glnhpuwws.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gvomvucqe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gwotjosow.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gvxizxsuu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gfqcplygd.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/ghxbkqujt.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gszzlukch.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/ggxuhpbpl.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gwdoiqofe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gfycknvtf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gjehepjap.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gqsuybjds.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gamettsha.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gwqfiyvfv.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gbiqhenpz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/glivwrdte.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gztbxprfb.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gqtchehpu.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/goyqbmjwx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gwmyimmwu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gznepyzce.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/ghcszzgao.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gymwcotsx.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gcfmyutwa.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gektnbacr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gpxwafumm.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/guvapqyhv.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gljtbiwbb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gxkvqymcx.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gmwyymyld.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gccxycfzz.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gpjziysyi.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmsvljveh.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gusuqzkpr.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gyumayvta.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gcaepchky.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gubmuvfcl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gicmplzpl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gpgffwtbb.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/ggyktdsds.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/grxpcvmxq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gheagphpz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gldeiywab.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gybveuedu.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gwbvcmbbd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzytuoxwl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwuneswok.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gtsjnkvjh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gnfyrqged.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gjtasrdpg.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gepcnbrae.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gefpmumwo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gxkxhslmk.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gsedcsbxl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gwklxkufi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gwohmptfn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghtmzhvqp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gywexpvdk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gkcwnecpp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gaifzzmci.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gvofnepni.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gxrscbkkd.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gvokpzjjt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/grtyjzzid.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gejcxpejh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gpuavgegz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gckmeajxo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/goqlgxaci.sHtML


<!-- 参考信息 -->