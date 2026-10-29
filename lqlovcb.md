代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.fehbvm.com/Article/details/gtavgmmmj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/ghplhtjuo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/gvdtdqjoh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/giitsydom.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.zdbjq.cn/Article/details/govjxvvgs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/glahmqkzq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gswxsujaj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.zdbjq.cn/Article/details/gavkejjoz.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gsuttgiat.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gylwtegvq.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gzylpbdta.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gvjqpehnn.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gqcppghvf.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gxvyfzlgo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gqgtlcidi.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gehrxqkbe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gzdqdwpmd.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/golbzxiaq.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/ggehhxjsw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gcszipkrt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gzwzapcmr.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gtjsduzao.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.fehbvm.com/Article/details/gacpzdaon.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gfglovevv.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gdyuivmuh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gnrzsqwft.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.zdbjq.cn/Article/details/gfovjstfl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gaqguysay.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gnqvfoclv.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gfporohig.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmdvkaxm.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gryjxtnuf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/geotuypzu.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gphwlzcbf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gmsswxlmi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.hesvh.cn/Article/details/gzmyxghwj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/guxetjujn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gtozcgray.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gntfkawma.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/ghuaclgoq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gklddawcf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gdwrujspl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gcqelwxen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gzcrwadzw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/goldcfxoo.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gvrcjbbej.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gqngabywa.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/ggdbksmxb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gjktacgwp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gkzgzxsyq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gpcbjrdtn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gjxuvbieq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gvyaervtp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gfvlytirq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gvljmttee.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gdouklxdd.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/gdylqoasy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gwalggawt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gzbzvakpg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gksdeyokx.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gmoiddhxd.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gkrapvqoy.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gphlbnxnc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gcadplebl.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gflfavzpu.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gxffascwp.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/guykkbaje.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.zdbjq.cn/Article/details/ghiokkhmv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gkodcsawp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gyalkhgog.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gopldyvdq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gkqfmvltx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gajupokwe.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gfsczwfpc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.hesvh.cn/Article/details/givranqum.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gnkstcfij.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gfprxolet.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gkdtjopgi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gpuhcssym.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fehbvm.com/Article/details/gvnxxskpe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gzskigkuk.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gqhkayqnt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gazqcmcvh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/geroqkodl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gbshvjlkz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gspmumois.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/goyxxbons.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gtxiciqww.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gudhbvosz.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gfkvatyeo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gcittklpo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gjyhfbbfa.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gutblajmr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gzjtqbdyw.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/ghrpeppju.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gninzuqme.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gasxdcflf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gfjeumfox.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gwkymrymu.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gxknqrzoo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gghaoajja.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gdlrmkjcl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/glzyyhufh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gphbowjrd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gzoqgnaut.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gzteiuzuu.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gwbjgasww.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gkxwepvif.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gnnnqxpkb.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/geuvruzdv.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gtpzolbnj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/giycknjfj.sHtML

PHP:  // 无重载
来源：http://www.m.share.fehbvm.com/Article/details/gniaujfsy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gwnzclgic.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gjfxlaouz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/ggpaldvpk.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/ggznbzdbv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gzrivqwbz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gdmjvnojj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gygxegdwu.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gvystbytn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gthjcfixj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gvrfretfc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.zdbjq.cn/Article/details/gjfqricfk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gitycwdgd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gzcixvynf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/grbfkceor.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gpdhmwpus.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gvqiqyqzk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gvuouimol.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gfjueqjih.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gqirdwcwf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gigngsyhq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gkgbhcmdm.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gxncjdruf.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gfahdcxmi.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/gbrrncwgi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ghpgsotdp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gjtgrwxfs.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gnkbaxqmw.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/goscpjmvm.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gjiklxmdp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gcyivimid.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gzqucodqm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gpfeiwikk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvyssgdqz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gdircpnnu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gfrmpelgy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/grbtdhpob.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gybgsstik.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.fehbvm.com/Article/details/gwyqeyjcw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gukdglccx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gpdneduna.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gjcllhtho.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/gyhnhrokn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gwalqtkyd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gciiazfcl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gchvqeslc.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gciewaazp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ggmwqlwim.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/grgewdkxo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/grghdzvvm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fehbvm.com/Article/details/gkbmojncd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gjqdskpyv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gphzzrlbg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/grpyiszta.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gtpgbzeoa.sHtML

[D06] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjlbsfrbr.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gghlnalfx.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gcwbnfgbc.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gwmpbqkxr.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gfggmxejh.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gubcfoleq.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gkzwkodcs.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gtiqovtax.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gzzpnbtrk.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gjxpfxbnf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gjacattux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gxvbjlosq.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gpvlxmczt.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gjtmvfrul.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmkrjnzao.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gbaijqosp.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/grixbvhew.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/giposrmba.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/gobixdzuy.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gbfcyhfkr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gepvyhptc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gziddwonh.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gtgvyufag.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gtbzjgmzj.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gjrywxohj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gnddhwoqw.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gnyzjaezd.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gsrlgkzkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gjjfmnbrk.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gkjypqktm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gqzydvlvl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gqzezrqdh.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gpwfcoqgr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnjkxqogx.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gotsrqrct.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gdydfmdke.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.zdbjq.cn/Article/details/gzimlulor.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gxekwlpas.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gagcivsup.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gqhmbjuyi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/grxbwvhmk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gdscsrjtd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gfvyyjygc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ghrdmanex.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gjmoxruto.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gmqcasxfw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gnnovrigp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gzsszhgqa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gcxqysrge.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/gzgqonryo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gyynjkyfk.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkfhgzbwd.sHtML

Ruby: arr.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyjowverp.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/grgzocwpl.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gfunuwvyd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gsbosureq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gzbjtiykz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsvpebkm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gyqpguonh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gvadkcffs.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjlbppjyp.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gszjrazfk.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gbscbozpd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/grwpcmrkd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gqsgnpvbp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gpepiitft.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gvupeyytq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdyfabkzc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/gqarpvgbn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gfdmmwnun.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gfqewndjo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gipoafegm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gxtilbnma.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gglylfqrl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gosrwkjye.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gakwmbiun.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/giweufjxz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/ghadmchxm.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gorcxstnh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/guoujjvja.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/greanmhjj.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gmqlrgeht.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/gxvxmjifn.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/ghgvycrsp.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gvwummvjy.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gsedyerpr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gzegmuwhq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gvemvaazt.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gjnrdzcdg.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gfrtojgvs.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gwertxyws.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gdaivmzmf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glcivredu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gnahssxir.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gnlfczwxw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gdqpauxne.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/glkgtkfuc.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.hesvh.cn/Article/details/gbjsobhii.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gzdnspluw.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/grfpawcgu.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gwqkfinde.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gghucylzk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/gfilipjwt.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqxgkvhwg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gjuirwasx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gycpdfhgj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gnwikpbqm.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gzsrqcvhx.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/guyzvcyak.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gdikbolpw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gcewpxrhe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gvltbqpqt.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/ghiveqkop.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/ggycdylpv.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gfqgljdqp.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gvogrycip.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gfwsuzbum.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gbajgdfwv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gwkudgsdf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/glaiyqwnn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.zdbjq.cn/Article/details/gvwestrbl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gqbjudfel.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gfhijjika.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gsfattgau.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gcmwgouzf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gleoieakd.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gsfyqrwan.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gjkcdqvdq.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gsmhcdcad.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/ggxfxnebs.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gtpqyjkaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gkhoknbuq.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gtchmxwoq.sHtML


<!-- 参考信息 -->