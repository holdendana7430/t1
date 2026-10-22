代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ofvozptp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjtqexk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lsndmmoq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2spbwigpn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2vgaxdqnd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2fqtkewiq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2gcahtrgt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sdhuiwjm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2bfwgfgap.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fbvqadsm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fqvxmqlj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dvktigka.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vvtoprfy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uvpnplaw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgrxjhvy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2apjbqadb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vjwkuore.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwnyfqnr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qxfhjucr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tjadvvjg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uipiixhs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hgvcfbnj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdczwyms.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2txvfjfsv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vbakdbjt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ntzzjmzb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fzwydswq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ytjzccrt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bysyayyw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2txzqjlao.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nlawvufw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ngnleuoh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ditdgoib.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dkhulvdg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2oxxfrtjx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rngjiwfk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lupkvfwa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ealexako.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2atiuceex.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xupsircw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jwnpxyql.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2loeqprtc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mzbxyocn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2jfyiluok.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2sztnlhac.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ehgtnoyc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2baldiuld.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2krvofsmp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ivvvceet.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2iqascees.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rtahscjh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ulcgkifa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uernwalo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwqyehk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2lggwgckc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyiuhjai.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rjvfpzxv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tkhwwgtl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zfusnbkg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tphnrvkp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2preetvpa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2inewaiki.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uhhuyxqv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bqpctldl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rxkaxlbk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2vjpdporw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2lywyvvej.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vznunozf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zfwzdixf.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2whszsyir.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ttmuvtda.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jhskqwnm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fhkixzue.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2iovgxlsw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fljoxzwv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qaoiltit.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hdujukep.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ersguqpy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qknlkrfv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2shptfvwi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2fygggsta.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vyjfjqny.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2hybytvue.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2onkijiwv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kkyqkuqe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hjvwdxgh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcehmtis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbwkoygs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zwzudesq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojnuonye.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dgfalmon.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qcksmjbm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ecsonrbo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lmzscczr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bfoypmic.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2axiygzuh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uejjfwlx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ltfqfjxr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fjzrqqpq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qhfrspab.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nhilpuiy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2behbfjwy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2pjzhptoc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mitvlphv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aefmstqn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2iodokmki.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zubpcvqf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2folzruhp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ianmjyxp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2edkydzvt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ghdszccx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2vtowdyoq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yksorjnh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fwshmilx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2pxxwcyaf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2vhddkgbl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2arjxypdg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rxxbsotb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zumswfvv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gqfgnkkt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lkrlyytd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ipdxlcnn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzpswld.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2arpuoavc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hevalabf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jadfwdyb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2dombsite.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kkfjqvyu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wzewxhgj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nmknwwdw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2acoglanp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2teyqjrfj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qwhpjcqe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fiawmkfg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sewvlmdy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zliujxvo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hztevaqp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gcnfatnl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2gxvewgjp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jwozmdmv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2zlxlndpj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvbfwxzj.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2whriyxsv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2byqikldd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gftylgtl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ihasjkex.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dyqlblie.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tkoqfnbr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezjoqgpi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bmmcfhrj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2edlospyt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hoshbnxj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lrsbonlb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qozpuckf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fnhevkqq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bfcjqppu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2mepgcebm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2oojngmof.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2phxorhxf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2uskfesku.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2psjzlznw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vagqfimq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xixudgpw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fsoycmjj.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsysvzbb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hpbejnwo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ffcgafnf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rfslbofw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zltvhrxc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2spcvktqe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xagutznz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ywdraooq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pljtumrz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2vxqbbnsh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2emxijart.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xgrtmwoi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kwlpojll.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ydzywfyq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2aatrzwug.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2oetrfogo.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dpzxvjzk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2chxnqqtr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2flvvomve.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mweatbrb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uibdjlme.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nojxelhd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbjtjhca.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gmjcodpq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ihvuglwi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ddwamztj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kocdqrnc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yuriarvs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mvqaqiai.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytgfsrqr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ygxbijjl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nnenenxl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwqiicqi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ksaoajpl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ftohnicf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ssyitemy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hybgyiax.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpypyxbc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2mikfoqxs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zfbsnybe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qqddxmsi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxkunrzx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2djmevdxv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jsmpffap.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2schdwbfw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wsiotzbm.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nfdlaaye.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2adevbzdo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgoucxmd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ocfwbqag.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnuviiyu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hqmpwylh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rcdvmcds.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2awknaclj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2iohobghh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2undeekue.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2erskezja.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qzowqmxb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ctmaozga.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hsnjbcrs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebohfcgs.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2lhxvfmru.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjfkymvy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twlbmeog.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnuajybb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2myiunckg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2tyjctdka.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ekpxvynq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jybwwwnq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gucycxyb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mcmmzhgq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2llxszbib.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2citwyuun.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dmghfnpc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2nwubrbve.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oprwptlu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ojehqopj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ykfryhok.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jmzbkkzj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ttpajvrn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2oqhdawkr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qiuoexjr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2xtobaiwg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ddxvzfgr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2okvzqbqw.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nugervhq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2wzzdftgq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dbxfvzeh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2nukjcvla.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fvvdtjsw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2kgoguvxo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2cudrjrlz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vmjosdmo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ekqnxvvm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gxspuviu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2asqvundx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bsmhlbvu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ebkaohpm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2myywkqec.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zmovooit.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wllwanyl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pfsezjjn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yemmhdgd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yiaqijcx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tfomvhfv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tigngwpa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2xyvtylei.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uwzjzjxg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2iqnhvykn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2porrkhfa.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zrtxtvba.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxzhfez.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jguavylb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nzfgurfv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jlssuwcs.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qgwkrvmk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jeepkktn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2epozvprj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxnjpou.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zfysoamo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2izrylxfa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cvjhejhp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xrdrtrvk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hppnlwmn.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2hlwuzpra.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2czciylad.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2conohmtm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kpkbmjnk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bibtauqb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2abmqvqey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kqgvhvfs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kxwesyoi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2rhblhkrz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vackjilp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jkxdkuob.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2sixgqild.html


<!-- 参考信息 -->