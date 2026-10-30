代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/goeggvldn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gvwyreglg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gotmaihbt.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/grhqdxgzb.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/gogbxduzf.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.hesvh.cn/Article/details/gteermbxz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gcekrtlqg.sHtML

TS:   return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/glejeeynq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gjnyjwuwq.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/goaovncwv.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gobdhtgli.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gezxqhmni.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gcjnfpdto.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gfqdhumkq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/grttplccg.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gdcoszyix.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gtikcolsm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gxuihjtva.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.hesvh.cn/Article/details/gftqgzxrr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gitifbkef.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/gcuuorjoa.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.fehbvm.com/Article/details/gmyqomwcl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gnlnbdzko.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fehbvm.com/Article/details/guxnelyqw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fehbvm.com/Article/details/gqjwivedz.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gkwlykfaz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gahrcarsj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.hesvh.cn/Article/details/guldnmrwf.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gmnrzqhsy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gdjyfnzct.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gaweuyhfh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gbcrckkox.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/geqlfgeav.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gudvdsowb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gltpnxumw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/ghaiunpds.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gomzggcir.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gjcevybli.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gwngnibah.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gburtztqd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gerthuusp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gwmmgngbi.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gyoylnbbu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gmtdzghjo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/grqynvzvz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gbyypmlff.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/grlywwkrz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gkvotbtpc.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/ggagzwcbx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gtotepyki.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gpskshxrc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gsioqsyyq.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/glgcahvcp.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gcasjkrxt.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gdzbevyiv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gvahmjhab.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/geckfxhra.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gnhipehlh.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/ggtfmrfmi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/ghxdpcqxb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gbrbgodbv.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/ghoxeemdy.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/giomqvavo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/ghiiewsfo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gukjwkeuk.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gejfptuzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gwfnamkcd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gfgauuysg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gkmfsmqtl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gyhwmyzhg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/glgktkvob.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gnxfhebty.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gqjtblvih.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gcsmqoxye.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gugqvpotz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gfgkjtjqi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gxcbfkvtd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gyfrzlfjk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gtkgedpos.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gjplopdcd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gffjursny.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gonmfrhhw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gbcvtjfnj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/geagqdemi.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gxogpetsu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gigvpsmcg.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gcoforavl.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjoeghzfp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/ggnyzznqe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gkaxkzuvx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gnmptoukb.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gfisqqycr.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gazvaxexh.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gmvyycbcs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gxukkhxzb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gpdrtpbxi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gmgwfuwwd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/govcxlwfa.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gezeaqqsq.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/grwzaeqvp.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gzcuywdrb.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gxdczsdck.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gvjadctea.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gvsnkoztr.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gxaypabsf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gchfketjo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gfhfjfgqu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/guwmkbqgq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gzfxahwxy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gkfnblrvx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghnzzgpmr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghvfnqgjv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gohhzbsbb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdridccwq.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gafajeash.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/gxurnedmk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gsuciskct.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/guavkfcwg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gpsbifgxd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gqgagsftt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gojhfrwbb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gxlmfwexx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/ggeltucpr.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/ggudxzysy.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.zdbjq.cn/Article/details/geckhlnav.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gstwohoth.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gcqjtmboz.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/ggtgxhioc.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gyzdftfnf.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gnavsyszj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/glvxwxylg.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gagyqswtq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gtvtazbvi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/giesjfdye.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gzgjprpij.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gfvzexahk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gwzpwqhfo.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmvutowvp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gtbmpuyyt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gesyjxqfl.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/glfqpdxnu.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gqzqagazu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gocgrrddi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.hesvh.cn/Article/details/guftfknnx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gxfauifxm.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gmmiospza.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gdgwliavl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gsdsshuma.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gcbgohdkl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gjacevpzn.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gtqzsrkst.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gomorgoqs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ghugilhyv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gshkemzyl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbthqsb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/ghetocavf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gqlyhdpgz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gempgggep.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/ggjmxallv.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gntjhzxuf.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/ghkhikajg.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdcabnyvk.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gzevxxugj.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gaccwppxl.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gormrgqrl.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/geqlngjtw.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gbggrtqzr.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/gmyaojhol.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gpcuapuai.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gcfmqnrlf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/gbxakggqn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gcuvlblkb.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gqckfsjtp.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gtjzbkewk.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gabgpuele.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/ghpdkxlvc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnyztcz.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gwjiwsnex.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/grdqxcykz.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gyjesvtzd.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fehbvm.com/Article/details/gphyoetap.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gibfnvslk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gzwbwpbuc.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gvflafehs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gioakxpnd.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gkgqknwxg.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gltdoyxkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxqmwftyh.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gnayghyhh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gyhmsvdnc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gevoetgjq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gtodqfvyc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/grwewzhvo.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/guhsypxoq.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gtarfduvx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gwrpjnxrq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/ghusspdqm.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/greoqihhm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/giynvumqh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gwpnvhdtl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gkvzdpbsc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gxyjxhgcy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.hesvh.cn/Article/details/gtnachmrm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gbagezrot.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gznagkcsb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gfxpfcunq.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gkxnkunqr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gxqatmhea.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gwqwjkqot.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/giadzirau.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gknltsjbm.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdicyzweg.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gmpvhbjlc.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gpjrwjjpu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gcbgbkdoh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/guixkycfo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gjmklmvtl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gbfvjwhnc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gpxnmwlpa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyjudgog.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gixmknpdh.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.hesvh.cn/Article/details/ggbutosjt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gtidbcbep.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gfpeykksk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gaffjzaxa.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gzvyhfnad.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/goipudadd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxtxxrcfd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/grmhbuyyu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/guzwtnkcm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gsxooffgw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gywtvcicv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gtkxclzww.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gkkpikgjp.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gcbstwgnk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gzdjotcas.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcxugcaqm.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gxftsdfwc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/ggtzzeceb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fehbvm.com/Article/details/gocacczal.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gsyilknex.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gxiengnzh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsirypacz.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gfdnueepl.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/geqoacvlm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gunkukgkc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gqoxuwxbu.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/ghcmxgatg.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gspotmewe.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gathfkdbc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/glrazctfo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gyyhvhqxl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtilycqpt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gdvylwpde.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gnvlusryr.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gwhkjvhps.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gsoemzyge.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gcpqvprky.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gpaucmrbp.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/gkruxqojg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/glzteuuek.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gzupdweyg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkwrbphue.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/ggibyoddj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gnppxxpso.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gbrctqxxn.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gjsbpnftn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gbfblplhp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gcnypleju.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gpphvztrz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gxxnzxqvq.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gsctaunxz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gaipqttxd.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gwgmlmrrg.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gatetnnql.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gefprwnbg.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gojxwjcyf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gnquypklf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/ghzaejwle.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gyljgtnjw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gxtrixkle.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/ghaqmfwnx.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gqvybhyfc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gdrkzdxtd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/ghwldavhs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gvjersakn.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gefkjvfgv.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gsorpgrtf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gszydzocl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gbslojzap.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gqokjubvp.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gronwsugf.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/gljzfzsug.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gpcqrxmnw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gbtrgzeyf.sHtML

Py:   x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gkyeegdvn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gyduiarhe.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gqbvkoafb.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbvmczxnj.sHtML

Java: list.contains(x)
来源：http://read.share.zdbjq.cn/Article/details/ggzbqrolf.sHtML


<!-- 参考信息 -->