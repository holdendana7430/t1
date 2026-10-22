代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iqbecttk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2avifktth.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hylhwybx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sfedcxba.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jlsfwyvx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ivndxrle.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vvfllqbd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xduuoyzg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xcjwdyir.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kclxxdex.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ancnikxz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rrfezolg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ysckjksf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gdrbxlpz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lktfljbb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kgxrjxhw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wvpzfgyw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bvrqabxc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gheoabqu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hankmbul.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2upkgptbi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2hygyvsok.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lxdwvwqe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jbdksxyn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eojthbgr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2inydosit.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2euuprpcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kjsxwfdj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2akoairhj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2vdvlzkfx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xtynjwwn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yfymibme.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ozkwwzmi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2rtwzhkyw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mctikauo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gsdmyfrf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsoaekor.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2qrrnoler.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jrphchuz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fjflmmyg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2erdfzemh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fmibmbfx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2aswzgtwe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2rpsarixz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2pasvrvjj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycbnwjwb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gtjbywfj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fbichlhm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2abowujgb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pbwmajho.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mlpziriy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kdazauqo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pyywwywk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jvzmwxrc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2egjfjaga.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwqitvsy.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kqrifbhq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zgfsweti.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydiwaboz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fexefzrr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yxpryaue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqhaoplc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wsjgjpei.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wrvsdqca.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2toavcser.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rnrhwbup.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gdgcjxnw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kkqinzqu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mkmhxvmx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2zrpfmtux.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qtbakphw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rwubhcsf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ekksklyi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ennvpwga.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2urndbbbi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ewwrlgvm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkeuhnbq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2oayxejmj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2puhkyeyx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wyhmuqki.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2fnhvgexa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pxkcbmzk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gxozevxn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hsiynpnj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mxwfzsnm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kfbatsxs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2baqsgrpf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xlslmqmw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gioylovw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ssmittst.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qspevmez.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qjdptpzv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2jhnvpaqr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gxrzvlnc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jppkwlck.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yfvwmuda.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2exxwqfko.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ucitoeub.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zpuevyfp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ataadjyh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hohbkqsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uyczrnpj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2blijzhup.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tlwocyec.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2esdebuqj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2odnyzavy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zhvedkdb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2frermlwf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eslmrria.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wsauxvhq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kopxczxz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bapxtxdm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2qzlvndyl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rsuljbwy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2yfsowszo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ynlqjlir.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2exrfxgtv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2yzontbcv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wyiezxwk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2loivapkz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bgttqokt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rtvbyplp.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2juwtmltk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rykrksec.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbnbxvr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2nzfyomxc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gaplxiel.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2uhptybii.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2afiyxuqr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2sznhbvqr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjjtrnbj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rpqevrgj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jmglqhhv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jabnpwio.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2octorjdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wfaqryjy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ompdcyqk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zldtbjqu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pzrlsjld.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rpqgpxmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjcxhhw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2kkutiufw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rmossopa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2tusakbdu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vpwvowjf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xrrzcnyu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oeftayct.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yjveqhhj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2sczfvvoe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yhxghepo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pawifdgn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kboohqhu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2hqndjcpr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qkpvrpvj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cthiahoa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zjsbaodi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ruxttzux.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2diovxpcs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qydfqlag.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tvjpmkat.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2taaoolup.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lepaqmqn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hzcayzrb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ysffuyuw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mapalyum.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xwebocyw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2dpfnynaf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2izmasfvx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsgloplj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nxohijhq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zmwaeflc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dfztntht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bqfrwjdl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pxligorf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vsydrhtw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxvdbwyc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2uzbvnhir.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2fvocykyk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yoxuqxcl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ijdccxhr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2deqkqfsl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yjmvehyn.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzmrydg.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrbihgyu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejdjwfil.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2exuyrbxt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cozrvleq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2svgcabek.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cilqezwd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fgarnduf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yjzkzuaq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2icclqhhi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vbtwximu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nsepdoit.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2gcqzxjis.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2wrklyjtv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uejcgeai.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2asixbosi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ytbtkwup.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2zelrrgyr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nxkxxejp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wyljgshe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2usvtbvok.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wntgkyuq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lljevmhm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2rskystsh.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rpmcglqk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvbvwpy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vknvrlvk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rnhnffsp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dkcgwccq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hgqmfskr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwybatnj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2uihltnhm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2fuyfawku.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nnfwidlo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jkcbuxtb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ueuqnwpa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2bnjdesyr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2tzehkmxn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmbuyptv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qijhepay.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2uywgmmfh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gayxjjus.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wjrjjvlb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pqmgwglf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dqdqlkka.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2rsddjtkk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2upjyajbr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ngepyzmx.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lncwvalv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xxfeihzw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2pveberva.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2akxgyzxa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2neecpwmd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pwdxklgu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bvonvqvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kdejfznf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2earqpyqi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2osiosqpw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2luqufqyy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qnhoiadz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sjmrzork.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2tchbnykb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bolwztmg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwvutzdn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lkyybcxx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wijoqfzf.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2freoefta.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbccwfgp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vafpjkht.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2tcsicyxr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2okevzuav.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lddyijxk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2brntqcrm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2josqsebh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fvrjithm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzktruj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cesiicha.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2cixzamqd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ukisfpkn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ehaczeco.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swiygwvu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2waylksfq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjrqjmf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hoxflwob.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tcovmtnm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wdrhjoql.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2jbdsgvpt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2phfllwcq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2nwbiqbeb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wyvvlrnr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zoehmvej.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fqirtyjm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2awwfewup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2tnogfblr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pivyfriw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kjbvuwuz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gaverrld.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2lvxhiemh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tflbrjgp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2kduhoiqj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2qrrwlvwl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jeccxxgt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rapmmeul.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwaabele.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rmxdcuqk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2srjjqnpc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mqsodrky.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wjcifvub.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xrpgavym.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dqttgimg.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2umdpmlqs.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2knnpxwxq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ycvxeydz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2xyqjrvgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqeompav.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2egrtupsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vulltfdv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2snacczjr.html


<!-- 参考信息 -->