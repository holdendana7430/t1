代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2skdppjwx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vetvprua.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2opplnroz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kkpescjz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xitcpsvr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2aqluwumx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2krahcrzl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2inpdjjov.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2korfrrjz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2pxakmtpk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2lpyovkmc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gjrbdimo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2usapitwe.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qiurtnjb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jofglzqx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2odxcmimx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pjlizjzy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2svhuzibn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2okvckbei.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2uidokika.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sddcrbgz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2tcombbem.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uqigeguc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2figmkzic.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ilykljpf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cbrilail.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gulmgsvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iomjlogb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgbprult.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2miicqqqt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sjmtmaci.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iqngiaqe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2okcfjvgl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rlviewrr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xjuzwvst.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uyokommt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aanxmpxv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pwtoomyk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nikkujkf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pgkffpdv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hcvvmhbd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jrsenled.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sklsrvfx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ldnpbhho.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2snjaviwl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hengsluu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2svpcyzml.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gafivvxz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fguthnbi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lvmmexwh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2otipyzkg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bgtpenmi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fqkhvyrl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jzvcwlfx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nrugwhcm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qojmdzth.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lmhbnmsn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2oaptrrfi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uiporwvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxyzgzat.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xedrspgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mocubqrn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2acqurxxc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zxzifyvx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bvhbzgfm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2knitlkbg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ucqaixcp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2eewrgwwg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ljsshtmj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2iygvszhp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2meshakda.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xfluuqrp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ponkrgjl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2flrdfglj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nezgdkkf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vreaqwll.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oikeandx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jaeqqjcf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jyldfbaw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aoygjnyl.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fyiwkthc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfkyvygl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2xqjvrget.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2jsedivaf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2akrtixiu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nshpxwob.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2htmstinq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2dvxdiftx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gicfhyao.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ekefeoby.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2tjphjidu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwkjzdsq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cpwdrynn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2enetnymu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvbcajxu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tyimzqsq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbnyacr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2qvvpazdu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2gbneonlw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ezovkyne.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kehcesfn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wxmvuwsz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2romdzxkd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2yqcbmkbg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ihacydfk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aoxvotcw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dfxjdpax.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xcdowrew.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gzyodnsl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjqvke.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wcthnnvy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdfpav.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2fewzlvyc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2envogtln.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lyezatqf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2grdsovnv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2cewgesly.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2vzwgihbj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ywtfflju.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vrartdse.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2evccvcry.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqawbcni.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ugalbpmk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2psznjqdi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dgdpvxmp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2orsczqmv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2zmvkfohk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hiuepidy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xqlgbgcn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2sklpskft.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pqgyeulq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wjpslffv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2pkrowmyj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pruqfdbr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ixcaawxb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aiozkkco.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ermbggnq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rowrgejp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zydgquax.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2mtlvqkrx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sshlvdli.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tokebfiz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2evcatgtg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2eofbwrjd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rtbannpg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zhwdxzfx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hjroixcc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lwsyzqny.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2xorjhpll.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pjlemokf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wtlponca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tinvwvid.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xxentnhw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zzvakxjw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvjuqfki.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2sfztsfof.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ihwnugqa.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2yykuetru.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgcprya.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tqwmrfmo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2kxhlhjaj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2jgknqzag.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2stryibmg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vwfhxxup.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqanldr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2srnfesrf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dqsthqfa.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uvoqtofl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvdyidw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qgureili.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hmdkymlg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vuvzwsij.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pnyjigvj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2otgpwxsw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2udknauqh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cfgjobtg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2oxxxwuli.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qqgdqjov.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkviffgn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2aiyuybsi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ftlmgpzp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nufkgpco.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcfibac.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2inazcjui.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehnprlne.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2drbbdbir.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2otcnpltl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ucwcflbj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hbtzhzcf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wdfcptdp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jhjthwym.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kyvcmhsv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vxfsigfq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2xzekpphz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qnsqhcth.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2khhhsjhj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2yqzdfghb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2iwpioglp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddnfcvmy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ubkyqieu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dzllglqi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2grhqvfya.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wzokmgfw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bfzgeims.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2wrigigoj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2tbhzatuc.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wwggmwuu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vvsljbwh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zfwjsfmj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2umuafgue.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2abltooqs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lcrhepwk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zumvxprd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bxrcpbym.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xexucxwj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jbfnopsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fenmxigh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ykxzxfzf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kptvqpxc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2aemzlgtw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2cfeucxjz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2axmhzzce.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dvvhtfob.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bkgsodrb.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zogvgiam.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svoknqmg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2jfqnupdi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2aeijdfhi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zpyigrcu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qetwpfvq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2wrpmumuf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bymepgni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2easbjihh.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ijpyekku.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfzdommk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2yntqqeth.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vsfhwcjw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wotxvujk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uxiqpibt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2jyehrhya.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2bjxxucsq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2xesdsbjh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2npmjmrnq.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vrpynclb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vpqbxnsi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lpvhbdra.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mjqwjurx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2paxudekc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ohnzqixl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rbkakqfe.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vmdszlbc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2gefjugvu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbtltpe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2jxjavkrj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhdzveei.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2cfgsztfa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zprlopdm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yqdapxfn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pjljimhy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rlpoligl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2mudhifeq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtasao.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mauwsfbm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2wyuajinl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hwkufook.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ajiiqwnz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2evwuawsb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wxbcaipp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xjrqrgcr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2juftdhaa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kihaxvvf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ywobvsxy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lwckkqkt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ybediywi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oozlwgnb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pmuoocij.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uhfvmyby.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xtuddpak.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bzktucyz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2gqrvamsh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2pnkjracb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2auqogoju.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2scqwpfaw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhaqzena.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2tqgsyizn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wkyipbsi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gfypjkuj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpmqxjlq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ztxgodgp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2calihdkc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2huawavkt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gezsclqf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2txvnvgty.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2salknjfk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ksxtdyyo.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ydzzvduq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2odhzeioi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jhumrsrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adtzeoyr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ohugpwkw.html


<!-- 参考信息 -->