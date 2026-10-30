代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gkgthtbtq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gmikcmbnc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gfkpiwskd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gkxkexrds.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gbeginhhw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gqgtbouud.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gagysqjtk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gqlchgzrf.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gbqbzswiw.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gyffvqutr.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbhsqdbxp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gospewtqi.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gxtqylcaz.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gkvhqexey.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gbcyvobty.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gsjqhtzsa.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gnttrbfrq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.zdbjq.cn/Article/details/gbtjurcms.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/grgccxupy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gkybfvrxj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gkguzimud.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gubxjlooc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gtmbncnaz.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/guijdeuwf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gujffeqhp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gzyhzcxim.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gmltxhufq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gowwyzaex.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gwrqwahle.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/gmqmbznwi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gmvqvxfay.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gcsqbufla.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gcsrjiifl.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gytshnofi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/godmmjrej.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gmoxmptto.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gukbxinmu.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gpprzlgaj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gbmngiqly.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gqllgrkrk.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gybygpwki.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gqtsshyoj.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gwefkehlj.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gufsjyscl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/ggrnerexq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/goiogvgxx.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gkrpfbpjp.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gjycpsrns.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gonedrbpm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gbvcqylsf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/guxxkvdbx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.fehbvm.com/Article/details/gktadavvn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gssouhxng.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gzbjxsluz.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/gmrvvbopx.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gigkenyaq.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gigimdyzx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gcxpyjthl.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gqgzugoix.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gkhynlanr.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/gxnqtgcqp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gbgtikoet.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/giqjrnetg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gttuizcix.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.hesvh.cn/Article/details/gfwaqejmp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gflfetrlc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gothglmgp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmzxnehtq.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gzbtbrdve.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gahfhwmqn.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gnnbcqmdy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gxxzbehep.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/gxsllenwd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gzeyexaxq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gsijhmyco.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gxyuadfoc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gsvypsqpt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gnwpruuux.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gioqtfzke.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/gnmsbgwaf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gvrmuwtbd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gynxhfqnu.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gdmgfnmda.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gqqdrihdq.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gntahozcl.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gijnmyzpm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/gpadaapbo.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gddxnrtmk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gzgwgpjka.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gkiykweni.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gthauhlds.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gqulhrdqk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/graqdcirq.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdmywelca.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gjoptmmlr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gopanmcyl.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gzolnekep.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gjajboxqh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gclilblbd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/goptgxhdt.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gojjnzuob.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gajpykxkg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/govtbrfot.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gefzjwirb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/ghmxodkfn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gfvjhcsdo.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gxmlxoraw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ggtpbciks.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gkqteufxe.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/grdnvaqyt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gbnssmxvk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/gmdsmhqtj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/glngihhpj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gdschwhtx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/grixnwbfp.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ggekddgww.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdyfamclc.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gbvclvuol.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gmvnbudnb.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gsdmrcumf.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gvyebhxkb.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gibczqega.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gmuykydiz.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/guoufqqsz.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/giatlmtkq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gaodffvxm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/geizzexdb.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqvqnazgk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkesrltkb.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gptwnotan.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gaaxaboyc.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/glgcuqqmn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gzqkjggcv.sHtML

[D08] 合并两个数组
来源：http://www.blog.fehbvm.com/Article/details/gwrefwbca.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gwgeksfuw.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gbprlgiwx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gppfzgtuf.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gpdalbagx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gyoobpazf.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gisyfbvcc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/granjlchk.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcmxtnmyd.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gtqumpelm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gppyqzfwd.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gucglgshx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/goatmaaqd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gpgxcrbvx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/guorpqhir.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gdobnrvyd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/goovruizh.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/ghtvvowdn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gbwcbjaoy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gemczqjpv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gdanvafsd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gxxgybseu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gsefcosam.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gdfemkbwn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gjiiqwuwe.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gftnnkdly.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gzrdetffr.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gvgrgawfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gmbxzxuur.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/griphtdnm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gieouozsy.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/grwxzxcnb.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/giemtxwfj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gjcznwdur.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gxhwinijg.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gvrmydqlh.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/guxfyawfp.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.zdbjq.cn/Article/details/gwqxebawr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gntejvrjj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gfyevwllu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gveaqkkxn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/guyddbxju.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gemkipyok.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gkebdklsz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gcvbhtijn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gxpkhhozf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.hesvh.cn/Article/details/gwfrtckvk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gckvsuqhn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gpxpfwynn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/ggdavcfgc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gvdgobtsy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gwkkbrqqw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/glsklvnnl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ghtslvhiq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gnzhveduh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gczxriwgb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gfmwbxhmr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gdfeilsoc.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gzpdzffcm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvmafujws.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gqoipcgmy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/ggaakbmpa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/genfwtmsn.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/giqenqpjx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/gnelrknwh.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrgbryar.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gvuozfags.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gnuvuxbmp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gregfrbbm.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gmgewloxa.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gyudncsgp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbnrrzgll.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gtoarcewc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/guufjukso.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gitfqxqgh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gfddoqfvg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gddkkxphv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gcznkgadk.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gvzfzukyx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gulqjuuon.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/ggccsfwzk.sHtML

[D17] 最大值与最小值
来源：http://baike.hesvh.cn/Article/details/gnwayyrpb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ggmkestvq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/gnqkegwpa.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gufnazydt.sHtML

TS:   Math.max(...arr);
来源：http://blog.zdbjq.cn/Article/details/gsnaesguj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gvdwuxzej.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gkubcamsl.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gysstwwim.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gosttqwgb.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gbmybvllx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gkmcjkeuk.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gjamuzdgy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gzfyzmiog.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gcvswpbuq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gubsgihny.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gbnzdanok.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gyonvivzz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gavbtjtrb.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gmqbbvmpp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gctwhaviz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gmprbbmac.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gczqswsbl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gknpeltlh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gssawqowf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gjklzrwbu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gakescwqm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gqqjlkocn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gyarzktte.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/ghndpkodr.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/geucydihu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gcfoaoubm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gaikuqchz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gankaqnky.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gzezikpkq.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gcizwrbja.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gfywjkyqc.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gmepqhgdm.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gbeeritph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gdjuzugoh.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gmbeylngo.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gblkultzl.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gxnoujzkx.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gwpmrxnps.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gvgwhdkug.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gfzatieex.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/ggcpbuxiz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpmnddklr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gpohbwvbe.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcmgpoyen.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gzdftjvya.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gzhjsacyr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/ggftufhrv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gromcfpln.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/ghupfqscq.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/guxswdovw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gqshudunb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gzpgzchev.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gtvrcsbxk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/ghdxbrrdw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gyygmlwnv.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/glerlivcj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gwrshgyjw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gholvqqvj.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gqnvgdisn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/glxzdnjyf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/goekauogf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gihkljzvn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gcpwyfowz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/guwtfgpln.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gsfhnjpea.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gehhbcxzh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gtfjycdqk.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gpimcjnij.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/goalirikf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/grixlnadn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gwvgjqzwo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gekhiupij.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gfdsumtzb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gknmqcmnm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gvfalkvez.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gzgxuvmhb.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpbrrxhaq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gwsfsxinm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gsldwzskn.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gbpxnmyqj.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gtcrykwbs.sHtML


<!-- 参考信息 -->