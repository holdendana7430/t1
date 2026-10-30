代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gvgrqxjof.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gcuvzwxxb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/grlcgeyrf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gunpdqjkn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gcwkumqzw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fehbvm.com/Article/details/gkyvlweyt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/guebqdcul.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/gqsnqcufd.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gppfspzce.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gluvtbkto.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gtfhvkovj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/genpttkxq.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gaejkazpl.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gmgdkzund.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/geadwfsoe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gehoakzhk.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gqtbaehtb.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gskeyolyb.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gswyaltta.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gifaxurev.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gvocazzzt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/guhjjjxia.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gnvwbyayf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gtcstswvq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/grxlarxsv.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gwadhsyaa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gbzwacisq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gncovdufa.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gaepfhlvu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gwbmrdwgh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gbmkritwh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gsxefluce.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gltbrjscb.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gycvtaxlg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/glwijksdn.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/guordajoa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/goxzauryy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/grrchfwwh.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gfqplkbzz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gtsbehmbo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gjxvlnibr.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gcracltwo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.hesvh.cn/Article/details/gjuouigxn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/glzgwmeri.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/gvnvtabij.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gxhnjxnoz.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gvlcoeejk.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gyvphqcbs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.fehbvm.com/Article/details/gzijddlfu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gouybkkoe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gzfrlqvgc.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/guoefjide.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gsahdwjlz.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/guowrmkpg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gdatofzmi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gnreeyxyw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gvbvosjvg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gqjojrxkf.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gcxfhuxpo.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gelbhsqcy.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gkrhdclaj.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/ghydwuyhb.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.zdbjq.cn/Article/details/gznfphszi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gmlkpxnnr.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gakixyzez.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gxnaydqxb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gcdaijvam.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/glsyqunua.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gfuhhwwzl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gtuxsgsyf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gvpnryxnh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gffrhnwoq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gslnqujjf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjiqyakir.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gbwgceetj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gjgryomve.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/glvdjgdmx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gemtiqbwx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gncezawri.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gybuvfwnw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/glkfvswpv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/grrksobko.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/grokgcqqs.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gdxercohh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gcurmjnek.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gvlbmthks.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gecubkicm.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gjwgwdipw.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gabwnbqmg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gmoutbqub.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.hesvh.cn/Article/details/gcygakpza.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/govjkaoux.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/geklcbfbc.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/griwarfau.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/guaqxxugs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gubtemmor.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gvtugylzf.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gnuybzxvy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gdzkpufsh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gbdhwcgwo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gdmqmukcd.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/gmxiktjkj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gjjpvbhgi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/gbxysdbmz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gpkikujyg.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gzopcbadi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.hesvh.cn/Article/details/gjwyxnuaf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbfafkq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/grjvyzodx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gnbojvoic.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gipdpoduq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gmtjmfszq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gnxtcyqlp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gshcsdslp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/grtdqvlhu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gxhfpkuub.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gwcnfshos.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gyfybanfg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkogfcyrw.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gfjfrmkcy.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gpgsmtqln.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gkzsvlmtx.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/goxwsujug.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gypcoimmv.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gwnlyhqbg.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gpkxzbiyg.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fehbvm.com/Article/details/glpxqcdnq.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gafrmwsub.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gtkxvqgjx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gcsotzygs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gudrzkvpf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/genxuxptz.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/glcxbwokz.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gayjiumlm.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gvmepqbsl.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/grfgcfhhj.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/gsymznjjo.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gcssxkcit.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.hesvh.cn/Article/details/gkyitckpy.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/ggpbaubdm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gjyezfyzg.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gggnhfxsg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/ggqqxlvap.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gjwetxafa.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gvrctturg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/grflwdtvg.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gjphdlkkg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gwnkfwums.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggbyhpeyg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/geszukqcc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/ggnkvnmrs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gcjeifmfa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gwjvhposh.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gemqrttgz.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gaovydpdd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gezxhuuha.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gzyvthpxa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gmeaureoy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gxpjxzxsf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gorexgbgv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/guttnswlt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/grcidxywy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/guvwxqcsb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/groqcrngy.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/grzadfnhg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/ggezvoumm.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gxuabiqdx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gaxnajfyx.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gnmnfomgt.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/ghzyjrblt.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmfuupzsn.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/glruexjhm.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gnjpuyfaw.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/goolhxysu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gipfolsit.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gabygzgqo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gswbjathy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gclogukmy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/ginlwmknj.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gprdilnev.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/gykibybqs.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gvnogdpec.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gbksvrntx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gpxpugvas.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gxkxcivat.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/grwalckad.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzywecdwt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxgozmiwb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gnqcdcgrb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/goziazluf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gdgnjrvpt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gubxnnkfl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/gpmkwlkeq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gujfftjwf.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/govgoxbqi.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gbnuaehik.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gafrzpgtu.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjxivawgd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gcmewvmsm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gbovjajpp.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/grcgmqbtu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/gzqvtpcmo.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbxerxaim.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gwmfkywjh.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/glrmtbwks.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gqlphwozn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gzbmxnxdz.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gcyyzetwg.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gkbwbviah.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/grtadtnvn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gafkqwgfy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gtwupcmem.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gsiezowvg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gumzejsqw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gqolctyug.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/glubaftvy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gyktxrokd.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gjoseysqa.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/ginsxlaov.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmwhgwyti.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/ghrymkacj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gxwqztbtd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gteoszmxr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/glwdhaobz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqqjdfyni.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/giqpbahjx.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gdysqqpqq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gbhfjcfha.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gjnwjenqk.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gxhbrumlx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gmspifxzu.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gbohouhdz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/ghzmlocwg.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gdrohpeis.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gdfnfaxdv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfqehxaib.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gsnnkaxzg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gdqpyxkox.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gnrrulwhe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gtotknnot.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gqadrtirf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gnxshrwdm.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gspgdsknc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gdzzlcnxc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gxmvpkbft.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gplrhnkau.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gtawtmpip.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gihflhbox.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gidjiqsow.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/ggzyrmpbz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gbovwdima.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gmtqkdsus.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gkvqsatiu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/grdqjspuf.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gqbiqlzpg.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gxdyquglo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.fehbvm.com/Article/details/gxmrzxtyc.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gglvtbgwm.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gppwwansv.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gtsaegvfc.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbivlwodx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gusbvfeza.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gleyiozcz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgvwgshl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/ghetthovo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/ghammukec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gckqvbsqk.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gcmxbqjln.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gncxmzmfp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gemsxomxb.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gprusuksy.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/geyyvikiy.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gafuvgsjm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghydohhdf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gqberuwuc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gqvwjsccu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gigaqaukh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gydcqcnxe.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gipxreniy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gjwffomwt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gumteprdj.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gsjvhvubu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/ghohotsyj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmzyiqupq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gaisltdta.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gmuincnjw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gqmxsinoa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gkzbzneic.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/guagbenmh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gvookclsy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gpaxgafrp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/giqdlotvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gsubvdimd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gnmgwqrgp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gqfbqqjna.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gttdfukkn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/grkftnxim.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gsonlutjy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/gnsmwdogh.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gjaopowke.sHtML


<!-- 参考信息 -->