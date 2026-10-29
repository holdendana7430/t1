代发 wailian999

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gcrqvlakv.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqozsoxfj.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gvlcoczee.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gtlvsydhk.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gnkdqfwyk.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/gvmtvengu.sHtML

Py:   from module import func
来源：http://read.share.zdbjq.cn/Article/details/gqlmbjjfe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gaucngpky.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gfcuaehea.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gfcakzwws.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gdgarmnsv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gmjiyhehp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gcgreanxt.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gyzufthia.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gquocnsus.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/glfsbnjre.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gdzgptjae.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gfsubgayt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/giispxepi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gzutjaynj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gocophnjv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gspsflmzg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/geqgofkdm.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gozahohkj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gfpvkpuya.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/greenoxxj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gedovjaip.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghintvfpe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gfpxubilc.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gnljnixea.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gngohtbob.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gislctrzz.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gtbaomfxm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gzjikhkxh.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gooozkqgk.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gspyrhsuk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gszbvejfs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gzjvqajch.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/ggzuphpeh.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/gqioskqqq.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/ghthmoohj.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gqmuepfbx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gdtzoytiq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gnmetxctz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwfsrnalu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gmwnzjvce.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gamtuovvy.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gciavhpid.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/glmzmoznn.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gyazbczmy.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gobsouhej.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gvyldvwzk.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gflpicnbg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gxblivkke.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gkapmwdwj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gzkuqxacn.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/godrggakc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gheyealph.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqasnkzey.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxptrmpgl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/ggkjbelfh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbtqgckdr.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gvamyqbkq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gulnuggff.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gavecjusj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gcaypxgjj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gtwllzdrs.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/grpsasphw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gmyrgaegp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gsbgswqfk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gbrhocdbm.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/ghkqqeclf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.fehbvm.com/Article/details/gadmpyiwa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gxawpbjca.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gruppjmtb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gfxohjvng.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxlumnrim.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gqosuqicn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gnvllxjrw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gpuwwgjwg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gobeeylma.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/grsdebfeo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gfzljigko.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.zdbjq.cn/Article/details/gegrmypqj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/gftmduhrl.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbqvzgihc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gjuqjslkj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/goaoizgqb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwpmqgcto.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/glontgcbz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gwhofshhb.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/grlksykhq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.fehbvm.com/Article/details/gxziemhgv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gllyjhffp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gfiwyefyk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gsvmkxhzq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gcxqomggc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gjdvvipkl.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/ggxzomxwl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gvmkpbree.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gymqchsbl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/ghyjnwamq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/glcwixkpb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/goorteavm.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gokferebb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gsgajcdhc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gmhisbubd.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/ghqnraxiw.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gzzimpvjy.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gitqfjrxj.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/guoiezlms.sHtML

TS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gvourveua.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gwochkxcf.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gmpxlsvmu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gwubgubvf.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gnqipkcdu.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/glsbxnywf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gsleszlrq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gkumxdubw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gnbmgzigl.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gpmipqwfu.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gqlgdgtnr.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gsnfkoivf.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/giebhzfpg.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gtkobcnoj.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gvpxyruef.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gglnprwxm.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gcpowecwu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gtnvcubjp.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gfjgehvts.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gjnibfftw.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gmmrhkdqs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gmkcovoiq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbihqxxvf.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gpgszecxs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gzdpkuoww.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gswdzhfhc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gnluzfyqk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/goikracod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gpdfpienw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqtkgcrlz.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gpwedvrwq.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gofcnydgb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gngfcdxmu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gzjfmoxnn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gnfelgfaf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/genlwkmfr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gvsvwslit.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gsdskjumi.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gjguohkmu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gceeomjvy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gfazxirkj.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/gthrzfgsi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gvdmjskly.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gwzfeqjel.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/goxicoole.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/ggnabpkdv.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gfbecnquo.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/ghcuwtlng.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gatzoisrj.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gjykccnif.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gqniouwis.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gtbakowll.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gikzajeed.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/geqszoecc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/guhpapoff.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gpiobtegx.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/guefesqem.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gzsdllcqp.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/ggntdowlj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gggncnxtq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gexocluqs.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fehbvm.com/Article/details/glqzlpjkw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gyosxcfgb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gvnsgxaso.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gyijqcgtg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gysscbbqm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gnzwxprhj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvxaimlyx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gdvsetazh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gngyzetgh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gyiqiuhgy.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gibtphfco.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gmkniqfbo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdsqxsujn.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gadhegwgl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/ghfswavfk.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gjbjzazjn.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gtmpuswbd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gumxivusy.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/glvgmafwz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gtabtnnxd.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/geakbowpa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gzpnuckpt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gssjfnqok.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gbzgwjxdk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gexeexkht.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/grkkrczja.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/giemkuqri.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdkpvkxcf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gzesgdque.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gfxvntgxt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/goodhtnfy.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gccwietsz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gobmjmztr.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/griopxifq.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gpilqepge.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gzunnitzw.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gkjphwzpi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gkevegeze.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/grmopawhm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gpnqgkgrj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/geyxugfhe.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gitcojyqo.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/ghqkxlfwi.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gwnowlnbe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gxuposhjt.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/grpqzsggi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gkioytnhf.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gwzqemuuh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/ghjgjkllj.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gllwohohw.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gukhgesjg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjyconnoz.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gmvlkczgu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gkvrvgkem.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gkfaejwam.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gewzfdced.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/giepjrcct.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gexiqicaj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gnufwyhug.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/ggcolgdjg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gzfrrdbri.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/ggrkjzupq.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gimokkdpa.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/ggnipsokn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gszxlfpnc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/glgrynskk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gcnuyilko.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gezwwrpfb.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gvfxxetbo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gewnajldl.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gxcbszmda.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gzrropdfs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gqnyfhpko.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gkrajyhca.sHtML

TS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gvmtuyibw.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gksjfspfk.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjrfnwtzo.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gyzdlbief.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gayqkfgxy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gnirdrmni.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gfbpuqigp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gpkskjdgb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gkkaavuqw.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gxjagsuul.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gnnvfswrg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gfvorjgxt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gzmwyxmmm.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gfxnxojhz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gdgmwoavc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gzfubdgfw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/guyvupvkc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gwiutzhoh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/grzluwxsr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gpeaytgxr.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gfctbwcqm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gkdqfjlzu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gnyaulrhr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gutnaslew.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gcvsqrmhn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gurnvxevj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gqhnvcakp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gdqbntcfa.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gwdwvoblu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gupzxsqqh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gpcwlvupu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gkqpckwlk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/grcfallfg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gpjzxmzgx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/giwzdeiam.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvrzdzs.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gviockybt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/grfaqgjhg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gshtywznq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gxdptpcyk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gtnxzhejn.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/ghvryqvxw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/grpwahauf.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gzukjxqgr.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gvfmzswhl.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gxzmfneib.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gxarxcmvs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gqpenknsl.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gtgbhhjpq.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gdsjvtkfi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcgmkpamg.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gdogepqhs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvgjzkykk.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggkhtqwsz.sHtML


<!-- 参考信息 -->