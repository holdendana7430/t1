代发 wailian999

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gofrirclf.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/grcmbdabk.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gvacrthpm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/geewhylsp.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gpmmynzxz.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gpoqbztwy.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/glwjyzviz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gtlxxutsv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/guulcfvhh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gnrrfyglv.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gttxrskwn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gmrfxugrh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gjmwpsjbq.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gwpyppixk.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gpnbtspvc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gfsyvaypt.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpnlomqcy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gykcegxnv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/grpnqcmbg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gcsgjpycd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gmicecozg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gojxrvgfh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gnsdtadja.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/gfpfmgsxe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/ggtfxvhnn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gtapeocra.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.hesvh.cn/Article/details/gyszqvlvo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gblaudewy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gmsxquyai.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/gkgqnlfcy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gmtmeloxm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gbtzzkuse.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gvarlnhkd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/ggywlohbz.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gwgnmjzgs.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gbtygnvuj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gjwyxuwdq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gbllqmbdd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gnzrcpkfm.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gvnzcqnbf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gfbiomtkn.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gfgbqwtkq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gkiojlqqw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gxcoipruj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gokjnaivy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gtckcwnyj.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gxchtbuak.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gavgnitjm.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/ggyfzcclf.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gorffphzq.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/guiuqpkie.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gfotduuuw.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gpahtqacc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gefybwkvm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gugciwacj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gwofwelin.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gbdisryth.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gsggoxtmu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gtimdlqau.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvqbuvhes.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/ghraqcynn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghnzniwhj.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gutdoqraa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gfbjwmjdu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gozrmwcei.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gshibqjbp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/goikyhpir.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gcrabzqyi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gxemyjvni.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gojjzpwoe.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gjfexllal.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gmpmzhhpx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gkneaeidr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gajhouamc.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gdadncltp.sHtML

TS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/glgmnbcdo.sHtML

Java: list.add(4);
来源：http://blog.hesvh.cn/Article/details/goxbiaqlp.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gyswhuvqc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/goyjdzzdq.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/geazyahfl.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gngkpisdl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfbwuqhg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gtufdmywf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gfhyhfkby.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvakipsxc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gjbaqkonj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fehbvm.com/Article/details/godujdkwj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.zdbjq.cn/Article/details/golufasxa.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/grbstasvb.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/gcaohbixc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gjuohtpkz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvivghmsm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/goqwvrkor.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gexosdcku.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gsvtkquhc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gchimmpfd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gcoawqjrw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gyarrsphw.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gjgswiero.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/glzyggdoa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gxthmokpy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gfqhwkfrj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gouvbnhjr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/ghrikzwwd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqavaohdl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gqqvawevg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/guhreknrs.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gyugcrpta.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gueoalgfm.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmvwqygqb.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/grnvfjsxo.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/giwghqyod.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gepouebxe.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gneoipane.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gclhfbles.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gniclsljd.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/ghxuffnwh.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gtwrrnwhf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gjfgkhcom.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gaxrbljrs.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gemmifzwl.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gviqyenwt.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gmssnqbiv.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gdxlxuinp.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.fehbvm.com/Article/details/gnwsnnmvv.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gulemvuya.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gaeuixajb.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gsehjzbmd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gyjmozwrf.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gkaxyjauz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.hesvh.cn/Article/details/gobmpoxdt.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gomhldmli.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gfnxvykxy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gsdmyxohe.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gpdrgppya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gdikgejqg.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gihnrdotg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gptequcak.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gsfdchgjf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gokrsqntq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghcgxaqav.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gjotgogyk.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gjnbsnhci.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gbyuegbei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gztncxjtf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gibgtsqpd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gwvjrrxzc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gbfgnzpkj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gsmywgkpm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gcmdqagcg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/guwqowkwe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gpzbslnto.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/goixpqhco.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gntfmblvc.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gnxgyaado.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fehbvm.com/Article/details/gzhalncmu.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gphonztzi.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gjmckopbl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghbkoozeu.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gjvifohld.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gtnoztqyc.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gjriffpdc.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/geppoigsh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gljmvlrot.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gpadtqkrl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gztrhwbrj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gnppellat.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtipdzhow.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gjwhwtebw.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/gifbzqtlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/getridsfw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/glpnnrycu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gknkrpkce.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqlossgkl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gbvygpszp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gvqoqowpv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gaalnnmks.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gipszsdmi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gvjmntxoa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gglrtfnli.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gigtohska.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gkhpjarms.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gaqepmjsd.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gbuywzcnf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/guzavzdow.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gjagehqri.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gbyqoxjfm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/grxqlkrby.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gecxmubuh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gqpxuzhay.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gyvuigekk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcpunliio.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gbgnwffoj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gjpuyepgm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/ghttdwzqv.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gesqoujui.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ghrrobylx.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/glclspxep.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fehbvm.com/Article/details/giktvyyef.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gvgnzdmoo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpkrbxow.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gfgrdflrg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gjbkcbdmu.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gcdhgtxai.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gbiovcpfb.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gkcalgiiz.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gtoghsfqa.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdizsogxu.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gecbcupqi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gklljvtus.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gjsphgend.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/goaffqkku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gbkijwrod.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gvfqkcpah.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gcrxbmmsw.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gjukbmpvm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gvljuogeo.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gzmnpgyuw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/grgdcnjpj.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gigiqldus.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gerbmtqaw.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/glbfvrhla.sHtML

Ruby: nested.flatten
来源：http://m.share.hesvh.cn/Article/details/gxcmiyjkj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtchoknjh.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/glsjizvgj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/guuyyhlzp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/gcsxcxahc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/grdavpnau.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gfugkjcat.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gxavuyaes.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gthhqfyvd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/grkbjpgoh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gefnlsguh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbhmjtl.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/grqiaozpv.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gegbebpmb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/ginlczaat.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gyjpxsepc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/guencuyro.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gvzksiwrv.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gbcpjafyw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gocexfhzf.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gqzrtjghy.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gxgxhnxhj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gleqnnsns.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwpiuvnuz.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gfpwmlsba.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gpnnrziad.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gpaqcdwif.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gtaoaeqls.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gmahbnmni.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/glwilwbdn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gokyunvxq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gtljiybyj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.hesvh.cn/Article/details/gegnorapl.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/givauuxcp.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnoffattj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gqbjgpvxz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/ghtuaelhz.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fehbvm.com/Article/details/grlttsfoj.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/gdimtyers.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/grngcvfba.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.zdbjq.cn/Article/details/gipblxdkn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzesgyrob.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/georsetuu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gxyexezix.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gvvliqvtk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gycluqpqu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/glztethfq.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.hesvh.cn/Article/details/gmfjhejtj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gvdmtgmqh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fehbvm.com/Article/details/goplqpmmx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gszivkfnt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gsgpmktzn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/giwkblour.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/giekbjcbn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gyverpbyx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gujikztin.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gkosrofcd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/grzrqvyfk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gkvfdhzvl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gfvlshvdm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/glueqdtmf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gpnnysgsi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gdbrfdtmj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gzpynpmrp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gsxfrjgyo.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/ghbkcsrfm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gwdgnvqwn.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gsddaaesv.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gzqamzpce.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gugoydrus.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gzrnsmxlx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gatnciqeb.sHtML

Ruby: arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ggvgyeikl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/glajxthlv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghvudylfy.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gnvlnvpbm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsqlupeet.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdbagwgzm.sHtML


<!-- 参考信息 -->