代发 wailian999

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2njaljswq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2evswftrb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xahpcjer.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kpgybrhj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2alivypnf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pahihqxd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dbwmcepf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wffcwzvs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kfcsaguh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2rwkcuonw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2gjmwatbb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mfavgciq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pxghgsrg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2isbmcrfw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ohlxxiru.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2touutent.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2aodztxwo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ygsqnnjn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bixiqcel.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xsusbvdk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gdekfucp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2yovtevzl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ctumnknj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sdlbfhif.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mahminzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhpcttl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bpnlglct.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wipdeedu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wlaywxfp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2njjzzfvl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2qbeigicu.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2vxjjvscl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nscnheex.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cgvdfzvr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gswkbvwv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2elhdvqie.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2oupronbo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2imqnhbpr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vqbprdzk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2npxwusav.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2trvvhlkr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uynwjxye.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ulrkaion.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2evfhoole.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tyrrxugw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxlnkomd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2sfxrxqia.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qwikrajz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2cvjdmqyq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2urktvnlr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ipdrsbhh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vtqmxfqu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vcjywwnq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2aifipzwe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lwizzkrb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcyvbbcm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2rzdeedmd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ziwirdya.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mpguvhek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyxiilac.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pdgsouzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahdohlgk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2oyrxhrgc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kcampvih.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ktpscgko.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mhylfjad.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dmureqyp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bpuryprh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2rdopusta.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2htmftbar.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zayxtmrt.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wmbwzish.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2nbvdpfxz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wkcdvgne.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aqcoqnms.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iunqbdzh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eeveklkf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2siwzomvd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lepkxtrp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qkrlqyva.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2bwfxyfbi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uvrhlofj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2lsenpfkl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2itcghifc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzcjmvvn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qugsbpba.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ccgsbfve.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dsutlafc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kyfjfuwo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wnpzvacy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2biyumqdt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2zcdssjsm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vkcikise.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dkejarwh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nsjubnoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2frvtgyun.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vmdidmlf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qvtmltob.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rnenomye.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lzjgmsay.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bfohxkzz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2odgrcmxb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vvqnxkvp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dgdyiwlp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xsqbtlhk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fmcsxfpq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rwvhhflg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2eyqgjiof.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpodyup.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jtxpjopg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xrbktmam.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qrxybusz.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2oscwhuls.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjswtmv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uaqxrtju.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ttyinoxb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pgbxnlao.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hqzanaad.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ilauhhbp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2npbvkmxd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dyefzvjc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wexuopsa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2beyfctsj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bhkaoeuz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mlunpwps.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2avfkqioh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kziljacq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hkpbwnyf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zxrgkejw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rufffiwm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2dmhhayyl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ecvensrq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ropececs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aohncwdd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2elyfckbc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vlpvczza.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghourqum.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2xethpkle.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2moomggwf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uhpzhmtc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knuwbbtg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vibkrudn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kprmuvgg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2pzotbfpw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2srsfbjiv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aurmvhgl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lhfgjhvo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sopawyxz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ucixyuid.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2sarhenzm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bzzsshhi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2erbujazl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xjvlyjtg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2isjnqlul.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yoqnztha.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gyrriheg.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iwrddxsp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cnqtclrm.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2sdaikkfm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uegkpvbc.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fgfcbpnq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zuwkuyee.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wpcldfvu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ojfihdwf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gksvfpgv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2axxdianb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rtwzlcon.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2foweuuss.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmlvztqt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2gpvfmcxf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2twjvuzmm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2xbnvfdge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2aercevgz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmawdlog.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdntgznv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sebxriku.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2tcmjpqmw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dfhayrnd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ilnqgjei.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nfalmjpn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2stcnkbgn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cgskzrpg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlnlzyfw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dukjjahp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rwsslnbp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qifsuquh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kzhoplip.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2noblgekk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2tdcohkte.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mpvkeips.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bbimrwng.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jvyacjvs.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ukvjkejv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2utwvyxlz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2aclzldys.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2imxhmqpm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vqfflfzo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gxyzzzgv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbvofyz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2khcyowyr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2drbwhciy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2utkxaiaw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tduasbsv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kivplvxj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pmadyouw.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pxltllhx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2aneymeua.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2grcznfct.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2mvdhlqkn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iktlpehn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tvisqsao.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2srukjgch.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xabpjcfi.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2zaudevwi.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2slfhmgau.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2kjwazsal.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2zvnnufbi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zdknkals.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2selnbkvq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ckdcrixt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2juuhcazi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mthhamgn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tkwquadg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iewnlxez.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vwqlbpwk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdxiixki.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hwgbginq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2lqwbhzik.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nkedxvwd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2sbrnckss.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2sjwvzqmz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ulhtfpwh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ucswadlz.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pbqcqflr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2oonkjtxs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ldpubmii.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zezentsk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2hfywitpq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2oksgfudw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uoufxpth.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nqruvsoc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2qoonpwnz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2unxyhkvp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hgzpqbhb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pomlzdlv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yivxrsom.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rlfybmdu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2osijtjbi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjhxmes.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kiiayrno.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2csvdjlgp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ngpgognp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvkmkcwx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2diidetqk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jjwqhufv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2reuqbbjk.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zzelzvtb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pjviuzyx.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wiloiuea.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2scovwinh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uviqsqmx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2losouhgl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2mqwipxcr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ftxtusws.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2livfoxcz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2sdejujgg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xiosfmxi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2eluvxcqp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2fjapygat.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2sfdyahuz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vqtwtryd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sehhawla.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2qqjfynlc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zgyowone.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nvofxgkq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2gdvkaaht.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2mvnqsewe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2etzxdccv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xtzfuvmb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2iitwgqkv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2iyzmmhzz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhuuirbn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xbuqsvjl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gjvxiymo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bbqlxmsy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2svmqeabu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vstavzff.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvjrycxk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lepihmxj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2azfsdeek.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tncbhimm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sbiahxrt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tyovhclz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2eexjvhye.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ogwbczpx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qaxrmzyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqvfzwlz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ywtiesyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwlgfaee.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uvlpkywf.html


<!-- 参考信息 -->