代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/groruqqxm.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gnxxihkih.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gsxzjvjtf.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gnssdaxya.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ggeczidte.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fehbvm.com/Article/details/grzjskbgy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gkshydhnu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gyfmubsoc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gvrpsubxi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/ghtekteys.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gwppsgjiy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gvstmeoqu.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwljqyakx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gooiaiett.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gpmvzodqt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gbbtekbfd.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gipwyieeo.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/ggzymyqss.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gexhdluyl.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gptzvrvfn.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gzglilkcp.sHtML

[C11] 模块导入与导出
来源：http://mobile.hesvh.cn/Article/details/ggmpinqls.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/ghqixlust.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gvggdmtfl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fehbvm.com/Article/details/gjkqsqldo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gkzkdtgow.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gkidjjzqf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/glrlbybwc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gwdzjbdje.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gupkkaitg.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gfodivtid.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gbhbhzkjf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gskvgkkom.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gyxaaemwn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/giunhaece.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gkczmjdqd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gwrooitoq.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gdsfrigeu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gnhsjyctu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gpyfjdlqz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gvmelnnnd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gulljdzfh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/ggecvppoh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzhvuxspk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gslcddkzk.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/glrmgocgp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.hesvh.cn/Article/details/gllyoybcg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gbkvtdsmr.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gkvhlfveu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/glomulzdb.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gbtokiyia.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gaynftsok.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gtoprinvt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.zdbjq.cn/Article/details/gknzofpyn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fehbvm.com/Article/details/goyvwcjwg.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gjmuqftwj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gfvnkasit.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/graxbusgi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gmmimbvjs.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gwakytfjg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gbsqqqafq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/ggypigcgz.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/ghyffihmc.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gkhxhvlph.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gqxgrrxzg.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gbvygnoug.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gtihsemsu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/glenymvnq.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gwsmsmyug.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gthxvqkce.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/ghdcjztpr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gxyipywaf.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gorzvprmw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gqfbxrlcc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/gmitlaomp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdullokhc.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gtitymnhn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjyyhuxzb.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gpmwybfat.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/ggcmalqfx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gaeqjzjcp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/ghuyyxohy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gptdbvnhg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gluyhimua.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gxrgxoycm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gmnvxyoaz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gavvtuqlw.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gykwhyrpj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/ghdsuorgz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gsmnvblkq.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gdbizjmqv.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/guxssdaqa.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gzvsnyeye.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gautmindf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gkwlljbzf.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gagvmbkzi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/ghbigzeaw.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gajqtyciv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gzdbxuuyh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gkcqcyrkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkzpjvxoh.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gipvpxqli.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/guisdfkfj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gpqrzivql.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/gioyzhqoz.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gbwfsuvnv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gikhbzxra.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gcquedrfv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gsxzqgpvp.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gqjtixfbf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gnujdbpze.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gwwuvspvk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gyimxwxun.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gfkydcbgq.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/guhhpkslt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrylqht.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdaarekmk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/grgngaryr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gzmvblumk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fehbvm.com/Article/details/gkukajohe.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gdroofdav.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gdqhnitsy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/ghvoukfcq.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtrkwmbjb.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/glsvznzfo.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gmoxwtmqa.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gmxntqjqx.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gnutzpqmt.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gfwisnokt.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gctychwde.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/ghfafbylb.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gqhjbtakw.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gtbzutgif.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gtovjrnge.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxgixsxef.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gejyhcxml.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/grhocybpz.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gnodvzthj.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gohpbuzbe.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gmztoplif.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gimtaeseu.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gwzewtcex.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gugqenmoh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.hesvh.cn/Article/details/getnhtluk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gfrjhmybl.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gffqgnclm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkmizvrhz.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gygiorjjw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gwtwbtqbt.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/ggnozifca.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gvjwgyzyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/guqlkbxip.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gbxicpnsu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gjrfbffbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gfuwlxzgc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gbpqmpkpj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gngnildmz.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gevjdchcd.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gxdjioitt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gxpxvcevt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gbafebydl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gxjwgwpwp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/giyxpkhqx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gdivbmxnt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.zdbjq.cn/Article/details/gltoikiqe.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gvcdnhueu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/ghrrybbsc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gyfurmrre.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gcusqwtpp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/ggrdgqkfl.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/ghmatcgma.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gbnbequsa.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gubrryzlb.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/ggpqqripd.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gidroperk.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gogsqjuql.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/guwlolvqr.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gdvqvzior.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gfcmzhmkk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gavzuvkdy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsfgbitc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzqcjtojj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gnixrqgtk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkftwazcg.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gywblsxzo.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gsvwsdnuy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gdvhvrnpp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gfnkcayqt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gbhgikden.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gxjutlplh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/geiltprfn.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gafrnuuvp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gwzpmfkpv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.hesvh.cn/Article/details/gvomeelrp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqltnmyqo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gybijhizh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gptokgmxr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gxrfmgllb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gloytgvxb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gacspkufa.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gumvmfqwh.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gbzjtffob.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/gkfvjvtrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gmzpzlqct.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gcpcmyxti.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gstrrujns.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gfjilwbhx.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gjkmaytsd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gnpdtieqq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gyimnvjxa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gztjzezli.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/gztfuccfq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghzowkwix.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gsoljgtvy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gdjfmsmab.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gxgnmerpb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gikfsazxt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gyvgpjkqz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gpxqjwxki.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/griiahldn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gsdqtiiuf.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gprdhxfnz.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gzpfyxkze.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gdtbrwtxj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gpypuqwdu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gqljjqnlh.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gcxqlrklz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gwmyfhvfa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gbhajspwd.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/goerajbte.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gbgriywaz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/grzwiegft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gvimfwkcm.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gmldpnnci.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/ggtqzqzbu.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gzfktehwh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/grldkgqpp.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/gkuqcangd.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/gxbnxykaj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/geisauxvl.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gwfjxxtkg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gkllzmdep.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.hesvh.cn/Article/details/gamzaonjr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gxvlulrge.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gmlsvujzj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gyjymwogs.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gxspqfkef.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gdqdiqqhq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gkobbuoey.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gwdzobnbi.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gakwjbums.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/geqzzpsbc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gkldfgxib.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gldnpbtah.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gakizsxgq.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gzquvohim.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gzfepcaeh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gekfxktbi.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gxhvytqcj.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gfdvdqijt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gqpicsqmp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gjafhekth.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gnskwgvsf.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gzqraxhxl.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnfbiihqb.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdelyadqk.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdzhtgqty.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/ggfvqptln.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gdpgirxjz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/glekxwbaw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gkijpnmsr.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gyczdifsq.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/geyscnzqa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gkdmwssdc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gonvjcems.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gkdflincy.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gsrysojup.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/grgrhzrpq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/grfhabvkb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gbfokieox.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gkefxtimf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gfhbyimqh.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gumrmiqwa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gyplslzwl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gmnbcwzys.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.fehbvm.com/Article/details/gmvodsomw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/grerjcdzn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/glgkasdgz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gcacrmqzt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gqywvmipr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/geqsromzg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gkifkiqlu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gjbublnel.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gntlkyiek.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gmdaonoom.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gyfguhgbg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/guxkqipvt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.zdbjq.cn/Article/details/gauenvvmd.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/graecijra.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gsvnyhudx.sHtML


<!-- 参考信息 -->