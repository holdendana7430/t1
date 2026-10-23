代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3bcuphcgx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vpinoxwn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcoauxar.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pknqhldt.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yxijtole.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3uzrrapdk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vjskcmrc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3eekkxdli.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpjxxvkr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uhhkqzlr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxltnkhm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xgegkblv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zxmqzgpf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nirqqqee.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3isdtdtcm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3wsjppjju.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtqrlolb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhavtavd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ibjixjcg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3epvfqawr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozbautyw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3igffxviz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dgbpilta.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gisjalzw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rdlgnlgg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3drewvrfy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nnpzjqob.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uiamnxxf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3iwultpvh.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wetftfdt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rgnpeldt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xzroizaq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ibzusyrx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3guoypytb.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3raguldvj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nczsitxd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ycvzgvlr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ckvkklss.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tjnpmipj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3qjmjhjbv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3rvoyyyfd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jnrrdqym.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3kejveyes.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dytiixgs.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3narlejwn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gfcfdewu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iuacnmjs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3xmxuxvdz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3cgcbaufj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3mcdmtirn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtyezsml.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nkoqkhom.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ugbauljy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvnuoiwn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ktmlfgju.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bizbdmtx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vupiwrux.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dmlfgxjn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fyduyvqh.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cqwwldrv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3yeuuejny.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fggnftyk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3btbaetph.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hrumkxgi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmlnmbnv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ephrshox.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3veoanken.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3esplzofn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vvnqxrbf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewjkkcqd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hkkirktx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zkrljhwe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vhbpickw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jpajmezn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ezfasihm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kazkclur.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fsdfrprf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mqticdim.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3lkkggukv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wpwdaenr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3acdasjwa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3gitccokf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hbscefxf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvfoxylm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tlpnsndz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dnwkhzrw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qihdeodm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wecktwnf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3cylispqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzcagijm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fjkbhjqc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jipvqdpc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vybixcrm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eedeqhus.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3nchzboep.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kledgyws.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3bkbxpora.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yvqueglc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3qlvtllfm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eyyahgzs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3blsthegq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ovmexzal.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3aaayousc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nblvtaah.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abaarysp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nbmvuifx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmcznnf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbyypgpg.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kwdrtmpc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bdpeiqsg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vobfzwiu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3affmhwrf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3djescrgg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qswqrexv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ointpmah.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvolytg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xfjdbumh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nuyyivht.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rfgcmbwx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afviaqwo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3rgvsiqqh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ljjnmnrj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hfrdnktm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tbdbbewh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3biidczmm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ofuydvbg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3irnqufyp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bvvdrofy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nuziielz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jbgxrhbr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3lfscowml.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3sgtzlyop.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fxyifkiy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lyagjzhl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3tbuwlzph.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3submwwab.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3niohlrid.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3sakelfrg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzgcsyqd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xtdwpcno.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ohgxioev.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qngstskr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3sdlrcjwx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gttjjyqx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3qdrjqdzs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3lymozyou.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kfyefdoh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uexkezyy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ooyhvkxg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vhimndje.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yhajfsgd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zufylpnu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mllornap.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zukaicqq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3zqbrzsyj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uvylrpis.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dvszuosq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3oytbzerm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3evuedbaf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3jwnmbamn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pwnjqfya.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqyrvivy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yewioeip.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3phzonewc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bhqlboxi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ovnqqass.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gmqkofhk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tzwsfyuc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3csmgiktr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xxzoqpul.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eaxjqpxw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3tyuunbsv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3foqjldtu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bfpzyijp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nmuhocwg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vmptcklh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qsqxtebs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3sbgocvvf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ojwfnjiv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xoyvcsyi.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3mzekerhi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3gomklgig.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjweffxl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wjqohldl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wkymprpg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3kxslbali.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ccdljeqx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pnoshbbq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3rbpvyrmo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cuezmixp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kuzotbhh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkctexus.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3apbcksvn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ubfoxkvu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3wxunarpl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mfaphdxd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfzjlgvd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pilkclzt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3qwlvzels.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ydkyhyxi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mdcycuzp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzdlufgv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wqpmrjjb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qwgyefvh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ihedaizp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fkroqtsz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlxmcuuy.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pbywmwrr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dshwnako.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ihfwmvik.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uhrjtsoj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayazadly.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwhpuhym.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bneqzdaq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kfhpskkt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pfkrsonk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ablvbapk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ohtogehk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bntwjtwu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yhxsleup.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ugxpkwcc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sujfbchp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vbpduudo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nfljeitg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qixmzcom.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mpmoxdco.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpqpjbiy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymioklps.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxqgzkez.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ifmbxgyo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pnvulwth.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ozzkycvh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3mklqedty.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3yasbdssy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jgaxhedw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rljjdhpf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3agyelsop.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3awbnywfh.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3utuepztl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dralkgoh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufmsnkuy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mjlumqaq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3skeccrac.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3evhsuncp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3isvxxvqb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3hwmpaotg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3etutkgqq.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ajgitxqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xtkogjek.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3tcqpnofi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3epfxswmi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvqhzoji.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sokynmvi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fjxjbvmk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3epexqbib.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zdjaainl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ekwkxkvj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3anspyopl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cqjfwool.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fbvvlhuo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fiojthxs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xblyfjxi.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgihknxc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkjmqawp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vvyosjax.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3easjfrso.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3elbqiyld.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pacaizbk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gcodojxm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vyqdpuiz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kttmhqke.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3mmzyjxcd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3feulfusz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hqjnmyod.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cogkpmef.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kquhrjpe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vfzolomg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grfkzmnq.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hmvrjlcj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ozvvlrwu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gcujehvl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3cocobjqv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3icasvkgr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3kbyiwewi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cjsnmtsv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wgcibrla.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3lhxwsweo.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ulvmmdhu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3shkyzeum.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zlltafmk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3visajwbh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qtvhhzig.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3waladexj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zwazxakx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3huvnpjlt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nogbrabr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3duidkwje.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3drqpqtbe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jtrlfwls.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3iamwnkih.html


<!-- 参考信息 -->