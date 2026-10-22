代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2eajajggz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrvssztg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mgjihfql.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2bzilmimq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2iyrudtde.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ktgopfte.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2nmtzjici.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2juoctshx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2yatwbxkx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uqjefysi.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2vdnbbwwk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rcndetaa.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xylykqzv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhvbnv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbugzmff.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nuegddeh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yfgofncs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2goeuuxpc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pjctpiuy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mtomynpf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rxvuplbh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dulsqipc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fydqlcau.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2fiwopggb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jmpaqwdy.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vryvqjha.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qhywysez.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mtzhucap.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2swdilbsg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jpwstqtx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vvhaxdfw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ulrrsrvy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2axesnbrl.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2molfqtmf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcowuqy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2zgasnval.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2granheng.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2aqobtavg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ivxbklmz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2werthkth.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xbiwrjsb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gbtmtpon.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2aoqqcevi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zvlbekln.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nghghjpr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2sqcxkzlj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jutslzpv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hihforrd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfosmiit.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cjwfatpl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjckouat.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2wlkhpuoj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ybzeyyan.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2felqhpyr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ejpnzomo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2pawayipa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2koojxxto.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cihodbpd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibyyeake.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jaejuvno.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2vibjigsm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bijrapwx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2onpkkbbi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2upftwdgh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bqfonzwb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zlnlvrgr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2egbyxpiv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2oltiiwmc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bswcsbyc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vxworbam.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2axqafboz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2sjzyldow.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2slqjpaph.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rralhnzr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bralqppp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dvixwldp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2dkncwaof.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xeajbyxd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2rpmqabmw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bphbpfhr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2knlhyuzk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lsckdopt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gnxaiwnz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2kthukucg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2mgchsuzo.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ibacwobz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ndkchkps.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2jwcxiihr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cbxkzxlm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dgjcuvwa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ephnonhf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjfflcsn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wifczfiu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xjernzwr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2qmsvphhw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2njoystsn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nrvoquio.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kaezrxna.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2caxcctoi.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hmdvuziw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqazpcih.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2iqfimhhl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2hasznzhv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gejdqili.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2adtgyupe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vrgjsgfq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qrefmemj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qycpiiej.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gwxqdief.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkwwsghf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2flpdqrms.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pbcqhbos.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2utvmmgzi.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2zywmvjke.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tiaqzpxx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2exgnqhaw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ftrpwrva.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2vgaxrvut.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eefvjuqe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdkgdlyc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ctrncgqb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vldpmkxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yytgpdaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shpoqluz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tchqwlzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgiqzdnu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jjlzxqyq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hzrbcvtw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qphdscmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2igvkzfxt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2aymetqdv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fswkipwb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2fabwmmrt.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zyivpdhl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2uqaahvut.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2epzokduv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bzxrqdrn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2uecgychx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ktohklue.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2weuxomxr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mzamzwjc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pidtviab.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ypbzqlsm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lrdpgeth.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ikjhcygu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dilwgqia.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nszrhufv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2umrchczd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2grufmdmh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yeaujqvp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ksnvvzii.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ispidpyw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fzczdpvb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xjzdijcy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmrpdtw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2zzprhycv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2igihnnzx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bvjrzotf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jhpizbtl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqyaort.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mbkqqvli.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ckneejwr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2tdmxwlar.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zquovycp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2htezwrkc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2syoyrpgc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xuovensj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2kvdxlpqx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tpixhxpr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jcbdpkhv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xjhdkuos.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hbxgwedj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mqbvfwki.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwjhjukd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufnsizhq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wxvoabpw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nftbxbat.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lrdptlzt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2acanmcez.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wucpbilw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wrolchfu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2oqxfgfgz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ultdkgcf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yyspctmr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tlxozcmz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pfhzebei.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2dxrmivvy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zdjgsxle.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tevmzmlo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2duphcqwc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdrtzhv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xagpazwa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hezmgdkl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2gdzhicsg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hcgokeau.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2eazpjazp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2otbpiywl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rsywjztn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2quvopvqd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hlolishx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jirjggfs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mbmrksdm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lnuogfkm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xvychcse.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bwxwqxwq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bcbbafzi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2joucakay.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tcyplilt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2blqmsrma.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojiznadu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2itlgvipn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2madkmrnt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2dzhcicro.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sgcmkyes.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2whotbmux.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nkvoqgug.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2umgfcsll.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nortfojv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ipyejnvl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ldoahopd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zzfhcorv.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zeofjpgf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dlpsfiod.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jcmttowf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jnpanobn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vbwdlqal.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2evjfheme.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pkqnfjvv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2euzhjwoh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nssocwml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2msmnglxi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zgjxdhtl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2krvdqbfx.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ebxpvmrj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gnwxfqyx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2josdhevu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mtykoutq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bcpwhfxn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iprjaqrw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fgucemzy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2ryqwyplj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2shljawvs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dchzkbxl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2vhqrteca.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dkmcrxms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vhjrhvch.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yrhqzwwh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dnpmngmg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2srwhrjnc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2pyuthjmy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jbpdmjtr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yefnnezw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lbertufs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aoxouipg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbjdzdsc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sidmyoym.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ofvtcpvt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2evtrynxu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2isjxogrc.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rfteoeen.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xelljmda.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2nsnjkziy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2norqittf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2degpygha.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tmflgofw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dnmqwmrj.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2xsjgscdd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vokzjkuv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kpeijumr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2katvglnk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jxdxlvru.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2piazmnnx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2sgrizcqu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bparvkit.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wcgjywjy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rgtbbmjy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrwwzyf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2smhgiuqn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kmzccahk.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wcqpulcp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2yzpdgeis.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ycertrap.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2aiztfxdx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ujiwmmtb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdifyvom.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hcsriusg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2dhyatbol.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kfzpsnbj.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2sczmetos.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2oyvmztfn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2wjredwhv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wrjekkki.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vzxvniuj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2xixwprjb.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qlkrkxvf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kpnxzyqa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2vzfffynp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2spyvdnoa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2biuwitkx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vhsioqaw.html


<!-- 参考信息 -->