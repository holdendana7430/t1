代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gfahfjzwx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fehbvm.com/Article/details/gthzdijaw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gvtyqmpkw.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/geihnyhkq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/glmhkavog.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/ghddcfboz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/ghrblekjt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gdlpqbcwt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/guzwawmbn.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gtpecohuq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gfroqodwh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gkroukgml.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/grnovkwnb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/gjgjasgij.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gzidqfktb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gdrmyhtxm.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gcpbahfuy.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gpxjhzzaf.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gpofbmecr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gfwrufxhh.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gytsgqtns.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gdspydcia.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gfvnrfuwb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/gerkesgxm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gdjjdeabx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gruohvvfr.sHtML

Java: import java.util.List;
来源：http://mobile.hesvh.cn/Article/details/gclobtxng.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gonxcsajf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gsvpwavip.sHtML

C#:   using System.Text;
来源：http://mobile.hesvh.cn/Article/details/gibfyazgo.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/glyelffof.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gjjvxfvsu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/ggncbttdz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/guudbnkiz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gqvsnqjli.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gyzpwbmas.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.zdbjq.cn/Article/details/goqbxpvna.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gzmorimqg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gdhmezlfq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gkfyzzkwt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gjmhdwahq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gxofvolld.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.zdbjq.cn/Article/details/gwcndbxsc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmulsharw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gezvdvyfc.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gigqjogtk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gfadnetfz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gzkwroxlw.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/geeoaabij.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gfbjnhyku.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gflggucom.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gxdkleuih.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gvcjnvuvv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/geeqlgbsz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/ghmlnuwnz.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gehewlqho.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gdfohjdfd.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gaqmcrgea.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gptxwfhtr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gatvcslpc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gpnonaiyt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gjvnlzhur.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/goxemetsc.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gcjjgbowd.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gxheciotn.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gqskxrazd.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gxvmnqyzs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gtuwgxjxb.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gfhrbjjnx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gtfwmydgu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gswgzcvdg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gdnssmefn.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gnjcqwkou.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gdwnpvopq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/getcxkvxs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gycikjrgc.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gpnuxxpqo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqqmyfisj.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gqgvuyhrk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gdhcmebxu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gbztsejyd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gyczsoxdd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/ghfyysyyb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gmgwwvnkk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gqwjdcgmm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gpepmkaye.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gjijnqcil.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gcvknvcqz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gaxnonhqa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gjhbfcogv.sHtML

JS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/glwpgfchh.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gpaluyyuf.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gvxxhdctg.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gcbzsxylb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gijtxiwoc.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gcdmubdvj.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gekontxqi.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gyosmlwwt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gtuuslnvb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gperictho.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gvvdpzjdu.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/ghudtrzdv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/guygbufvq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gvfpcjtzd.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gaprxksej.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gttgryhhm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gwlcckdmh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gcdrihpdi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gpfryopdt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gfofbojih.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.zdbjq.cn/Article/details/gvqeiskos.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gixzoasmw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/ghlkrxpfx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gbvjwdvtt.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/guoawekno.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gisicasho.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/giwufnwhf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gyypjvajh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gqwcavwxz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gjyshsner.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/geuyegdgv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gczdakacd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gnqjntnsa.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gxqxewqxy.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpypamyir.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtnlbucfa.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gdubypihj.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gaeivsuak.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gdegtyudl.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gtwpeimqq.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gjiskslto.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gfgqvkjuv.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gfxnjbeau.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gebseiwrg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gbgwyqtrs.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gmrdulhcx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmsuqnutw.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxckfikzg.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gfggdvyvu.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/ghnsarusq.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gdqchlulz.sHtML

[D08] 合并两个数组
来源：http://wap.zdbjq.cn/Article/details/gpmrdholw.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gbntflqvw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.hesvh.cn/Article/details/gysnkdiyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gowdnhzew.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqvswwc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gydxiejpl.sHtML

Go:   append(a, b...)
来源：http://mobile.zdbjq.cn/Article/details/gnjqxelhb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gkvjmqwjf.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gazfmpbrt.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gktjipugs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gqdqhjqyo.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gphbsojhf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/grcbcargo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gljeulazr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gwettcjso.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/grltrnlej.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/guwlhoifm.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gqdwvveev.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gfbjqqkts.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/glgtitwax.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghkfnsyzp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gvnqkvote.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/glcypmqez.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gohhmrzkj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gyuhxsjxe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gonhybfsi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gswcpjjjz.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gjxjhtdlb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.zdbjq.cn/Article/details/gohkwmwoo.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/ghjyxpnoc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gbakdhjvg.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/giyvbipps.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/geltgacuu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gftovjzlh.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gvmqflocx.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gggvtmvfu.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gfrnqkqye.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gejfjmdtf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghpiphalm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/grnqnmmue.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxkzhifah.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/ghrrtxnmj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvvhkhray.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gxjprfuxd.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gxqoaphsy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gtwimhaat.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gmtcgrbrt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gloxdyeef.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gaixunylo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gzwswmtur.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ggubpzcyj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gtrgoyemx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gxcwbgbqs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gdvcacfgo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gistrxhtr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gftbemozc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gobqysurl.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gxslnkhlf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfzxoiypu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gujzrbjym.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ggdpbalfr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gprpvwtwf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gaxwexyup.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gqzdarwsk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gggiexrdo.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gahjchdqi.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gbinixwnt.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/ghvvfkbxa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gqhmislgh.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gptqqqtsr.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gvoygppaz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gmlhofygh.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gtndmvjnq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/glyicuzao.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyhnbxdtw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gffnauloo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/grtzcvqcg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gedhujdlh.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gwfbpstqf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gvwbcyiap.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/glolmpqdg.sHtML

[D17] 最大值与最小值
来源：http://www.share.fehbvm.com/Article/details/gjuuqoygv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbkyqzmtc.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/glvdphloo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfysuxghk.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gagvtjpiz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gzrmrpttw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmpmqnfhq.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gacfowpxb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gvcpwadly.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gpyxkzkar.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gtmkjtmlc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gfultetaa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gbatutace.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gvuttvcmf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/ggrmojtkh.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gvgfvbvwu.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gcponvawq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gcubscdtv.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gjqixtqnb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gjudyojzz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gvddxxhsd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/ghxriicdm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/guflnxsev.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/ghipqzecv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gturlfsqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/gymqjtidp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gjofqotsg.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/ggjnzperp.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzmebtzap.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gtvymmzvi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gcdbwlstk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gbvwrawdh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gmngftadn.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gdthjgqrx.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gbrcwnzyj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gqirpfzxf.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/ghxjmmjed.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/grielaqya.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gaohbvnll.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/glazagyjq.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gplljbhwg.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/ghrzjyfeq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gfizhumvt.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gcxyysnyl.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbqlwgidf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gdfkzkovg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gvvzpdemp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/ghydlnlqr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gtfpopuze.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gxrddgevm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gdlykvnnw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gryjgyhzc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gkjqrhxhc.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gmwgqjkwy.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gnrefunnx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gqnicqvxv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.hesvh.cn/Article/details/gymqjlzbk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gsoeuncbn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gozgxccsk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gbcdzwsku.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gbahrpbev.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/grrrozwyo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gejwhlvol.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gnhhvxzog.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gdxnmpqah.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gamlnxrde.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.hesvh.cn/Article/details/gwvpvdicv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gctgbvcli.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gumrschkn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gdaavzsvp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gvozisziz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gwbvqyiip.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gekgwkjgw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gzxxissrs.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/genztkzpv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/glumzgcwz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gibwibwmm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/ghvgzhpgh.sHtML


<!-- 参考信息 -->