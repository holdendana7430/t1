代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xopezegg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gznzzxmm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2cvgmatqd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ugpgqdyf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zpjwsznt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmpsrhv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2etjirbsb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2glysepmq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2hjxkqsuk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uatkfuol.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rgxmcjoh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ahvpeytx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wyraiwip.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bnaodnrm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2cpazxfln.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2msqlffug.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qvpovxms.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ofsjgfgf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skdhrqqw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kzrnhovg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2acaqbysi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ngceflbx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2geeykiov.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2gtsidpzr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2dbhconbu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jmmjvhap.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gljdhiyz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2vaygczvo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oownrqjk.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2xurxtzdj.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jrworawr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xtaiwcfc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vbgajijg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kjkbjfwr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dwezxcou.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xalskmar.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2wbcgkuhw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vnlhbsgi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qwpzmbnj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2naakpccg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2txnjczay.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2qvsynpbp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ihnyarri.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hboaqebg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ftupoogj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ncxptceg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vlfjbszy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fnymkswj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fsvbavaj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sskkspoy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2doeloaud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pqeunzca.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2agpddvnc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ptbpyltw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fyhbhiij.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2qgnwrzvk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xrxpgddo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tgwiwaru.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2npbtsqko.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tphdxskk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhtgpzlg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dilfnlgd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lzbekyer.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ceyezzou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nxivjiqt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zogdxjvb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xwqicqvu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jnisujmt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2klevkxrx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kfumskgd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bowjwgml.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zncqkaxj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tquhsvvm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2kruzwzna.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xihiqfre.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cgxlbtwg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2aoptwdjk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uacxetkw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hfimehuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhduqhba.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ddoavqon.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajllgvgo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hpddissr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jigxescj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sahyzkol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igfotdas.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fihgqfjs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rvewmyva.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mumduzia.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bkyfjgpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xkojgqvg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2obroorjh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mljizzme.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lnmhztke.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2eplzoxsr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2akufgzlp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2aemynkhk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ukalflcs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zuhfxykf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eisnuuml.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dvbbwwpc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vwhlvmcw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cxnzdcgp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vdacmdon.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zxgrylec.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cikmlihm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zqfhjfox.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oadftctb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bxcbbeax.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wnkpvvbl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gjcnvnwo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2obwdrfbs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hletcmjg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2akmjsdtd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jhpagddy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2idlmymhu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2cifjyapf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lkgkugts.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkxyfkfl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ascloqpy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oiaxuqeq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2twgondpw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rzqmlauw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2auyffpww.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gvkzhmuf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qblxoyuo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dthpydke.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bpwqrocp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dpkcrdnv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ybotjfpi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eqlwohrh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nzdwnpzf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2foshfcau.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dkwcqixe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wctofizd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2llnxewij.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lhkvvsqg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtymzai.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2zyaajpij.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gfbejtsh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2yjeowdqb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2xyzsmyzh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wobtxodo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jwjkqury.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hpnghvph.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mubymakr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2eranosnx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2yczporfe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kwynjxst.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2mrjfufxn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2odrgboyj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wglvxzfz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2fvxmawcj.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ftxjrsyt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztlliboo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2oufkxhii.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zectmpwz.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zqvzjume.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nklprycp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hlrseleh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ohlapjvf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sowmthrr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gwjympjx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2efwtljux.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxmnqrak.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cmflvhet.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2rxcgdwax.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2gevxuztj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eyglokuy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xwpoairw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qodfdhnd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ruicpgqw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kzjxfidw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2gmcnjejh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2fywydpyf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ouywmoid.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2btjtcujs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2yusnvsng.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2swiswpgz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mrvswotu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2apwsmzhp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mrhyetpf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fsctuqwc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hxxteygs.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2yubidkws.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2awyfzsfc.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2otcilyaq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atmjgecy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2efindhdf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2whzcqivs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pfohszqp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxtioyat.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2iyuyztcu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2byhzcspm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2cwxdbbwh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ntyljopc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vhrywobl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kuuxpbye.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wagwvgcn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eujgqldf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ujfwfuyk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2igrsdshf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ztcoxsmr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2lhfrjufe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rxwfvrzx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qinxzjtu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hlvlynzv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgawexl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2creexahu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vzlddekp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2xewekkwt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tvkpikdw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wmmzulcp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2csvybpoz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2blplfyxq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2swytcbch.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uyuashor.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2rdtrxoif.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2hptckrml.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hhblycwc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqmyuseu.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ynvzoglb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lrvorwsd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjpxvjw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bepkcupz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xiplldfh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2usvyward.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hoxkbglx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2staizmyl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qezzbsej.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ruizhywd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hikuruqz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jxaqqccv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vvbvtevf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2masiyztf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nwbiqqkz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aekydwkr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pczpmvnx.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dslvlsll.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hhyzqxrf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lwfybrpp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qfdttkpt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hubsijhl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2nynqwphk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vbwedmol.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2qycokldk.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ivguksis.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2srotbaqy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2usliyajs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pvvggzgz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hrxjfkks.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2urrgobtu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dsstyndj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2wpprlhhu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uhalrtfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2pvdyqzvx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ektcuish.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tqufcfaj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dxecunff.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lnxvpgwi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uwafyfhq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wndogiyu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2mydyxwxh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2slbpyrbg.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2pjucvofu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wgwspiid.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xqeiqasb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ynawapjs.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zsnhgjxb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnfkgsmo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvjediz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qwziuaya.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2thyltlnm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rwmctwgs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dtfctyvz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2jwqqqecg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xaugdche.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pewxtnol.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lcdwfvte.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bjtailwc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fziyvhpd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ofqwulkp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2brrxtyff.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2twfupojr.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2lwgbhvpx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tclfbbhs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2baziteln.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zzjxmqlw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzsyfxk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2aemevyko.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2izfyazkf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2gecnebiz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmaoxzyq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ziasntku.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dsbdiuhu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xftwhqyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lbduekag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xwhummlq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ojltyxdq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dyptomlo.html


<!-- 参考信息 -->