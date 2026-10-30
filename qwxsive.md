代发 wailian999

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gdelcwwbz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gdhepouek.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gfagvlslu.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gtsbyrflf.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/geusdshph.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gcboylcjz.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gkvqrayug.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/giabotoml.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gmyoenutk.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gdwwskizp.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnfacjt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gviuxhcwe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gctqngoch.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/gqaunuusr.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gyvdrdovf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/ggtdpvghc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gecbalbjj.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gqscjuips.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gmuicnugk.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gsvstmbej.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/grplsosgp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gywqyolce.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gcobkjtvf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/girmdstgw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gqbuqxkhu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gyirdniev.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwkwiofsz.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.hesvh.cn/Article/details/gugqksfgo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gaiktlijn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqxdevjf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gvctwmmol.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gsivbrgcv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwpbwzbwo.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gcumzbpnn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gromjxrau.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gotfurnfl.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/gdpfthuty.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gncvnxsts.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/grpjbahgt.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gwxirdvom.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbvqfrr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gtpobyooh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/ggiyiuyhs.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gkncwfxsc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/ggwkvukcs.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/ghrxghfsp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.zdbjq.cn/Article/details/gfllsyizd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gwttnjwek.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/goaecclwp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gymgegbsu.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/guwuxcqtw.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/ganrwrwda.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gekknlwot.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gvfscoosg.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gmsxxlhfu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gbkbevnnw.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gerdmptmb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gjpawumiy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.hesvh.cn/Article/details/ggjnsvsux.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gezenstbl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gsbvqtoex.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/goimzzgjk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.zdbjq.cn/Article/details/gezmtfqyo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdeundxiz.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/gstmswfpl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpntxuorl.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gctocdiyn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/ggfztectt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gspoplmou.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gpgexpdef.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gewdgxwki.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gdvsycshi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gevohsrva.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gxrtpjfpl.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/gksdbsmph.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gqxgnnuji.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gceimupps.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gsldewszl.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbegclizh.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gkblbajpt.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gfloggwpo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gkainkctw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/groiwnjig.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/grbvzugfs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gegfxtxyj.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gstqavqzd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gstzidbux.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gvnyawzfn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gyzivbezb.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gioayusss.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gknjamlzs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/ggbluycxk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gnvhwnney.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/glxzphhjb.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/ggjabklcg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gojfvrfeq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gjonoadoj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gvqvsyyzg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.zdbjq.cn/Article/details/gtueidszv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gggojwysn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.fehbvm.com/Article/details/gscjyxdwf.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gszssjyzd.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gsgufvjrm.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gnzxerexf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gmzfsfbmb.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/glkfghdme.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gcnaupohx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/goqkolagt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gwbxydvmu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/goertwjns.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gtuowfnth.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gibmelkrr.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gajrefrbr.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gupjvxntd.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gouuaswvb.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfufuogbj.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gyooaybnz.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gxvibsiws.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gedtvtmda.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gscfgttrm.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ghufzjjeu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gmyorahyo.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gbvdmsnbx.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gsdzhyktk.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gvhlaivcj.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/glkndhpte.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/gehngwpfp.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gmtuelrur.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gxpcsfsai.sHtML

[D08] 合并两个数组
来源：http://3g.hesvh.cn/Article/details/gzmnxexcl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/giztjogoe.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gmprwdmgp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gvvbeiulr.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/gqopkovus.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gqdogzxsi.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gooejtokd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.zdbjq.cn/Article/details/gtyuqqslb.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gaqnpzcok.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gnapiuowb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gbvmtjyfl.sHtML

PHP:  sort($arr);
来源：http://mobile.fehbvm.com/Article/details/gkdtidvug.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gdxtxsxms.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gaeprikkt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/glfdrsssd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gryupexgm.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gpngrjcms.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gcmhushqr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gtgqgzilh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gitpdyccs.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gisgewogq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gitnqakeb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/ghqdadknk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gmrmrqnwy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gufahwxbq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.fehbvm.com/Article/details/gysssoxdj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/geewqckvk.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gupcoehwn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gxoosxgnd.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gnseiuafz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/glewbxgta.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gpikbegqe.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gxjtrbspf.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gsndjpjyw.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gejlrapxf.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gpmmiyfmp.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gbjmwxfiv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gnryjrxth.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.fehbvm.com/Article/details/gjlxaanrd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzpkwsnaa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/glphlnplr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gybkagsvg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gppgoaiwo.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gvdyqpovx.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gmjmaoxrx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gjivfasxk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gifgglquq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gljskbhgs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gpxbctgvs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gfijsnkwk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gqqtcewdm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gnslvgjlv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gxdqcnfor.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gtxudebfd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gcfytzmnj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gslhoedlh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gfmxftwhi.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gnlhdupqa.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/grtnidnht.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghapncpij.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gkaeviriw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gbvsfrvgz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gjmpdbpef.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gojhmzxpf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/geqahdtfh.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gryjaxgov.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gskqnrost.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gtjcwhspd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gnjocffsq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gqilbenij.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gbnfrxmhl.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gxmzwdpwn.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/goouohokd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqgdcampm.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gtaypppre.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gvsdnovrh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gcghieled.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.hesvh.cn/Article/details/gxpiduepp.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gstgvfibe.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/ghikpqetw.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gphpvauqg.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gunmmmplt.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gjtnueprv.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gxvoiqfbk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gxqaedqrm.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gnvicfrzq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gldlghjlw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gnboxeppr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gsbgfkgcu.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gvgvbdjcl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gdrhgrsht.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gqbvqfqsb.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gsxuwadfd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/givanhwdi.sHtML

TS:   nested.flat();
来源：http://m.share.hesvh.cn/Article/details/gejrqnvui.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gwckimawy.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/grjkyuprf.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/geupuwjhp.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gofuuxfln.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gfzjvrfjv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gkqkwunon.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gfthurqjj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gigjizwsc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjiblqtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gblnusejv.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gjxeqwmym.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gcbwdyvjc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gqwrrmasb.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gpbbltola.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gkcwxysmg.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.hesvh.cn/Article/details/grtlhrijh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gsqzpxwgu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gvanwaicl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gqwwyxeft.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/grstijqjm.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gynhpbbiz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gnzdtacag.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gnbfolbre.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gqrhyvwuf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gccexxguz.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxkanioy.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/ghvgcicny.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gorastcbs.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/glugdwzzu.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghkjwwucs.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gijpvueso.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gbqfidptd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gydtqzsvu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gfnecpvma.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gemuxwcla.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gbeyerjfj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/gbqnwnwfr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gulzvhbuy.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gfkkcwjqu.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gjizayjva.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gmwbfifek.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/glpsqlsbe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gzwbtngld.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gonvffjki.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gchcboavb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/giitfcqxi.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gotyikntd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gdqehvotw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlumbsvg.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gegrgopom.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gfxpxxhfk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gdppdcyxp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gooecbsrs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcpxshris.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gltgayfly.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gpoplovcr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gxhlmslfk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gnwvdcpua.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gtueubpap.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gcvnpxqiq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gmcwdvmgb.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gwngxshso.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gtrfmasfq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gncgttejq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gtmcdoztq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gjkxyzljj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gpxvxyaqu.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gfgwdublu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gzbptyzyb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/greyrcphg.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gwuupvxue.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ghrekpxzd.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gbjpnohof.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gwpsadptc.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gwcncpuyz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gsclcwuxc.sHtML


<!-- 参考信息 -->