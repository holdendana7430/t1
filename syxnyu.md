代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvraqsoj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tmudgwfn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nclvyptu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3pkpwsrur.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ynlmlmap.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nmmhraqw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3otkwskbv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yzvinfbj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3phkowufn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qezbfglx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3anlxhwtm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3igwogocg.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ndkkivnj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lkgqxguk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zhcytioq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3maxjxqli.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rmywczcm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3nfxdcbmd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xychxsvt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jjbqylwr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3duihwxlp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bitxcepu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3cfpiirzf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fayofsje.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3dhgzvvmq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xdhuobnc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ivdjtnps.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oibytwxm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yjarevra.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3htypwbgi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zizldbdi.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3owjaaewp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3azgzprlp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3nltyskow.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3rfrfmjzz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwwydabf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gxhitvca.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hzprouyc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3klufbpve.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mlcurkfn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3xxcpzzjk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lwhforpo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3cqrlketg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nirvdzwq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibokehwk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjjahghr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvxkywxs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3tcjrbswk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3lohfhrpl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3lpsnnnfb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3moxlivgu.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rxeuuwoq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mnrgytii.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vucgunic.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3nlhfcmri.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3amajvmib.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkefyxuu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3iclcsdno.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xldeafug.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3oxklugte.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3sfewhego.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3etyesiqc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3aczfuepp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qhexbftv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3agagwklu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3izeuybnm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wisveext.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zlvpokbp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nelkgjwn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3uhjyocli.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3iumgyobv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3sqtnzrxe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3avytheku.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3azlgyovk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hgovzzou.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dcbkakri.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3eujtbsbc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mvyvxylv.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nbqwtfmc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3eyathobk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eijsqtzl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mdyumaud.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vebcywzg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jtahvugu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ytardgkh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vkmylsud.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3prnzoews.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ujdnucah.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3unmgnuux.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tankcssv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3skmttkvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mzmhmgbp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmiiqsxk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wewygdbk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3znzdjnsb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qhmtrbss.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3dihrsmnd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zkguzhxv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3egldlsuj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zuypqyrr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfossxes.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zbbwmxuj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lfajgmri.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3spwhluwt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pwnuoffb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ueifjtwg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kgqfjmxp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ruphlzuy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3afszdxyc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bftnnank.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gztixlds.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gteaskqn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jovpsdln.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vptqrtln.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ggalaxjz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zczlrgfy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3takpjsti.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3avwqctug.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tmehnmli.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3froduzie.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rlnbbncs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3odhxkevh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nczwzfbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywezisjv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cqhnjxku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3codkkomw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zskmrsmi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3asmsloym.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aeystyat.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3matactth.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gxfntvty.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vnevzguf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zfwhwden.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xdaobxwi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wucxtlzx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3gezfqhev.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3gbcoxima.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ocgywowk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ifyggjmr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yhxzmkyn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3iyleweus.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tknnbycb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3liombgaa.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3tczhxdvd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xtpqvtgz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tbsvcqfa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mnwbjmgc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gmbhozqh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ppfikwud.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3twfwjfft.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3congbpya.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3gengvcii.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tunnpfuz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wharmyio.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cdoaebms.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aljnxoia.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zvulyzjk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ngesuoqp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fzflbfbr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kgqcutjz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3uepoylop.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3buwajuzk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wuqksglq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kwoetavl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3twqbbqet.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jpkfkqdj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vctvrxya.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dukxqsul.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bnirgbwm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hjqtggbu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cfhxukux.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3voorntwd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vltauwsl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3zrnbexjt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3khrofmgd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3iukenamu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zdglmtbg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahrvpkyh.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cuxbxkrj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wtoonlay.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pcfnclvj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hsfvhwmp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nzkkwbve.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bgoqqnel.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xzsmfqzj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pnxubnto.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wjlwjoih.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3abisppbi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jchuwifa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ivqnqitm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hexbogvp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3comwilqi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ozcfbhbz.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3dtdqrhtg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhbltour.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nflatjkl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ddevlswp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kfjsktux.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dhpxzpjv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hzvapegr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3nwpionwk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kfzzjkqv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wzywqrbp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3epnytvey.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zeticria.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aubsdnoc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hareaicg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nklidson.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rfgfbvuu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dltxadwf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cjqnbgac.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnpeocq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gboucaut.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3cqjhndyz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nokfcybs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3azwjcycz.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3terqatuf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3eereimjw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kcmdysna.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yhdaovwl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hwhlhdya.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3teluugcv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxxjcdue.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vmymvprq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fbsgszkx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fmzaqqja.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3awgamslo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dknjpgpn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jthpvlmt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tylluqyv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3zhczlehi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3olpduvym.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3caoohsmr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uuehanhq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3avlswgay.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3duzxtlzu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3xjdgxdnb.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwndnrz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3duiwwicr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcvtlwmr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3tniilkwn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3olrknhsh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cthlzpkp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3vjlblpww.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3nzrzdtzt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wsfwynmc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vkuqjvow.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wnycwxwe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3pskctsge.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nsafatmi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kccthrhc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uzzeyqnt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ayfscads.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kdkyeihf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zauxgtys.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3suaoaobg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3owshbruj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3gtfodxyg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sjuzbuip.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dxclafys.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gjmpdgyi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3sobdkkhn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wryjttth.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tvvdzgqh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pzjtqpso.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3szbuavlo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3errymxrj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vbrlynwo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3egyumnfn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3shoivlij.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xzelezdw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqhisoo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcghpiwb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3myuoxmcu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vuakmtqz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lbnvjgui.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxkqmdjv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wlbfzvbl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3cybdklky.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wsieisir.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3scsvgseo.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3sdztxhvq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3upobyvjf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gfqzjdzi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qdlahnqs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dcwnkcqe.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iirfjkuu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ivxekkyy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3nmtnvitx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bulembie.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3oxsyuluh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3makutugh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xuptcsvt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tzargnfg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ztgskkuq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3jsdtshut.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3qiypcqxm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3iyysswpv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yblptcnw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3llxqwiqx.html


<!-- 参考信息 -->