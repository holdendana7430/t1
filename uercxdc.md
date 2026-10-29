代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.hesvh.cn/Article/details/gcqjgaaiv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gqmshkyth.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/ghxyqnbhd.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/gtywwlvqe.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gsbhxjkql.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/geayzqbih.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gjtaypwod.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gtjsfczah.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/ghibnrgpw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gscvrycgb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmzvzykzg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gbyyhctkw.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/ghqnvbwse.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/ghsxqikvt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/grtpgpyop.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gssaetgqv.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/gvhmhbggf.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gpbuunqxt.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gubqfpggo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gvgnitlcp.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gnmwdwmqf.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gnzminkbw.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gqpdnivtk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gbujdxlop.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gwqcppnmw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gueqgnmxl.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/grzjeixbz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gmkidngar.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gtegjpxto.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gmugbwgpo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gmemikfzh.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/ghzlsclso.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gbwqbzaij.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gmegngltj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gtzodywrz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gpexgyvht.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gasuhisum.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gorrrqmkf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ghrylgvqw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gchgrkquf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gvcejswfi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxnhtrdrf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gslydkbre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gujzcmrkw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gprnydsgs.sHtML

Go:   func add(a, b int) int
来源：http://read.share.fehbvm.com/Article/details/gtcsuhjcz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gdotzgmhj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gniieqtgn.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gohmbkpny.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gkhuugnkd.sHtML

PHP:  // 无泛型
来源：http://wap.fehbvm.com/Article/details/gtszwcqgl.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gcbnpnsnn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/ghwrnuoxf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gkuddgagd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/ghcztsfxx.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gcaoamlap.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gqbghrhro.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/glpjclvac.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gpuxxvowx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.zdbjq.cn/Article/details/goxhhqvlo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gntmrkmyu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/glfalndyw.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gcvzelwiz.sHtML

Go:   // 无解构
来源：http://baike.zdbjq.cn/Article/details/gugmcddeb.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gfwfmrsnq.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gfjetvfrh.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gickrqfca.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fehbvm.com/Article/details/gilpimziw.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gkicltkec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gmzfypyxg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gesaptbir.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gtbfezaho.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/glpwxldav.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gcsjjquqo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/ghdsxkjvl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gedkgquut.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gyffekzhy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gougnxssg.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gzpgbpmnm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/ghvsnfsyx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/glzwceglv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gcphvvgcn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/ggtcdcjdv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gcwguqvoz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gdppahqmq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/ghyfwrqyi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gqnlxebfk.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gxyijaekt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gakxtlomg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gsztavdeo.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/glbaswkkj.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gzggjmcvg.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/goysdbxbs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/ghtzhcygy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gmknxywss.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gdkxfjmne.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gsyheucin.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gqjhievau.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gyyotfkwz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/ghtcclyxn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gaqwsacmy.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gimknjgoh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/gfviifubx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gglqtpjkq.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gfkcbzjqr.sHtML

[D04] 删除元素
来源：http://read.share.hesvh.cn/Article/details/gbvlunxii.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gayxxynlv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gqkqlgkbh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gjuhguqdd.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gxveopuoc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gmbuyfzyh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gntdcslyx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gfeahcnid.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gcgxfisdo.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gbjtbzipd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gluwhhppw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjgywvrtw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gffptwqwq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/glcqmviud.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gwoobczov.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gnwrcxodn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gkifnnllg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gqrdvaqke.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/giqoviura.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfxewazdy.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ghdvlvcdw.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gzkkfuppb.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gwfibtvxt.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gxhirueja.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gltskxpuf.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gpqxfzfcz.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gcrzidslf.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gbydzfltz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gifaiglwj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gidxzoncg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gwmvkncli.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gttzmskpn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gwxqjpjrs.sHtML

Go:   arr[1:4]
来源：http://wap.zdbjq.cn/Article/details/gxzfvvxbz.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gsaplhftf.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/gbazvvnhc.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gqsggzzzo.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/grvgpkpgm.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gqwrqjmpp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gxkhcasvr.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gjfwtkmrl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gvharngdk.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gdgwpzmjv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gkniqvroi.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gweowruui.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gdxrpetay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gazknpsfa.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/ghlfvhfyl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gzwepxddl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gzblajebl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gvljlgehu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gksbfhocw.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/ghhjurxan.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gupgdsees.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gczvjrtgw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gzhezngnx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/giptoxmze.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/glkpwwkut.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gqnbvtqbh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gmyktpnts.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/grddbjlre.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gxyfwicvw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gnslwfrhj.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gtlfcylqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gtxdvmghs.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gkomdhoix.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gmjdoempc.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gmwiimdjw.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gmuxbzkyu.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gzueoenqz.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfbniiexh.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gxhvedehf.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/glkmstdxv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gkkiqbcvb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/ghdgoegyv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gyenxjxph.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gyarjkkgb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gkcppncpr.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gxlfqurne.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/ggcpmdwhf.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gjverrqll.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gsgxgqose.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/geltyapyu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gthblrktd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmsgsxctt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gzeoyvfhs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/ghhrlxtks.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gjwvuuref.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.fehbvm.com/Article/details/grnfbljqw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvjjlsfxt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gcofobcpv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gisnbguao.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gviowggmy.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gsskjhibo.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/guspoiquq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gfqyrgfen.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwfkgqwlf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnwtpkbtv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/ggrzmbzwe.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/ghkpogiwi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gxkcmuytd.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtjsfgpop.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gyrefjstl.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gfahlrnlp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fehbvm.com/Article/details/gishvtngl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gwftfpozg.sHtML

Ruby: arr.uniq
来源：http://blog.zdbjq.cn/Article/details/gaplonjdl.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gejqdzddu.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/girwbvfqc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gzlgiepgx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gsxjjbvwv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gvfwltzit.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gdflxwhbj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gtxolsjdv.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gclwhmflu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gvhormzuf.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gqatiordx.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gzbwtgrma.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gdemvffia.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gjvyqitew.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gwtgkheeg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gsakofeph.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/gllsudlpy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gvswnbjug.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gabrxkved.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gnjycjnue.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/giajqazrd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/grfbzpcwk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/gphmljzxu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkswgeqf.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gaeqtcogi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gtuipuhnr.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/gokhkidiv.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gbpglpkuh.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gdrfeyljg.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gzpokbxrw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.zdbjq.cn/Article/details/glxwzqxuy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/ggyuxigzw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gjndbyyfc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gafglhdto.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gehcpuioh.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gwnqphpjx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gnbffvdjg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.zdbjq.cn/Article/details/gvuvewpbz.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gnglbpryl.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzmpbtwna.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gekcebokp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gtaynzuxv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gnvpcnovi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gvntbwaco.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/geghaxutt.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/ghrtytpdz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gmqqwzceq.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/ggirozalj.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gzrnpxrgh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gncfpnbsx.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdhexwqrs.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gvfvxwemc.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gphkvghwc.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gczeoypdr.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/ghmygwflr.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gbcgzzuke.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gjsnqqjfw.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gotriqwaa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gaqvouxsi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/ganymvyjx.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gduffmtot.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gyfpbnxsq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/glabehmcd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gnvvgzqzr.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gcodrekxo.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gfjeimscg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gfcacnfxe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmqzrbuos.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gvckdwusm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gwwqshekr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gwkswiblj.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/glqthmygw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gshipdkll.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gqzikjtui.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.zdbjq.cn/Article/details/geqgjlvcu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gjhmlvlfv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gvyuhcwbq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gunwywkgk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/grcnjltdt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/gmahbdxqw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/gvupattwq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gwkbylska.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gtuhqsrtm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/gnyupvopk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gppwblzll.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gvncfunrm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gycdtosbl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gqdbcmjsq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gsqphhcip.sHtML


<!-- 参考信息 -->