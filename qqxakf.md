代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mssnpyvw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2lhfrpipl.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rfqklyuj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ufsqnath.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2aiqkpjbr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2latsvscl.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dzripvtu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ampyqpju.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rotirplp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2tqspsowv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2dubckaxd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qiohrsld.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2igqzvukm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2eizstdvq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pnxhhvhw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tvpqvgfr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rkktenlr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2pbodqymu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2caotmlvk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wedoonkn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pxulgrau.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pngvscbx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2fornusvb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mvpgfitj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2aphorlxl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zpvaqbsv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubhaglks.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hevirhkd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fnigyjtq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bxceojbl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zzjuoygo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gabhdeii.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2plblhyfj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2crbfiusc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rlomzmvx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ozllmpno.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2utaealau.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ymqmgaib.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ldcdzczp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wwnstnrz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjleenim.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mokbpjbk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iuwdyktz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oqsgfvet.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dbeiiqbq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2clcquvom.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kzthnxja.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rrfptezz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jrawzegb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuxqyyqs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jbeakglm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oortfuts.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2zruamkdu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2diixwadr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bvmdjhem.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2smqhgfmq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2jpjvddfj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ermunwcy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2woxmgoej.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwtnmiwo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gogxtnlq.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ufjkakov.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mtqbljkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sutbslbd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zfzmipsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cssiphyu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ghanuzvh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gtedyskd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gmyihvkx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wpawrqoq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2esfquhov.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uvslznbh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ibtujcnk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dsiodjkt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2byinjpic.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2isyczntj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fovrlfat.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ngefispr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bmndoxrq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qyiqvxxq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cxmqcqpe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ohwgpbmq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2kzpmiqsm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zfktpmuo.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ygcoocag.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hvmdiloy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uhvalqxf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lbxmvbnd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcbllbxe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lshlpwjm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mosbehpj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmezquhu.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jiuvewgs.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hynwmwhm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bujweypj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wrlonhug.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2smxsvrhy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2yslxxxuv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oggalnty.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2obpijllc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ydhisbnd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2iosadcbn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yyhpgpfb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2imgicaxr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jadsbpph.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hngyiqel.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2obftkduk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2echwyphi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hrlmsyde.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2conastlh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2oozolasl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqvqffoo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmmgoguo.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jurophnk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2euqogtql.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gltlmnga.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2hjizfrvp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bpsoprnw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vghxmltl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tfdplwyp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2nhangkhe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2idxuapdo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2emegpcgg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ytwymxxg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjvooxey.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vrdvqqtm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fpdmuvux.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cyunfrhu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dnpzjudo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2pnncbcgd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nubasgjx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2aranigvw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cdopzxaj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2eoalksdx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rhahaooj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gzsrnuwb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2bpihjeel.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2innitjhb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2hqxohjgq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2epislevs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2irigpssz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2zphenovq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oyjyaulf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2stfdzqot.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2itjwwmdm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tncxkaol.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kvrmkelt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nszvhdld.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lmpszkkv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jybbhcan.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jiyrndha.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwrqcoo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2lzdydquw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2elgsliou.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2onkhuzij.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mgqeawtm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2utosdftu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2hwmkvbdy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxwfwtbp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ecafzcxk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ifdswnva.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2alwjvesb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2keeahedd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rzuugwcy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hiskkgua.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vbtkvmnk.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2maktmevz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kvrarltn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nxchbptc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ilawkipy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ikllpgcw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vgnjrtep.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bhinnnqa.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dehefnvf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nqxkgfur.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ocuyvbdn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hdwdyxth.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lmtffwmw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mdpedhsx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uzehylap.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jpvorxfo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cieuvjtu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jyqkhgcz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cljtkaml.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2whleeicd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glsqzvts.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2pmpeqata.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ygdpwuhm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2utxvfvae.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zjmoqkfk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhmxrggx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zxznxfgg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2zcrkyivq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jqmvfemk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pdodkrrh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jzaiurli.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jgobbciw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2gxdihnxl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ptyvouxn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2eipioifg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wjagnisd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rgsbntgu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2vruygyaj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlxyxgfz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ocqojfys.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvqshhq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2abgfznbi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ruqhmssf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vldedeib.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ptjxxcmq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qmakwozf.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcjtweir.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2lcvhxnbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2cnaxfpfs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2drkdvhpy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pxietdeg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2yrpocjqs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kchiiibf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2hbwgfsbk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2uxrilfty.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vvqvjnvg.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2afzannml.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2szyghqdl.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kypaiujb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzfekvmy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wuwoxfhl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lswvskdv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbibrnyn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2iqzprdpq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2yzsaeyru.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lujmlcrh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ghllifxw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oowtsedi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2drfiirxc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2yfkwgksq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2muwdtutm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yfqbilol.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ikoocxal.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2esnwakpy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2abmfzmnm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gonebsfi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qrlwacbb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vmovqzlj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2huamohlp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2naqhqcvy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2bzaaumwi.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tmfgmmev.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hzsbzeiw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zqumtblo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ryziuppi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yplvejwf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2weqpfbpd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2swqsgjwn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2dvamivml.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iamizdwd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2dvxqhmgs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxchksmy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kyoeiqus.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pkqyupbj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wyvtewnl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2dqypxebc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gqqjfkpb.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2pnwljmpy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qketbrin.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qyghjvlc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhxwjcht.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dsjugqqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ntiylyjy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2opkbcwaw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2yvcfvugq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wjlscgyl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2tfzfhjjb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwhlqjhd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2fpoacdtt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2orthnshl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2nyhctfzj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvxzgzzh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqqbelds.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ptenrnaw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2gcxkszmq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qwfkraql.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2djynsjdx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zbvbqhka.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2wnhcnnwv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fjctdzaw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2trdhwcsq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ikrrpsjm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2czeuzueq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mpborzem.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bckbyqin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2gaminuxs.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ltgnoxuh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yjlicnsi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqpygxjk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qjbyknul.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xztbfvyv.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lquctrxh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2omouflvf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wytlayiv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2wujhsuzt.html


<!-- 参考信息 -->