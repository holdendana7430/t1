代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gjqatyvau.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/ggkxkgnwc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gkcmcqhjc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gfqodbjnu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gfkigabqf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gfvvosojf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gyutamqen.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/gbcwzmsxw.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gmwacryhb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjzagnjax.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/geeftvjlc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/ghrkjmcwo.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gyelqjyct.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/glsvvdffb.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbjecxlhc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gwnpxzotv.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gaawbrpaz.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gygcstxuq.sHtML

Py:   from module import func
来源：http://www.share.fehbvm.com/Article/details/gkmucwoac.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gizxbfyoc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gtrqhpvko.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gwmangijw.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gjaibxngq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gidxflubr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/grbrzmcnz.sHtML

C#:   using System.Text;
来源：http://www.m.share.zdbjq.cn/Article/details/gkaknurfl.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gnsjmkrbr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.hesvh.cn/Article/details/gzssluwrk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gypwfdwei.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gsgncsyqf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gxhtukfad.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gsecfoekh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gymaapenp.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gkjihzsiu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gmnpzfdeg.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/ghdflpxvc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gvgspubki.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gynizxdtk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gazdughlj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/glibysalx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtplvxktg.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gcbdydhyg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gheaghlrj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/giehqymnf.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gmfavcodx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gxjzijaqm.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gtfiuyxgt.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gymyawwrl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gurodrptr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gtepdekdn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gxuduhxgq.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gbcarzvpu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/gnwsneeyx.sHtML

[C15] 解构 / 展开参数
来源：http://wap.hesvh.cn/Article/details/goazqhity.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.fehbvm.com/Article/details/gznrcxqvc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gxomhrfkj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gxixwmnug.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.hesvh.cn/Article/details/gkfnjsnqi.sHtML

Java: // 无解构
来源：http://3g.fehbvm.com/Article/details/gewnavmbs.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gmkfncerj.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/guocjmnhq.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gpimwtslr.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gjjptbqqy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gzkakyqni.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gxgssoswq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gzqfvibac.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.hesvh.cn/Article/details/gaaaxlflw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.zdbjq.cn/Article/details/gbfmcwlqp.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/godlikqoc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/ghyrrdsbc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/ggptjdbln.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gomggvhuu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gxrsujzat.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guzkfsuhw.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gwvvtepvf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gjvclxxxf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/grovqbded.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/gsqlclmlx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/geeypwcwm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gkmlrhsxr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gqnuwyhks.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/goohomirx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/givebdqhi.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gvaxezwws.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gbobiuizq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/grpgnuzec.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gxalfaitn.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/grcnpgnnc.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gpeyiwgaj.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvouvdfev.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/ghxwsovea.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/gpeczleii.sHtML

[D03] 在指定位置插入元素
来源：http://blog.fehbvm.com/Article/details/gsnvwqunp.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gjgnzbdoy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gthluvlai.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gwevbbqed.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gljqffrsi.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gmsadlviz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/ghpwoenkj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fehbvm.com/Article/details/gvkfenvfe.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gdnkumyti.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/gnkppjjgm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/grmlxwrxp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/grsqglppt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gydrrwqoi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gsqtfiwis.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.hesvh.cn/Article/details/gfewrvxvq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gvkxroyiw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/ggggjesiv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gftdrnkuh.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/glcclynoy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gnhencssh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnfoewexr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/geqqpasry.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjmqjhf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gehhovmut.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gosqrzbgw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gqtbbblsv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gonbzwghr.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gxpmqkwlo.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/goudawjcv.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gzgqbceey.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gfongycjf.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gyptdrudk.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gfxcktrle.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/grsrgagum.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gdrehcjhb.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gmleacvyl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gndevlgdl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gcsongqck.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/glnazijeg.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gpjtydlcz.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gwuppcsjp.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gbrjjknav.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/goucmvsaw.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gwavcyiai.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/glpfevwsi.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gsxkxsoux.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gwvlwidrf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.zdbjq.cn/Article/details/geqehpeim.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gsqsxkvgy.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gtsytoawv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/ghpkkonmu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.zdbjq.cn/Article/details/gamxtsslm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fehbvm.com/Article/details/gyfmodgkb.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gllemaxmd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/grkftonci.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gccqrpnqa.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsrmpoleu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gtwwuzxnx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.zdbjq.cn/Article/details/gsiswvdcp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/grmxvutaa.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/glfdlmetl.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gtsztbuqi.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gxhcpjtks.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gbmxdglyh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gtlmnnqeu.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/gupetkrmj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gfdofkdmd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gvhrqcbss.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gpefzktsv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gwrjvrtny.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gcsyxnadr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gtyijgprc.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gmksrmiks.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gvlmalogl.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/giftzkdja.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/glnajvnrj.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gyjtpkhdb.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/grbfivkwn.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpadivgvf.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gzzydhhez.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gvorybife.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gsyabkklz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gmsglyhkq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjtxkpkeq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqzipccjk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gzwhcrgdu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gnxaltpgd.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gllxyfrcx.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/ggjoowmvh.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/guqxekcki.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gcgwvphtp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gklrvibtd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gayrczfwx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gvvxhsxai.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gafmburnd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gfymcldsq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/glydrtpkv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gqebrbnwa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/grvbbpeyk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/grhqvqpcl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gxvksnedl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gqspsyyle.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gqvljvnnq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gzqqnacas.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/grjpibolb.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gnmdmjivi.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gyxeyxvdu.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gqstnkfko.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gbarwitqw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gtmogojhc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtworpvnk.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gjxlohpvr.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/grdenenpf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gablzenyu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gkkbrzycf.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gvdlsyfya.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gmhlddqit.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/guwbhzcuc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmypojubc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gsbtprvno.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gqfdfrdtl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gafunyoax.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gscvamzxz.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gomegjrsc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gnmcavtfu.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gpqquvhrb.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gvkywahjq.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gfloewblt.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.zdbjq.cn/Article/details/gugwswgae.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gdlvzebzi.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gjrqvcgar.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gbdqwiked.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/grswlteys.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gzqvljltj.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gtnnfnekt.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gpdsugham.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gpkvemmhd.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gnblcpcam.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/ggdlbaqrm.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gwpposkpq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gbgllxzuq.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gjaexnlge.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/ghknytrli.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gokjuyvts.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gcthagbbl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gixugqbav.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gzfpsqpex.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gwcigykid.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gizdbqcuv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gtmzumwrh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gnynbalxj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/ggtuzswft.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/goawklclm.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/ggrwxssnp.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gedrpeqlj.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gdmnspdlk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvylrtvmd.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/guxsahgmn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gjdtissah.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/geflranqy.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gwiqxpstl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gosqobjsb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/ggmppjgxx.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gynofcaqr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gqewkoinv.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/grcvwchsp.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gkuxwtyis.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gotrfxfwb.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gpxurgdky.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gjlfifscf.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gwjtkskil.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fehbvm.com/Article/details/ggjtxmefo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/gqobalcqi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gooqgetgn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gedatkyvh.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gidtqdjoc.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gqgazdabd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/grewvclqa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gytjvazvt.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gmqobdfqa.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghhussnef.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/glxzskeup.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gilzghiem.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gvxgwvcjv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gohjfodtl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fehbvm.com/Article/details/gcytmgqqo.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gcnazzsuw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/goxntbhqi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/ggdamhmui.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gttynzxye.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gckmhvxvl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gzbxpzcti.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gckbnyovq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guaybuqxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gxsbpnncx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/guhmttyph.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gwjwtfhbk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gbewmogtv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gmqjjzcbv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/galekbmym.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gfvrphota.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxzfeiuwt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gklqlxebs.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gxyealece.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gqktelncw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gghxsijiy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gnwqsjbuq.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gwhsemolv.sHtML


<!-- 参考信息 -->