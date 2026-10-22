代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2smvtsbhq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2skpagaxc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2szrtftad.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2desdmwwt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kvqmxnpj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wxpfjjon.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2sronwsds.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pniilbkm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bwsglnaa.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dleslmax.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wnxmovpp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2keeovnmt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jijjrdlh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xxreubhs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2naqajloz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vhfzjsdu.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mltltdjl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aodvqceq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tresisui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xcvavrsg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eewxiykr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2fagcmbib.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2vrdoqctm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tgqnoulx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kkirshdy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xqlqaamy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2czcrcyfr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pthpeffu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lndpbuol.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vzypfwiw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tiytrmgg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2xssziwiz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2azprsvug.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2bdimqqdr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wnbieeln.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lthmbmon.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2onmcxofw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pwfssara.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixilotqn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2kalobzyz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2prkdnvci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ulizeron.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wrasuxmz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkfouveg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xiamnkcp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2swaebenk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2yweqrnyb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qtzvwppo.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uduhgzvs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2oenabehj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wdhxomkz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tflhumrh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rekqsdgm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2sgkdoziy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qpkqakgr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tjdyhiup.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hkfbjtfq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xdkazebu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2amerbkay.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2liciczck.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tiyuydup.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvuesocl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ssjgrwbg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ojjddage.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vocflmlz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2trdjdznu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hxhpzpnz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kcenmwjv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2movzmijf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2pzgbktjv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hqodhwsq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ieucvala.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mbfctsxy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2atbezfxf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yezctkcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afkrpvtf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2djlbdlkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkpiyqsm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eklpuwpm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wkeivcja.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aggrcmcc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2bkjdjptj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uohqjfef.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2yjwpntin.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2pqruvgaf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pgyjxugj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kxonbeop.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pejohkty.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2shxmpbbd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2yefgzoxx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ywgbgpbf.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wcautwvt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bzudthzx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tputczym.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ggwahedd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2leronmnj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ofgtsojb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ywwanamv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2cbhanzyl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fljzmaaw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bwbfecir.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pqztbaev.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uobzasdn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vksgrvle.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jiadsarf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hcwptvgv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xjmztsrg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvqjemle.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2agpxceth.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2jzdslonb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2iqsbglhx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kgeypviw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jdqqoeev.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2synxabow.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2eheoitth.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rghabeck.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uqlqeevp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ndnrbriu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2skhwcmih.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2dfxlyioi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pmnkigtq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hgovdjuq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nafpvhze.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2pljdjfkb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bsedbpts.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2svohabdn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vmwmsnvl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uiwjygxk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mihcbrbd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2soacsjbx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ijxtnubc.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hgxumtqr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2uerlnwyo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ikyyjmxd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qrluktpa.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xkugjihs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uxgbxlyr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2glffzwrs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ysidwhzd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yyxjklsl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eumoyuzw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2zqfykxzg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fxycfchi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lvktibhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nodnnjbd.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fsufqmik.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcnaixzf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gksxnpyk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2upqrtwow.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hehxuxhj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jlnyvkyk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2twvhtlmv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uvoasqkq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bznjdvlj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2undcquqj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2jjwagqsb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vfuewpgg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wlbhqksb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hnzbxoqz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2lhcsxsrg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kzqinneb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlykgkjz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mvljeozh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hmouhdhf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tudopdse.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wvuscgza.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jvujefch.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2bufsitme.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2krrqrnwo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dzlujtfi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mqufqixv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2oumnnmmd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2efohrkwe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jmgaxksl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hivekuah.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jxsjcgyq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nucbtkyh.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2zmrdwdbl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ccaoronm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xqckddya.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jrxieenw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rmgoopjq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dzibdkvb.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zjjliftb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcrbtitl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2cwgoyrtz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rrwpabjo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2sycyctki.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2imvevqpq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kzpapahz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ymrlavsv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2taogbnmw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2kqklecnq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2tjhhvrjq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pskmfngq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ivkulomx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2datldtde.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hkkvyipk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxibhevw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxqfvmvl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rgaqdbuq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kbbenilq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vhdewner.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lziahwhz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2oczldqxq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2wqvimgzh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yaojcoel.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sbiyyzvf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2poxlqxxd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2hisdkfph.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lacjukok.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2pdjktvhc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ofligugo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ditrwlob.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ymizbuvt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xtqmzsja.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2fglmhwfr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkviaoha.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ludwiyss.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hnvkoxbk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cbjkcqpn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2uwchalfe.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lxqfmpfc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2voqmgjvb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2iqslnede.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvtgmdd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2gfzgdkdn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jpludocb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2htdacnii.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2atftvfne.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2eegwrzep.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lyslpfqn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2lrlpajtx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ktmmysbl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2tnpzupvj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2yahfrjbo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vpmkqzbi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2foxejkkt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2elclnzac.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xrljjwyo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2siudvgvr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zdyostgc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2knfqdjip.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2mgrkzbmm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2anxvdaer.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bkbzxyaa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bbkcllyq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xhhykdnw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2aoafyrgc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xgfuoacl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vgeepwlf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hzkihuhr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2eatnzeuh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vttktbqi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jwrhobaa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2usworsgd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2svhdrfay.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2graoqacy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2fchwmysg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sbewxhln.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bldfbpyf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pccbaucp.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2idzratry.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qsirnnrm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvyqcxjx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kczabcpn.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xdpqapue.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iofcadfc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awfvgzfs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2noechmed.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2spebjbsu.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2lppozwnw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ojqythza.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2edxdakuz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qedseyik.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2akditior.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qkrzkaoi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gkadndft.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2xbdikyjl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrwvnna.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2onzymjij.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2dlsjahgg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kkjifzjb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2bojixxin.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rjmqjwwu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rxjgixtb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tfluaryh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ywgslhjh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2juebsfzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rwngrgio.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2lojuzsja.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fvlsovli.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mjdhsida.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2keoulnfj.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rruefoco.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cdghlhwo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ltwcxqor.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qehrxfiy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vztqsuto.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fdkohrzd.html


<!-- 参考信息 -->