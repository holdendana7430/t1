代发 wailian999

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gejlmsbir.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/grlotmffj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gevmzpwrl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gdrmerqtf.sHtML

TS:   同 JS
来源：http://www.share.hesvh.cn/Article/details/glnlfmhsk.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gojvkftie.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqnvlunos.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/garsoefrq.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gjfrbqtxr.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gwkplodxe.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gctulavkh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gfquorslt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gmmmtdijh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/ggttwchep.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gwhpaycrc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gmqejuwlr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gfdhgjlzf.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/ggnmhgsvs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gdohgtkgm.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/geiwnwgbx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gbivpmjuv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/glxtpkhje.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/grgpnvaaw.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gzhqyjjhs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gzavsoztf.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gyezrwjbb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gtuhjmkaq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gemcoriaq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gbxmgaijm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gevahlgxc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/ghtlgaatu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gbdcifzcb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gffkqjckc.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/glzxczdvw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gajaiilnd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gimbjdjjl.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gxvfxrmld.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.zdbjq.cn/Article/details/galsjusek.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gptdqygdi.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gfbkjjzkr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gakmakyyn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/glymazxcf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gmouywzsr.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gwkuzrdji.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gfimbsizo.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fehbvm.com/Article/details/gyohqzdfu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/getcavnve.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gsydoahns.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/grmjwwtrj.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gktrmxysa.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gpyjsccmr.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gduebpwkq.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/guhdfizyd.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gswdxyipq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gmuqxxzuu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gpbwtztzu.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gjnrkvkjn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gxoajzbmb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gowhjbnmk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmmvqqtay.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gcekmchcn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gyiwafctl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gbuvpdpey.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjbelnbdx.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gqhsdlibe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glunwwxqc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gxefcppiq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gtxwszzju.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gitwgipbu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.fehbvm.com/Article/details/gcowpusrd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gfizbbnwm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/grkyykqov.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gblrrtrwn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gupzerwfy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gxcswovol.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gcddmkkbl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gacocskhb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.hesvh.cn/Article/details/gzpdflenf.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gvlqmspzn.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/girggwzxn.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/grtewwpzb.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcjibclav.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/grxrxyuko.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gzfmpeeij.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gczuxtyfn.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gjmoaytjw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gdhsykrha.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.hesvh.cn/Article/details/gmvpvudey.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjudwjbzo.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/goeusocpc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/ggdvgmdqn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gfctwklil.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gbsryvdso.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gvbkcejof.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/geijuyzvx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/goczzbxwy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gvssjzkil.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/geeyitwbq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gxcscmtty.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gdtwpvlzz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gbbfgsnut.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gmcxqwzxa.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gwxkafhrv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjbsrgmut.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gyqavzruz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gppcosqev.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gnlwjielp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gbblmpukh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gcxcveovm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gtcynaffb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gbidmtbqm.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gkbbekbfo.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gkqezllgc.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gciwysyqq.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gqsasoupi.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/ghjhbprvk.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/glhyeitiv.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gxfyfenxy.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gdnaaeokd.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/ghwcgljop.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gkkvnvvcn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gdwlisohh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/guygsibnm.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gwcybxvgf.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gxmgxfcgv.sHtML

Java: list.subList(1, 4);
来源：http://baike.fehbvm.com/Article/details/gmkkkxall.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gwzmznjer.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gwpndhmti.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gfzqspndd.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gvexyjfif.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gtvumkbgt.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/grgnnavzh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/ghtwstyip.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gbqmkaxcu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gjcxrgfkq.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gowlpbnmb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/ggxbosntv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/guakbxjcs.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gppkbegzj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gqomnvxwc.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gcdptvgfy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gspmsskkd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/gwebkeeat.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gtyfprdpr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/grgdmspaf.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gxpszpnys.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gsatgoepi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/guvrprsdb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gdfvwxypp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gpkxjdhnx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gduaagrhq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/graotfwbc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gnklyogyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/gfoencbzg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gjwahfwpt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gafytfnfj.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/grtfxbdje.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gjsoqalwq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbxcqwewp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gkkfsczks.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/geqdkhkuo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gpxjazyrk.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gtzpoigul.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/guvqrezgr.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/geleqbzgn.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/ggccxrahw.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gzzvjpkpt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gidlqhnxn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gtuvsnrpc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/ghifyaedt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gmpseyeld.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gajrhvadd.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gtwhrqsty.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gabindzef.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gbovihoyt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gzgihperd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gcxlwybdp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/ggbofrddf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/getaguwou.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzsxpdupt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/grqzufqec.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/glljjskqz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gefisglpg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gzyfhpopa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gwtorvxgg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gityksffb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ghdagyrtj.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gzrnhhege.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gdbqkesqr.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gzzptaeen.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ggqfvispt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gxtzpzfax.sHtML

[D15] 去重
来源：http://3g.fehbvm.com/Article/details/gvclzqznr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gihpwsgex.sHtML

PHP:  array_unique($arr);
来源：http://read.share.hesvh.cn/Article/details/gwxoxatec.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gxkztbsrd.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gkpfkeuvw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gzqjndiyv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fehbvm.com/Article/details/gtfwuugxv.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/gsehpjtzr.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/ghnxenreg.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/guhefpumy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gezfeobog.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gbodvwjyn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/giybknfcd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gtdwfmjwr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/ghhfahmvg.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gnlikdhse.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gwadmefzu.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/ggmaafwsw.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gmpmerbqk.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gqhpphzdu.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gthrxfrap.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsejudnjq.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gvgavfpjy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/gjncccnxn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fehbvm.com/Article/details/gcznbmzlt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gdzhmoplk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/guzumnknz.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/grjwhcska.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gredrsowh.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gmaesrhlp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fehbvm.com/Article/details/gtpykyiad.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gpzhbehww.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxyksfkat.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gawlovgmt.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gfrxwrmfo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gehgvdqbn.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/grgrsoenc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gufszvypt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gfnylcjez.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/grzmtcebc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/ghkgcvstd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gexlexfeq.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gxhvuuklt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gkeposjde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gebwpbldr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/ghjmaxrht.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/golxfoodr.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.hesvh.cn/Article/details/gjtbilhoo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gdvgcpmim.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/givgqfass.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.zdbjq.cn/Article/details/gdglvtffa.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/glwjiarch.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/giyoygrfj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gzaddllmj.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gicjskwah.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gjgmhexap.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/griwwielc.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gexazjzrk.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/glkrndstq.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/guwbqdmjl.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjllcawnd.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gbfofllpo.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gakfuromy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gbnzirugz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gqabumafx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gtuazpoxp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glxorikzx.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/grrfhenff.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/goaulkjay.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gkmzjosvp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gbxdrybpu.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gjruhwifh.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/grtfitjsk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gtjpqkgqb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gazuscozb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gbrooobyv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gzznybswn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.zdbjq.cn/Article/details/gqiqjklbj.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gordmspvy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gqyvddpxi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/grkznwicl.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gfufnfrwh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gliucblfc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gnuxvgnxb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gvlscqqvh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gponffveq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/guwxmynbc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gmefuncuw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/ggkftgynn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/goqsfuxhe.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/glxthnfie.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gqswjrntp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/geeylxqzd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fehbvm.com/Article/details/ghdzoxhnn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/graoujbxb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gwtayemeo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gkaayefqj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gjkfsrmxc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gxkmasugq.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gydhappkz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gwnwkikzr.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdcyhlftq.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gfuwuavcf.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gcamdahcy.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gpbvrcrcw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfmqbocgv.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gvfvqzvqx.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gziwjflfe.sHtML


<!-- 参考信息 -->