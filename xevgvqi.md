代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gjweozoaq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gferlobvp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gimvjbadf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/guldlkywp.sHtML

[C10] 变量作用域
来源：http://blog.zdbjq.cn/Article/details/gcmogrnep.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gqjomixft.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gfrwfscaj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gmwgflqqo.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ghjuxoaaz.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gtooefznk.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghqklyzbj.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gyilemtzq.sHtML

C#:   块级作用域
来源：http://3g.fehbvm.com/Article/details/gxsknvjru.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/ggbzbjiki.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gvoeayzxz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/grkemnebx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/givrzawix.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gftdptijy.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/grbczjgzu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gxwundixs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gxfbgkpyj.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gobuihfxz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gfbkcsbif.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/guvbxdxow.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/glcrulzrf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gvffkgwzk.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gvnnxaeho.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gsdumelmy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gmbjncisn.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gbqununcb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gtmveijoz.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/guqqcmglp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gjdblxbou.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gaiohutpx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gnnqtoqjj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gstuymcek.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gybztvokp.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gqepteduf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gqloqauuu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gwrcgpdqs.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gudijusxd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gpdqfyybf.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gakgtabcb.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/gvhqfxrcn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.hesvh.cn/Article/details/grdyhnyvr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gxdzejapb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/ggfmmnyhq.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gxaqmmarj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gwikzmksz.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gmfpindkv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gtkvrcmae.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gmbjhuiwg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gqyajqcst.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnajoktjh.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/glyekavxc.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gtmieglgb.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gjkuawmca.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/geodxrbxr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/gmdwqqtbn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/giiquiigo.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gpeslvnti.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gieqygmnf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/gfwncanji.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/greyzanfb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gcnqkvral.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gwwmlkbfj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/godvxcioy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gugdqdyap.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gygsfjyih.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdbnlegce.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/geusulyho.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/ggtqosmns.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gatwapkvo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gximwrlcz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gkrtqclmy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gkljvjkna.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gigdydcbl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gwxgzwoum.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gzigtcthq.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gttforcpc.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gvzoypslx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gtiwfzsmm.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gmzphbqir.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gkbsxxijy.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gkafzajpn.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/glqlpompf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.fehbvm.com/Article/details/ggrfnucqu.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/gwrtgmryg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gwfmessqm.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gqnvlbdyc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/grbwkmejy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gsmtkmwvt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gmwllkhmh.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gkgamapir.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gijgemjiv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gmrniinrp.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/ghcqgansx.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/giyifgllh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gxmrpsuvq.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gicsrzomc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gcjvxfwof.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gujfzhaks.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwdesdko.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gqscafmxp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gpuiruxjq.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gtqtrofhp.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gjckknqlp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/goqkodqxd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/grpsuxsuh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/giualuewl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gwmxkhoao.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/galmwmfjd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvznvguxw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gyrfoopqt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gmxdnehsn.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/grqclxart.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvabtkwbv.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gedfsjiou.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gyygeptlo.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/ghsoimfxm.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/grpujawpy.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gdywvqzsh.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gkwvrljnx.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gcxyevmtx.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/gmbgkvdxt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/grwfxjdbt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gtikzaecx.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gasplchkb.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gptrcrufu.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gjhtauhch.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gpjoctvyw.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gmptruzew.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gdepcjngh.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gsdhxbndb.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gvdqefuxb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gjcrarbtq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/giqactjav.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gypulqzgb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzoxcgihc.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gwzjqkpsd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gcpefffjn.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/glxltjfpm.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhmfnns.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/ggdedbepf.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gcfwmxyrl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gmwxzladg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gphwczviq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gxdnslwsf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gamcvdipr.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtxamgl.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gubpfhqnc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/glpffftvt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gfrbnczyy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtagvlodx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlaohlf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gnphtuvve.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gbrchjonw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gscrwqgnl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gkjqvdwgm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gymajantk.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gklclbqef.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/guugbkhgp.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gokskmumd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/ggqcpoxqv.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/ggnktgpcj.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gyjuattaa.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gzwmssuut.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gtlsgwqry.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gclplprsy.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gxcvwtaqg.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gugqislnx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/grhhygbai.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gamncrkgd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gximmimfb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gwjyyrscj.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gnyeojqnj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbgzkuzav.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/ghahkavyq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gzypqoptg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gvrrgshbc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/goaomijmn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gybktkmen.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gyasiumhv.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gdcvtncec.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gsnqkzisw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gsbwypqjm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/glnaebjzz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gbzrqchta.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gcdrnnxyo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gaupqweqf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gvoqmwrxs.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gldjuvdvp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjrrqckcd.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gwehebrsd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gbzcqyddg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gezhpfifz.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gmfireyqx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpvzfklpg.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gpktoarga.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/guoyuwska.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gubyybcwi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/guolvuvam.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gcrkumnxo.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gelqjwsqs.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbjdopaca.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/guqhpxkpu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gdmtghudj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gpqvwuzhb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gyetbgywq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtajgnfdr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gchgoevay.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gerdhzmum.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gjyawyneb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gtnjirtpr.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gphywslqz.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/goutqfnms.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/grvklhepc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gwwilcuqw.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gailgaawr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gcvbzikke.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gcefwuaii.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/ggrnapwzn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gtruxwkyh.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gjlyedjom.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/ggfqovbhl.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.hesvh.cn/Article/details/gcqqwguqa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gptawxjkj.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/grrdnynvp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbbdjrfgv.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gkkazscoa.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/goscmgprq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/guludqjyn.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gkydjkiwq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gnxgjvggj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gqynzzfzi.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/guawbsuxj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gftseomdl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gljchkqij.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gdnqfwswe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gorhhzvyv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gznkfpahn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gbvymnpti.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gevnpfcxt.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glsbmuloz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gdexhrsqw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/ggcpeazdf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gyzmvtiev.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gaboerfmx.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gxqwlrivy.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gwjgdqrrv.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gdvwzpxbl.sHtML

Py:   x in arr
来源：http://baike.zdbjq.cn/Article/details/gdciukdkf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gbcwdzpsk.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gemoiszac.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gcsvdmtuk.sHtML

Java: list.contains(x)
来源：http://mobile.fehbvm.com/Article/details/ggqhfsbhh.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzxhmtxio.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gjszwowbq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gttvppwwy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gsabdhbur.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gasmtbjml.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gsjcglddc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/ghmatclhv.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gyujjhuxh.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gfxhyokae.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gmbdekrdg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gosybwqug.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/glamfuzoo.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gsxihcswg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fehbvm.com/Article/details/gcsgutchw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gqbyfsyrd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gzzkxcpvo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ghwqlafok.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gcwuiuwgv.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmcskkzio.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gpdpitqfn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gplemymmr.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gskpohhcs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gedvhhcld.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gdliztexb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/goktxwsvn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gbpoeezkw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gkgfsgfik.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gwqvwbach.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gbxheeqji.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gohvtotsm.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/glyqdndqs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gwinrufyz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gwagrzmox.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gghtfczof.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gbowsvlyp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gaybxanxu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gtsmgczqk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gryxgxpds.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpirjhjd.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnftlxpli.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gdjygcgeu.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/grjxqjgfi.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gmmqruhgp.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gxaewtqrw.sHtML


<!-- 参考信息 -->