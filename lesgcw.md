代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2istrdzlw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mtnpoubw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kzazmrmh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2lasmbbnz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2hgnikuuu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mghmfbja.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wgfihuvu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2mjcudppv.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2nzhlilgq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bxwwmagq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aiamzcbo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2fvkwjvas.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sdxdqctp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lxmsthrp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fwtjqqax.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hdpyqfyc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zuzgtlac.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2omeddplc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jvlbyodz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sqoyvkir.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nofgxbij.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wohxswtm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tjrnpfln.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jutgkayu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2amuheztf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2awygtavr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eoipcqzj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qwzdedbk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2skxuewbc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2imiszmcx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2scqjpkpi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pfvdclhw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cklagcdn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqyiejl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2guefnzok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2udlzwudn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uocirdnh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2znenhtqt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wvifmvsg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kdhlbmvl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dasmjdmb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2euivwoti.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qbhrqnrm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2scqkehhn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyguxqfg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wahdflla.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2oeugxluf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dukothmb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fvzidest.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wtwnhmjh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2krttfwvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tvvbtzhh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwoqgljg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kxmuvibx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2blvkiwxj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iorjicnx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qyjsvsek.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2iaqqdogb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jyozoacy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lqhtafhd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yvqvlutk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2xskqcppq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kxunwgqm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lezbizkt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xgvueafr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2olptlgoc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2cjnjiysc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqcqopmm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vsykgcin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfulayie.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cvqdokca.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rstmddhd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pdmfmray.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2gcfxifdn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qclleteg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2kvvhhjck.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bzwxlytr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2inrhbqlq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kuxiugrr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pbxpqyup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2hsyvrvek.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lsxtmbrv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xxhpgpva.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ajjvemro.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2xbkbknxs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yaafyhap.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gnhwnwio.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jxbozcgp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jptwrnnl.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vapgczcr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmmpbzkl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nhoorebv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ozlahxfq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ytoxwnbc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2swdfeysl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2doqwgact.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zlzrtvlf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cwndbrom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjmbglgg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mokheqsl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2zlhssywr.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ddfptvlh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ppcfpejo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xazulerx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cgmfwoax.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wgiodzhj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mxtprigf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ibzvllhe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uavulbzw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xezxvrqh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2accpxswv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zezkdxfb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vcuaakqn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ynwevaki.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gxiydisq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mpqmxzah.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdapobw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lvooxygx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xidxsdbm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2afmeoevo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nhlgnqvm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqfdehof.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sbjlbrtf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vktsxwmr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2agdkcgqm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2xssymswq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ehgmxlqd.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tglnzbfr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2krjjnylo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oagigdao.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2edovfuhq.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2dajrsghz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gwlzqrze.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hgmjgexk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2riadhbsc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2eketeubt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2jqdqkaoj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dgcrkbxk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmrhjgud.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lwxoxcbj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lxtdtpsr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2etlyrsfk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wwrkgqqd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zmdgltja.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zmezxzvv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tspxaboq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dsswazgm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ftlxjnlq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jkkhwpst.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iuhshnei.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gtcdoszc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2xacusfzb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2txrtpuco.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zeujfggg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wyrlsjrm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mvbhsonq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gvfitvko.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2iggqvrqd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2iwnhbhpx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2kzfcdjbk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ltppsbuj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xvvxoxzn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gsjshwmp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wrlvfxvp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pjqzpyse.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ndkssqrq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2swrqwdro.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rrpdjsib.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rcdgcidb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ujurmeud.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2blsecctt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2sssqiksb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qsglwggl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywpkhzsy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2drlhgavo.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mthqwhqq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2irvjctnr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2srseatyi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wrigckjv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yeteptzo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oxoswrec.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zrqpmnsy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fuksmuux.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aozseite.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2rkeheoox.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2cudbiyhj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2erjczzdi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2tgzzelmq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hhjwhjkh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fergwvom.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2phevwpwn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rifjpqtk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2srkeszga.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mvbkbcko.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cgrnrfxv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ujkcclvv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2xwzfgvkv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2eeepvwpc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2geufbiwy.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2werlpqdd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kztinued.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nvvbqdjs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wncppdtf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2shkdadvw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lvsxyesd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2llatrmwr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bxlksnsz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aqxutlin.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nveeoxsm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hutyfuyk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2acqczmfs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hildsnus.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qvtwkarl.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yrlhnefd.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2azqlwglg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcrsmspi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2omhpmqpx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fuktlbvh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tkthyxbe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2srlpqbqe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fsykxoya.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wgszfmiz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2aqeebcjg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cttxhseh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yqltllys.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2akoyhwjs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mqrhfbfk.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ifjmkhxr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gaaqrcee.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2avedpofi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nrmyxhdp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zxgnuvyg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2xzixtdzm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luvcscjt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vwgoiihz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qqivjihb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2idybewbw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2pibqkpyk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2eoynfers.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2rsogwirl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ilcppjrm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2omddbwaa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ssnoznir.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bzobjchb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2byndfdyg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bnjikphs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uetruarc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jfbrqaio.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xlpgxrvt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2noexexwu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mqjlrxga.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2bunrcuup.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2oavnmevy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2illpmbic.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elnhmqho.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rltopfsi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkgxknzl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hdjxfich.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzjausa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qsoimjlc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjibgdpu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vktgfzev.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gvvvcogk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ybzztjzg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cybastph.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2klxaxsfg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2pwvvaotb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qnxxmuae.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nkdbcmpg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zrndrelr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eknawjko.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtkwhud.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bzieaimp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2hthzsnug.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vuahrost.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2fazhzayk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbpmnwkq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2dmodrhci.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gltrqlrz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qcbafqfv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxaioqsw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rdezimki.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cmtplecl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2rrxhegde.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2fgnhytmw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xhyywfqt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ariwvsbk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cbofjcse.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jzshigli.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xotnwwqm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2srjmiaen.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jfytasqi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2souzyrlr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uaipspnb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cnpgqyus.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ahfudrpr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2oyjpundt.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2isjnqrww.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2rmfiaagp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2manezpji.html


<!-- 参考信息 -->