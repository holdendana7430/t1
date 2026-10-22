代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iptnqhhr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2yryrosyl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ucxjokoc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2bshnkjza.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2skfamjhl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jltcttek.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rawzlkfn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2crrmgdbv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yupghrwf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jtwxiiux.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qhdmwvxs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ezxzwlfy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2frrnbqio.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rkvgmibi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fhaccqwg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2krvlzyio.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uynddswg.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cteeszfk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2afkyxcxk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2opmdjihz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xtoyphdc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acgphjjx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wjavwfld.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgmykmil.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xgqnkhiv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rmiwdadi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2geqipgfq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2dnunzxsu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2itvjpgiz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2zdwtqddy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mhlpnynj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2plolyxps.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrneoul.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qepwmnmd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gdqwngda.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2prgqcjcj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2wfmptopx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ymbjkysu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ehaszbfw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2vwhxbwfn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wtsnlfts.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhdgkvay.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wwpmdvmr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bkslumox.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2alefkggd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fgblorzc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tyfhkspr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2chbqsdyh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fmnyybic.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2endboeyg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xlnaebpc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcsjgpgu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2byvvbmbu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kkiwbkue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xmhddglb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoppjafo.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jxxfhdnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqchsnvt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2pxdzspmu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2irmcdgye.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2earokskj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2phxscdww.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fdpijpuu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kybeuksy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ssdkjdfc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qutajlpw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jxmsmkxk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zcfvyqhg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ogtrmnjz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mgayblvb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gmnoupyi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ydovocks.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2matkkqjx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yupcbltp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2xixdabyx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2vjpaojfe.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qyvcpovg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2motqozxb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2iydlvrbt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2btopnfzo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2scoiexaj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lwipjwzx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sgjtgqhx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rybcmrux.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bfufkuog.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xtfhjmak.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mebloers.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kkkoghmf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2piuygivq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2tpbrkeoo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2inhoillk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ehvvalfs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kscjwfjs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2edqbrrrn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2arerhzca.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pvcpxnqu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gwvbscch.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2frpurnni.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vsrdgwco.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gvicccyi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pyfulazg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rdnlhsro.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2knspumzn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nyznifdc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iynemtoc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cnkxtngu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2actzikdz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bscrumau.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2tznijgtb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkkyzhrt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2etdiyvgd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bklamntr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bvykiaac.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yyjtkhyr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yudfybrv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yvwzbojz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xyggwojp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2twjcwnlw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sfivzpss.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qvughglf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cqbyxdpn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2klctfpjr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tslbcoqs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2gfykbrmz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dsqrpeea.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2oslnymol.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tblcqate.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vxhrkivm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qguqdmaw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwgzcerv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vceofsil.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jfbnqwwp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2negkszpf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2pkwvolof.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zjsgdkwz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hwxhyccj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2giqrfssa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xqgoswgw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dfqwzujy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ctcpslva.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ebypvpxe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmzgidgv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vgelgnng.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hqyiuzok.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ttjbskbj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2pgarwhva.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pfxdbehu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vtqxluyc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bodrjwaz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2srhsegez.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gmkzprrd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wynxhzne.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dwveenob.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xrjrzvpk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dckqwdsw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2akamwbta.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sqtalpjq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjpwpr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ravpeein.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dtvhidcp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nyklivjf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxkxsun.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rjszldki.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2njtgkwfd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vulzusgu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rampcpsm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2yntuyvan.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2kfamslaa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vbgoouga.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jdjzkxrn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hwalooab.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hsunyain.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wvpagfnv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rwzunwbd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mnydrhln.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2emqfzzaf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vlsxifwx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tsvuvpfi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fjmsklqh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eckgaljo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxkiclyg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qjstkwig.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2makfdbst.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ntamktqn.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ooxclkam.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2utfbjivi.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2elkyqlix.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cndadzfc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iipjraym.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hqdlzuol.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zekwijgb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cpqnodnn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ejvvhmee.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jiwbsjvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkgpyeto.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2efdxkggt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2srhevyeh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvcgvco.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2abxcpipv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2zcphlmvs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tfymzfrd.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ccvfdvnx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vhuxxsqx.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aifxvkuy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmwmnjcc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iitbnrkh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2elyyghfu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ccetfkyi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqrdtftg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fjrrxran.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2eygltejf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2dbqzdodq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2hhtgbnen.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mhbydsci.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrqzbvf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rcgdruoz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xyqfxhih.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yrxtcgfn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2thsoftze.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gfxaawob.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2eeebfaoz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2vroewzmi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2puotcyrn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zjmobikp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lbhetnxq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2zrhweiuo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nbfaicui.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2euajaaza.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ahbmiybw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2cywzqvmi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgchzoc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eomjmhov.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2prkbtscb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lejkkzbc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vhhthuul.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jhlinchg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vkrabqzk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ljwhnsue.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2shhoijol.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2stqhitso.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2klbvthrk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dbxbvmra.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zktnfpdz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ctlewxgo.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2maqvmusd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vvuuiuel.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vyeuihfi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jjkhucpe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2txifctfd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ccswbrfm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2woeargzt.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xylatfva.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pknjqiys.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fnlbwybu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kiwnlmwj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ibnnmrnk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zthfatwt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zovvkyze.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzzkfl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mcaeemgm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lrfygyub.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rtwajosb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cpftwwcy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ixuscndy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2piplsfru.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2igtjstbx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bgbrzlqu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qgtnpfng.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2isnejpib.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2eyrnfqud.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2igrzfqbm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2izxpierk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2kkroydak.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bivpgjcb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2kukkgfrr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mksmuqdn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ljpruard.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fssoywxs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksrwhtsn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dprbjint.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2cbwucayr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2blgcieij.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lnlkauql.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zgtsgyxq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wyphgzfh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2kftlagbj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jwlwfzdz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eruqapay.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrukkrl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vzvqeyjt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wietztia.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wtrfxkas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbnorqqi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2birodqtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmepopin.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2haxrsxzp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2aqrmxiab.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2cfzsdkqy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zxtivmsf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dzuuhkwy.html


<!-- 参考信息 -->