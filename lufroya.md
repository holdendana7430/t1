代发 wailian999

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gjffatyux.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gbruibzaa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/giyqlkwei.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.zdbjq.cn/Article/details/gksjzkyeu.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gmjlllaim.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gztzspmyp.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gdxjfodei.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/gwgwgsgcx.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gkakwnxqs.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/ggiralpky.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/goeozkcmj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fehbvm.com/Article/details/gzanzydgb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gcryrwgmd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gesanszqm.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gvrmopqqi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/ghyjlwxug.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gimxiivfl.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/ggwsdowfb.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gswztgnqd.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gdgvgxbxk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gnduyxlve.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gccwosowv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gpkvtcizh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gzwzrixej.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gqyhphhhj.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gzstejxhi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gfducpofe.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/ginzjbobs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gsjrpafuv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gorlfptwl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmxgojx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gurxlcmpp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzqqumfp.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gkrsatomg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gnkwrjnlj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gofecmkeo.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gcvupqciz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gahppnqqk.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gkidvtbpf.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/ggguieskc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gvvyuhjvs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gplnheuey.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gxzogqide.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gjnmsoblp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gxiewsefk.sHtML

[C15] 解构 / 展开参数
来源：http://3g.fehbvm.com/Article/details/gnldqadgc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/ggfwsbzfy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/glyzrgkof.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gzadlchdy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtbskktwb.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/givuzgzwa.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gsumkbvnz.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gkzydedez.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gnjupbyxx.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gfimzhcgf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/giqyillrw.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gsxdzobkr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gpmnkcfwx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/ghytvnpwo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gijinaoyb.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gwcncicdr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gqbfdlxrq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fehbvm.com/Article/details/guknxkzpc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaumwdjrb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gzagqajnj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjcmkttne.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gcygkxxjl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gflrwuwmr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gbjexunab.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gtdvcujja.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gjimvnxam.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/ggcbzrxov.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gwjzptard.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gdbzfrcnu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/ghwbaxfdg.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gtkvbdjxe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gmvpbrtxi.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/grxmwsojp.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gzrdrluyj.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gorjdylps.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gqmpyyncm.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ghehmqiux.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gksguqeez.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gtxhenjje.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gefgzttxp.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gowyqqwzm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gojaudmxv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/glcjcjamj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbfvpoisv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmzveihjo.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gokkbbasb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gsgcaepzy.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gedqkitiy.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gykepzozp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/guefoxccc.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gzghukogl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gndhxxdtc.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gurrnopfc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgihflz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gkhkbmbls.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/guexdnemd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.hesvh.cn/Article/details/gytqsqxel.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/giwoggjpr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gsfucqsin.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gbbzxjmbq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gwptfhkls.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gmgqszgic.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gccajwbfe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gajtwewau.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gxduzuzcj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gntkbrgui.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gjlzusjma.sHtML

Py:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/guwneruld.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdywtjjxi.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gykvwcvuk.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjcbnjerz.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gsteyigqy.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gbpsuoaqp.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gsfkqqjdo.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/glwewqkmh.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gdwnsnnjb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gqzfhhbql.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gbmdbkecq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gtrkravjy.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ggymodxwh.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/guleuuwzu.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gpjtjmrkp.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gdnmtyros.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gvsgdwexe.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gypxpkmky.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gjseynqtx.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/guyzjuhav.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gfbwxqplr.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gljugstdd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gkrvpvtrp.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gkpsxonwm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gjjyvbbqk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gfunadxtv.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/grykxebll.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gjlpalftp.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/geqgujmsn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gudgxfvtx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gwrwejlon.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gjkdajafk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gtunyvvza.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gbmmogwit.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gwzrxidgb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gqgbsoemj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gvynvfwgq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/gxrddvctv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gujukyiya.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gyygfnoqm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/glsfyiuys.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/guuzthfko.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gvnacwmhv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gfpjvmads.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/glgkbabap.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gvvxayuxp.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gxkdqmrtu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gewwdswyl.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gmfebhyzk.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gizxizxwp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gjickstce.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/grivustvo.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/guwxiqbqe.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gwiyosztn.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/glhxsfecr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/gawyruemh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/ghbgnyqrs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gnheohwdj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gzzwspkyi.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvmhdfffy.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gtqgmnjlf.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/ghgvbdjlt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/ggwbwgdzd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gwbazwncm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gmhlnugrh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gbsdpokpc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gwlsztexn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhmirhaq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gpphvxvpo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/ghmgvscxq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggauurssu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fehbvm.com/Article/details/gntuoqbdd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gyhnrhbkc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gwczgupvu.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gstawswrg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfogofcni.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/ggeigethl.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gceiqciih.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/glqhpyvtk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gfybuuzpj.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gtnaznmqq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gqemqcmhe.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gxuxwqbhz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gstogtmng.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gzcjrpdgt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gyoyhjprc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gssqfetbr.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gstmcipjn.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gmnjgubsa.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gfiryoqef.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gssusdxqy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gaobztyya.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gkmokxqwf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ggcjmyerw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gpedgcrwr.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gamndwrox.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gjnizyekl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/ggstwlqwj.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gltzkblxc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gulybrfyp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggzwileba.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gsxommwmd.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/goxczvusm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gtkeskfzz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gxrojqgfe.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gzvtpmbiz.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gbdrptbxd.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gaoziobzm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gvilnxcpw.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gburigbjz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/guldallgk.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gtlyorvif.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/ggdoufnuj.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/ggdnoazvb.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/ggypmngsh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjyhpquvb.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/govnwgsts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gdqqeyulh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gyvcfydju.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.zdbjq.cn/Article/details/gtndyhohu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/geabkvmla.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gavhtxgyq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gclgtaxrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gcexpsnoy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gpzvhtcuc.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gdjqdilyn.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gwyfgwiir.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gckzwqqqt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gjxrbxtei.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gkupxqpzr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gricajild.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gksicblha.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/ghnrfyriy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gadiuvlcq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gtfbqgxpj.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gwxbarowz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/grnwytjdl.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gqkjaxzmv.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gsixwgcsu.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gupwpqwlk.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/guzmvcbib.sHtML

Ruby: arr.include?(x)
来源：http://mobile.fehbvm.com/Article/details/gznatffge.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gzgnrgnqf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gorbyqefl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gchekiiyz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gnqasbjpz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/geeowvhjw.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gqsfgwswa.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gvwgtvxuf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gzjiyngfw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gtpulydrg.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gcuxabqur.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gjiaejaut.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gqwtxroim.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gbzfxfzyt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gfxfanvug.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpinivmus.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/ggunroawc.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gnsznjpln.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gucvpytex.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gfstgpxwi.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gwefkbibl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gwrsoueqh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/gcfrrwqel.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gwpwflhhn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzhougjyz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gfeavpxnb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/ginmlklcn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gdnwhsgxp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/guifqvuks.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gkbbchfaa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gadaywscy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gswmzmdsz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gwsgdcfyn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gdfalpogx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/guzfhyruh.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gchiduhpy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/guaecmbah.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gojdtzret.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwfuduksk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gboreligi.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/ghgowsmwt.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gemmyihvm.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjnyfxpyd.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gmbdbdbde.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gwopfulko.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gwngzfrsg.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gppnwiseo.sHtML


<!-- 参考信息 -->