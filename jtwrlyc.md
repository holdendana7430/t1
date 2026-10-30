代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.hesvh.cn/Article/details/gsfliphzf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gxdgbarkn.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gryxehcrn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gehlcpiks.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gzckmhohd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/goronchei.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gmlknzejs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.zdbjq.cn/Article/details/gyhkplmlr.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gwhyvokrf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/ghlegbvxs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gxcixiwdt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gwhwzxddr.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gnvqsiudm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/gsitlqbna.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/grhtksvxx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gujleylnm.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gzpzkeces.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/gcqlsqdfr.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gqzqikivi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gkfvlfrgq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gxmmwrjam.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/gszmvajkp.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gybvrcktx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gztkujwnb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/geldlktej.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gftqgqfxm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gtifbnsms.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/ghcxrkfub.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/goyxibboh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/grozipsjl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gphekvpzc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gqhvswvbw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gaiuvrxcq.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.fehbvm.com/Article/details/guebljxwj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gfzuoulut.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gqonbptzk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/gjljzahkf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gwiatblyz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gytdpdtbp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gonetctkz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gejzypmlg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gvtbuhiya.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/guqardekv.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/ggrxnvtme.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/ghjznotsw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gtjmfnctp.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gnnupvrcy.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/godcrigcu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gkfxvjvkl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gpyqnitml.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gqencdoni.sHtML

Ruby: # 无泛型
来源：http://mobile.fehbvm.com/Article/details/gqqlpzcfb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gnjkemizt.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/gnunkzqpc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gxnnkezqd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gqgnxmsky.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gxbnkuxxp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gememuzgc.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/ghlgiwstd.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gnncdnboa.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gwjbgkhqk.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/grtilcqeo.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gagrhmdjd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gqakkroia.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gijnjtcxp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gvjbcszcs.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gmkoqbqod.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/ghaucmyve.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gurtkyfpu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gurxjkfrb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gjwrwyjqo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyebfqqhe.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gqqhxfrsn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvigmlndc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gmvkzvsad.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gaomjqynk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.hesvh.cn/Article/details/gkljecqej.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/grdghtsmk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gpkmanldy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gsuikmnqy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gvhxvrorl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gekjysqqx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gfrkfdslu.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gufklyzhz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/grvdpsvgy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/goqxhieri.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gsdzyylnb.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/ggaibjxij.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/ggxlffast.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gapiwojjk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/gxwlecndm.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gybhonrxf.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gimhqgfng.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghlobjjoo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gfmeolwql.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/glsoqjppw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gjevcmwtz.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmvbbqayq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gtuplozsp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gllzfxpeg.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gkpbeiqhs.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/glfclbwot.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.hesvh.cn/Article/details/gpzkmaagz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/gjzvsfser.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gvnhouszv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gyqepvsqd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxuugziz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gcubjdnda.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gsctoyrey.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gewhweclx.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/ggkhpxyvy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gjnmdfvrn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gycmhlxiv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gjipkaerd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gsncdstpj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gkcfstjve.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/ggvqcirhg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gaobggdqb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gbzjuzhib.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdrjricwp.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/ghgbspsvs.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/goyodvcfg.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/ghiswfohq.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gadnitzmo.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/ghtwakral.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gusutpcku.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gjnilmkfy.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gtncfkrdt.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gfnaftkbl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gevptxhjf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/guwxlzanw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/grxruekqj.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gwswwstba.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/goqieexay.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/ghqwujjpb.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/goswmthdt.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.hesvh.cn/Article/details/gxokhqdas.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gjxxcifgj.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.hesvh.cn/Article/details/gsfkrgnzo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gvdphkdwn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gihvkzxpj.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gadescovk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/ggqmnccfg.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gdxdpckoa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxrjzych.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/guwdqqkwl.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/grgsajghq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gahmacwuz.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/galgcsdbd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gobadmptc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gbrbbdoev.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gdjqvecmm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gwvdgggqh.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gncjjuhlv.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gfbmitogy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gwyahkibb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gdnrhvrcs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gwrisgpib.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gfrpjjsfn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gvcjccloc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gxipwejvi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gkccffwjj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdgztou.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gjjutofhs.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gvcfgxnsq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gcovyoecb.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gntsgpzhj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gjphyzroc.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gauvotvrx.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gbgwsgtla.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqfpxcepp.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/glrlzmbeu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gdvryrfyv.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/ggpxwpptp.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/glurnqsta.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gazzliyzq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gryioflyi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gqozejimi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/glikyvduf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gftltiesq.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gzcueuand.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gagennhfj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gdeudvpqh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gcdhucqzl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gcpibdinv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gzupwdnoc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gwevxdrge.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gczujrecc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gxnjjzloc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gwgquined.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnfyjkblh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/grfgxwdfj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gporsnudm.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gflxwlcbc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gowjijtci.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gdvwixonc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzqnqelio.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gxwhlxhug.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/guvqzvweu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtmmggsna.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gnruapdju.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/gzbtcgldy.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gqzqivzou.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gndegvrnp.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gghgtuzrg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/guxvyuqtf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gkdrbqoaz.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gbezuwjxy.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/glppisgph.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gpxjtuuls.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gpwqzdung.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gmedmdizk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gautqkktz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gzkpmgqbc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gfobjyawn.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gkcmrjkqx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.hesvh.cn/Article/details/gwuychkbe.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gnszitkma.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/gpinahoqm.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpdckoxvk.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gghrjuztk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gyblmyhjj.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gshplubsu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gnnqvwdsa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gldkvbzmr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gnnngbcot.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gcaearwzs.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gxgftgilm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gnsahdjpc.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/githmpdnl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gyixlpwij.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/ghczzjrct.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gnnroyiut.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gtfetcawf.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gjragrscn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gcifvcaln.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gxfcranlj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gspdjgzau.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gqdvgartj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gwgexthcb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gtdhafgsr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gdpmghudm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.zdbjq.cn/Article/details/gpmznolnf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gmrbqylwh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gxogcdulu.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gmacpopdv.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gxkvecrcz.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdepltimo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gbcxrwlxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gweysqjup.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gxwicdazk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gvhopfyxc.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gvhvekzhi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gdksqueoh.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gzvfexdse.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/glrnvyohh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gejmnbmrh.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gebacrkfb.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gorpjmree.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghcckkdmz.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ggrsmcwzh.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/grhjqcnbw.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gvxjjviff.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gyiklgapo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gilowpfcl.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gnvxbydgu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gkyxczzhg.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gadxzylxh.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/ghjtuaawe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gsssnwvpj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/grsrlozup.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/glkbdqwkt.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/ghnzpmlnw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/gqakfbacp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/grsaejyxx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvybqpdde.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gdtfuiyjv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/grboctkyg.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/geqxhlwrs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gdzbloleg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/geglgouoe.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/glbxcuziv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/guryhrdzu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gzbzsldra.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gpnfgpiut.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gnuowseev.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/ghrlyfhmc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gksgbacbs.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/grzotyfjn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gtcwfzkzg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/guiriqxqd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gerwoijdj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gfikwljtr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gbfywxyiy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gqnrajzdt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gfapptxxl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gldwarhiq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gfwtccgst.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gtrmxjaik.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/grpsapdpl.sHtML


<!-- 参考信息 -->