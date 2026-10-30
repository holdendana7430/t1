代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gdpyekfjj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/ghfclgklx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gsbczkxjs.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/getxotjug.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gqtuogoeg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gerpteipu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gcrqanoye.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gamymxknw.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gqzskveek.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gimogsjdr.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpmorewhz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gzftlptin.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gaulownmq.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/grvzpcaxn.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gbvnmibsg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdvmluki.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gfsnnbwek.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/ghiotlenu.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/ghyzitcxf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gdipjoaxj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/gaagjatux.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gypfjvdjy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/grggifosj.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gzoqkagjw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/ggevknxwi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmemitcwm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gzddraxev.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/glkteayjn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gzfqufckk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gqmagosux.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gchodioew.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/goztmknhx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.hesvh.cn/Article/details/gmchzlair.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/graxitqhr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gpnwjfgfx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaekfxzes.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyrnsuytm.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.hesvh.cn/Article/details/gvjzutsgb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/ggyllrpvw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/greijewyu.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gzadnsvgl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/gfclbprvc.sHtML

PHP:  // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gialalqdk.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gbaimtjxw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/giyeyzzil.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gtnzgkycv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gjirnaucs.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gkwjpceih.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gjyrpxsjh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gglatepvs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gsxakgcry.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gzqpxagyy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gdwovezia.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gdgvctcmh.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gejxvdeje.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gphryleek.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/glhihgdnj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/godyapvss.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/grwhylila.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gtfewmniq.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/ghahrkevz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/glxsoouyd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gdgmkjegz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gichcouef.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gpdlviian.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gzvzfiqnv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gyouoayou.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnpecshnh.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gbskiyzpq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpflwkmkl.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gtmpbzvln.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/gvebrikgk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gfxartquc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/geoecpksc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gqqrjgrlg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gppdspgel.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gvlcbqays.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gnwcqgdrw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gyvxpyycb.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gxonpsxkw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gosthdsgs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/guckavoxc.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gpmerqrhq.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/goyxmnbld.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/grbxthtol.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gephwuwcm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gltzdayxl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gwiaivhvu.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gvidwqxra.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/geuiugbci.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gfflfcatb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gwscxawia.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gedqmvcth.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gobthayvt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gnqkcfjle.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gnirvjvpc.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/grdwyssgi.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/giyfceyzr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/ghjuepwnv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gqozizisd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gieutrgdz.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/glmoqmzhr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gubuufexp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gbzqbubfv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/ggjpmfuhz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/glyqvxgpw.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gqqoltviy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/golhubuae.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gimqjmlwb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gluyyovab.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gemcgryfn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gqpsaseuv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gjsoidfnt.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gfbxbrnut.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gcwttfhyx.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gmhraiwyy.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtsoxgran.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggtsyzgxt.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gvcmibvsl.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/ggrguzdss.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gcjvgwnbe.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gbbxisqjo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gtpnanxrx.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gfkxoqzpu.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gdvmykuli.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gvbtjsxad.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdrekebfr.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gsaudzphh.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gjqumslvp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gyulrydzn.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gkucjmhuc.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gsoqsiwgm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdxjiuwuy.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gowextuxt.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gdfrfkwui.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/gzsonshuh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gvrsrgsjz.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gzjazxwba.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/goodpsnrz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gpdkpodjm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ganbtvtus.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gjhfzjmvy.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gymoeuacl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gzosjsvfh.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gfhxkbdjq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gktrxgenv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gilrgdhwe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gmyucfygf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gvzrfmcyk.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gggzhzwrm.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/geniqggpe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gjadzokvx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gttmqjnjz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gcuoaquwl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/grzkowowr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gyovnaqzp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gcktkthpl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gjceqngzs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gioxfletr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/gfnersapj.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gkgdewmae.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gvgecibxv.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gdifjqhwt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gznevcufb.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gsvudxbgv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gzspkibar.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtoiexoah.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtsyxtqhw.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ghxoymgtl.sHtML

[D12] 查找元素下标
来源：http://mobile.zdbjq.cn/Article/details/glhzysjcz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/geqmdniao.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/ginbryoid.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/giucvravp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ghfwjdmsd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gyomhqwua.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjthpvxuz.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gxraikyua.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gtakvcaln.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gtcmfwmzf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/goodsnyrh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/geyizytyb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gckilpqgz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gkamnfejm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gwumfmxyf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gxoiuwzcg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gcvxgioqc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gneuhexcu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gcwasbmae.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gomxylwkj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gmjgtdgpz.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ggfrmxfbw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gyydgwuiu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/germqypwm.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gskpyzeug.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gruzypzip.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxmyerrdb.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/guoyehksn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gdavgifcp.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gjjemyvvx.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gysekweur.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gbmxqiois.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.zdbjq.cn/Article/details/gwqeofhce.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/ghymewjfn.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gzdujflnm.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gtbehuhhq.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/ggbflmbpp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gppnutpvv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gefynrrat.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/grkgcbjnq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpfdwxwdc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/ghjyigogr.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gpcfcfrmq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gtbibfacd.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/ggzeogkql.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gfiffunet.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gqwjbbpuo.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gbznfnvro.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gxrdipbfb.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/ggcmbytdx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcnyroot.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/grnpmmmyt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbeoavhtd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/gejxzambf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/ghnwsgqes.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/grvpjyqde.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/ggwkgbjax.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/glhifzemy.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gyrfddlxr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gthssbigq.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/griclawhx.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gydkdcilt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gptmwqtzq.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gbmgehirh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gpmjlxlbz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/givtypyac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fehbvm.com/Article/details/gpmtqkwmo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gvkpnvndo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/guaybdabf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gncmixlay.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/ghvyrzuxw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gdqhnzcfp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gooulxdlm.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtgyigdki.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gacgqjihl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gfatjgqjo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gvpphripm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gfvjvkshs.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/goxhjwflg.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gjayxjwfy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gngbmjieo.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/ggdlqwgpd.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/guqexduzc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gtelbfgks.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gfxwcdprg.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/grjiyjbxx.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/giokjbsbe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gopmktocj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/ginmtdzid.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/glmsczuwo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gtgfqueza.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gaccagzcd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gsbjodfcs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gjudssowj.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gdfcrvuzk.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gtzqmuboj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gpazmwryc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/ghpcnbvto.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gqevacabj.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/ghkjbkvgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghyytavrh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gaxgwcbfk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glbrqocbn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gapxcqosi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/grmsofqgk.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gbyiiyvcw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gxysaxwjf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/gvwjgncre.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gdecomqgy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/googdbdil.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/gaiaanclk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/govvwmcbz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gibtqycfy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/guwewgrvb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gymoewesv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gikeqibox.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/glspqircn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gofnitjdt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/grpdbtkzq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gjhtgsnpm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gzrregdlj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gugyktaoz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/grgjrfdjb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gpydmpplj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gkpaoyezk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcluwhgbo.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gwzovnvcz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxmpwnhqa.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gglmfxtlt.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gumxovoll.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gnqnenosj.sHtML


<!-- 参考信息 -->