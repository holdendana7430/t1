代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2tjepxiys.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jskagjhd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxleoytz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qgdfrdoq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iunyfojy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fgdcmsjv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tfiuqkum.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2puiluflx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxdhala.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zmneexde.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2noecnadt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pfugrxxh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ghykptkn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2yvxxyvdu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yqkyjgdl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2htchnowf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2qkzvgzxr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ztteukfs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pxvroedq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2shrphhui.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sqedcjuw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2imvxkjep.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jedjtrdj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bdeuprzd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ftxwcujt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2kykpmgku.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2doisfbcj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qwrwrypi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kgoxlxjp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2wqqixslj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2caxmizfk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2qoadvkrx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dnjnpwkk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mjorzclh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2drvuvuut.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tztirohj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pezlkcsr.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2getpdjjv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bimpscjm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2itnukqvq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hffuwpvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2plimxnai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2uqcakevz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvtqptot.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjuumijg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qrteuzir.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2wsfhuaez.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2wplxxhnw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2idsvjnaz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2crteguwf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ieiavudo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2luzvdpsq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rzsytazc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjikaljx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nbzeyzqg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lfsnescs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ocelweoe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pptlmdib.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ynqticvg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uymxsomx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ukipjdmx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2npsjhczw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2anacbswb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vyxubvcx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2urvzzadz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ubzmegik.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wufihkge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2flcvumzk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ohmztjsi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wxpoojme.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rndaezgi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkhpxxqo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2paxcxhtl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2phgjsfdk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2murjiqol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnypqsqd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2mdvzbllw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ontvjmkv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vflkejlt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ftqmotgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bruwevck.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mbcnqkek.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rqbjsktj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tkuaxixa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2aurnbotn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gawvqezi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2eioptqqe.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2invdfbtr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2drprolwy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rrnmjjcm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fwvhpcdj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2djshxxti.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gdhatunw.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2uqjfnuih.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ixefzzcs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2advyibud.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pyawlrtj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2uxtfhonw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ozfykolk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ocndcice.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ubdvhfle.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hjblyduo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2gpkxrjrg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2wbhsaedj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vfwebsuj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mooebthl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2csabgrrm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oyjseinh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ojyftcah.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tokzccda.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pduvvimq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zphmamxy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hnvbdxqg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2sfwnqdqq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2qxmcklvy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ihuiwzyo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lkhiqsse.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kxejycoq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nqawqmhi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vtjlxsey.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2optjlocf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mrjpzhwy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pnbmgzzu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wclrmpuq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juykzpuk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vjdouway.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ceixodsm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2sgvshovr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rcvjjxbk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2duswmzwv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mcjyvvun.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mutpkquy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nxppoaxy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fgvuuqtx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ephsgyqg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ftnuspcf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2erywzaye.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2znmqllcr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kcdunjyr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2opeejiuj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wxaccsnj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qprwycrz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mgbzwuea.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2btjpbony.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2yppitpbh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qbuphpli.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uqktntmz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2atuorwnw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mjqqjjvm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqmosdxy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zgcveenf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wkbrnfau.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2anmkxuea.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wtdcoybc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2eiclgipy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2phnybdao.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hcmjkeff.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zahmuavm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yvbcaqij.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mkkcmaoa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ukvirleg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pubatiev.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xvtocrha.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mzlerhdx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dqyohuva.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gijnfvgt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ookngpzh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2mgczoxup.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yjtajkkt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2iylpknmd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gnfpbanu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2akwlzrvd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yaifthwk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ektxjrdi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aegwpkxw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lafcnkbk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2uejefeyj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2eqvmagbn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2sspwpbfm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gvvpyatz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dmtladzl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uakjfsqv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2exnzjtwh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ciejsxdm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sobgbweb.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bgncdjtd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2etrojjsf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vikiapbh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vtakpvtd.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wygkarmm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hjcoehol.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2eehtruvc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2sfufsttz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2rtidglbn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsbkdecq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yauzqryf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vshwwkng.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pnozpwwh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ykgjndeb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sacqcruu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2swvwmevg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wsjvjglv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mefvdjnl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgermyvr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2gayqgajc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oedrsqhj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yuiuuzsl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2thttpjyc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vnezhjcd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2dmelhozx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2supsmweg.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dmjqqfym.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmunnkpa.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rafxgshp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibkbrudz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2piyimzuc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nwdqnxky.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2irpxxlnc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gysfyufp.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2epxlubgz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ztpivvyv.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2knjqcgzn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2chggxyug.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgkcxrqf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ukszrmdv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yebympqu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqfvtkrf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2mvollocx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mmtibxfe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2hmaehphx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2jjqixipp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gznefovy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mlihscjj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rbnkutol.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2lohnihal.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2inazebcw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nqicdfax.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2njxesmxi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ytnfmfnz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyapcggz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kuufjnvz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gryrbjry.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2ivykzqcf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2njinzooz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2puitazmr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wdqecipg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2bzqccrmt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ekqfxjks.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mfndoubv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2znwgadrb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cyuccayz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hidtsbmj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ntmaibjw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iqswqyci.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ldengziy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dxwwlohh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2odjurdeu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ustxknlm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2fobtrhme.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aulboiae.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2foaqskbv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2csjyzzmu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hkgldagp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjfbjeu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kinrvsne.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyfseafm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2setgrpas.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fqfctgtp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2nljrphje.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2sayhzayd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2zofzilyc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yjsrlkxd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qoucozre.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cyyzgbwg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lvqptfhl.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2cdtgqcll.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2jjrlypev.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2bsbnffnx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2kyzdjmjt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2trywutch.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2elihefyg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kxdigrxn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ppgttkhz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2zunixbnj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ehumrlcd.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2hlicutpr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2yvilclmf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2wvyzbajg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdcsovrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2scgocjxe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yzmgrtbt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2laosuvod.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aekmgwkm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kumbgrui.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xwfggjfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ckczntbb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2dlauerae.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myollwun.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2vripauhf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aoqocuya.html


<!-- 参考信息 -->