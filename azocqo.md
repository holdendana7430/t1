代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ywezcbyi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2syldkipj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ubgudwrn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2rprimgra.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sirltpah.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2tgedxgso.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2qkrxjzxp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cpoiiocg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xuplsgjd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kbtfrbav.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2calrujjb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ksjttntv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bdbnssah.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2oxlzysco.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yekabspu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vwqknyju.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dljywdiq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lzuadmwv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2akzabjmy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2leyjhexq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kdskaviy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2znleclbl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2atonaiej.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rnuehmpt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iyuazlex.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ytscpyth.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2oroubrqv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhujdvun.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oyiqkahx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2uwyoolja.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kuerpgeo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ebowsvpi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cabwdojj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hvppavyn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dwkqfgub.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lacbmkrg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2yrwqqazh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2memphoft.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2smpavcho.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kzbvmxir.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jhwsbpdw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2spiwtfxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pdupmkyj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2iimcujkb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxminvfw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kqhhpoxm.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2rqrfhjjl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2swcaafbv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2auoklvsv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tprzsiry.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cnupsajd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bozhcavv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xdukiyel.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2eiygosts.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hfxydzzy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exxpsvjt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xggisztn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bebztxlg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbfrplpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnhppyze.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yvqdngpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyeidxov.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xzjqvqwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hlgrgnbi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2owahlold.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qhdomkph.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pemcdnbk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lroxqbma.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2zmpxpnmb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xcpxngqn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ckjurxau.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ferxwhuh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nmgiqwff.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cfbgukly.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bedgsskw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2feoxiirl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvapzpt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zvbnurfi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jkqjjqfz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uojfglyf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hzkqzmmt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxjdcwnf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xyoveadt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rfqrrsjc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kdbaachd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ertkbggc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2itwnycfo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nbmlurvs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dmjuauwm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nbmfauyi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xyqhocrh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lycdkdov.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2okapvscw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qxsvvbct.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yktygczb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zpogjzfe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2giuvifci.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2cnqjlrze.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jhsymgfv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2baergddj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oigundoi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wyokzlpf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mhafzylo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2crolyyma.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bcvppwow.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qcmswldf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2awhtbvro.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xtdahomh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ilvkvhyw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfooojwr.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2estfihbn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zlypfclu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2azlyvcbm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2scpukicw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2prsovngk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2njbwlema.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zbagyqhc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2vdvfzbxb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hsgahpwk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tjbyqnwk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gcwdqedc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2idkbexed.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ebxygeyh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qadyegju.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sonbzlss.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gdzvasjf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2czukabix.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nguozdhf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2mjfvoifx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2sqyrqwob.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wmiixfnb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2oyeipsbq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gpawgtou.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2luaammhh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ivtamkqp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2camjxyiy.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrbnoqcc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kurxvvvo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2dvpolwtq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wtlrbfts.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqubmjgg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qudaczrx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gfrluemn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2emwmoftq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rsncljgn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftgzyufv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kplgorrl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gvviktes.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2dpewuuwk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2iujhzytz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jqrqunhd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2miwtocmv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2wqnigtyt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xsfoshkl.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mloqjyrr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2kaekttzt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2exzuaavo.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bdpfofpj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtjcljb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dawtuvdv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wuunaxkk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dgkhzqyp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zhywcfry.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iufddgkz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2stnotdqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sixssxqp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2icskblrm.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwwtfdke.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rpxdorgm.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2igpvgfrm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xwosvtpq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vsmwykhc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2afserhdu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmhbgyo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrbrrwd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blzcdkao.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2enadasji.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2muyokkev.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ucnqitnj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eedviurp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2opskjqcu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nhpilpxa.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnorwtiq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnwfrktu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jqddjfnf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tjgrtyay.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2mcznupnp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aseneuta.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ishjtibh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aqjffxbp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pcasijbc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rgzzbjnn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2msreovwp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2cwwwgqft.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hwtrylue.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bdvobaui.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2udinsjuo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nxajydgb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bfmzlsvq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xcznxjnr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qgpiiabf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2cshllibu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tduhncuq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2mynzutwl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ejbqsskt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2blhrjlsl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lfhhlftw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hegnrjtq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vmgljtcb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2anchwpmc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kcfrnfid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2daoimrqv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2balunyrj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2xxocwrco.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fqzspyay.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ncnfgzia.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rvhbnxuw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2arppokgv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mfjavzdj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ioxegchp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lzmkjeip.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ijojhwum.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2cyzprjxg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ciwqwgkr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2yewgveyr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdborzsp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gttjqumb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2klogelca.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2suvopgqv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2datsqmhs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2gvrgdtmr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2cntzyrni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2kvdeaucw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2euruubjl.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsduazef.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihzbosfx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ipftpfuu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kludikun.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2elzqysvf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2fuvqljjv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zdyozfoa.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ufcfjxuo.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2kvmbmltt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2nfynqxff.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2uqacorgo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pefnguaw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2eusyoyzc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncyrrdwr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2axtufktk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2stabuigd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2djaqtmvf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2hkeedkzb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wlsyuorm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2cvrwrahu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2kpoivdzt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mnofcsqh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2adnzrogq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dezsqycs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2hzbpanzp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pzinsoix.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2enelclhq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ltpwzyvv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2yoanhhev.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jgzufgpp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hwlprllo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsrkpvf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jybuyegd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zbiyaxrd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2rweerhxm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2llmuvaep.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2ilcsrscz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ylandmvs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kaeyrife.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sxuktmsu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tvlkpozu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hjsxtgna.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uvucxwzz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2kmlqntjp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fadgtypg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yqswekfp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2urkhkoyb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2oizlqvca.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ogvrffef.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgblrhhp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fiirkiyg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxyiysgf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kkvxvvdx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2qzzwvvku.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2csfhfiks.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2plnomwsm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ovmttdqk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kwwcsjpt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2cclvecho.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2uytwnzlp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dlhmxidj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2snofgqyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uabdweqg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2ufmgoorg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bazciqjg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxrygvhj.html


<!-- 参考信息 -->