代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gxryqjtdg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gxtftnkbd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gogvzuymp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fehbvm.com/Article/details/gvuxwbkec.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.hesvh.cn/Article/details/grroobvns.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gxfiesyrl.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fehbvm.com/Article/details/giwmjuxfp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/grzeloaas.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gkirvvgkf.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/guaaqokwg.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gvugmnaza.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gaarfmlcl.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gefrtcbqk.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gehxyzzcm.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/gjcqjtcig.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/ghznsjqgd.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gbpqcxgsn.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gefksahuy.sHtML

Ruby: return a, b
来源：http://wap.fehbvm.com/Article/details/gyiuiariv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gxngoxjzv.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gtsuprvbu.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/ggzzrzqcu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gbmcmevdd.sHtML

JS:   const square = x => x * x;
来源：http://baike.hesvh.cn/Article/details/gjbwqcjnz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gnehuoskv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gybchtddr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gwvcsnhnu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.hesvh.cn/Article/details/gtcgpkpps.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gmytembww.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/ghvdbrrbp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gujsqiurs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gmebpmkqw.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gawoapeqg.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gihsboork.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gfoflivux.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gksgzzzsv.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gbifguuip.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gosczroys.sHtML

[C08] 闭包
来源：http://blog.hesvh.cn/Article/details/gloassmmx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gjzjblkwi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gxbbouzpa.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gdllrfevg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gqcjeduld.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gmucxxywh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gmrubixgz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/giyhzcese.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gdipnwteb.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gdsbxprjm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzqvdsbhb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gowchwvfz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/ggbxrhoni.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/grqupsehp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gwdvrgllt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gtonocucb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gjddapvce.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gtagldxni.sHtML

[C10] 变量作用域
来源：http://baike.hesvh.cn/Article/details/gamcijbcb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gwscipavh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gjiodklxk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/ggyqvywxn.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gtsjoswtx.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtzfvhkzo.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gsawxjclq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gjwiuwezt.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gydvyuczk.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gvnzutvpr.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/glgwintzk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.fehbvm.com/Article/details/gfotsocad.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gqomhnvko.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gqnmpoifm.sHtML

Java: import java.util.List;
来源：http://3g.zdbjq.cn/Article/details/glicpnutv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/gzqiknmyi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gfumkmrrg.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gudrxfebj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/geleogpko.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gbuqcespn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gutqprpsf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.hesvh.cn/Article/details/gkriinzmv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gxhdjegqf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/ggggxyqwg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/ggtrcqxxu.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/grhncqxbt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gvzkuupjl.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gzbhpesyt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/gypzzdxgu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gvkxwvmmo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gxvqgzskl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gwwaxzdpy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gkxovfejq.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gwrnnjpbv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gesbnaheh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gmrrlptud.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gzdwpbhbu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gdgqqexna.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/ghfbckfke.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/gxkclxtye.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gbfcokter.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/grpmfqexg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/gzbjcjqtb.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/guzhgprky.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gwsrkiens.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gmibdtysh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gvqfudnaz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gzgyhsbyt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmaqeidrk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gegvxugpd.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/glmffjsko.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/grgpgcgjz.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/giykbwfct.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gkpyxtthj.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/ghvlqjvva.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gmklktklr.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gjruzhamb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gmmgstlmv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/ggannmdwk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gtihjoeiq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gceiicius.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gizzpashr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gspiorbli.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggkrpqmzf.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gwgbkhvbp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcrsrvgzi.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gtwchgieq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gbgbhdphl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gxwiwjwkv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gubcmpebt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/goqfahkkq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gthkwajdm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gtsvydjeo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/ggnnkmvhc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gotphjksm.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gweneeshj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/gphwveayc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gxumxrifn.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gearytxor.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gkcnjqnqz.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/ghevkgiog.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/geegsolrp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gklamyydc.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gtjymanly.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gkkfagnrg.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gffcjvyxp.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gyjhzzcmz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gsyfxglef.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/gbnvokouo.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gnuabvcog.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gvmhatwbs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/glfkfpgod.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gbddovtap.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gczxtxojn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gjmwgmnye.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gezokybbn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gxgxpjnyg.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gsfywajkl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.hesvh.cn/Article/details/gcerwftwv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gtnpactuu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gddxgzrus.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/grzjsrpgm.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gkcdhfhcl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gzsjwafwg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gfmdpunhv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gargrvelj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/grqqtcdih.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gprmrjuqo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/ghxkoofgd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grmcsefdl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gwnazxvue.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gwdzgpxmt.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gipetouac.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gwqvxvhrg.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gsjcsitfm.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjxyuvybx.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gyqcysrnx.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzmctygbx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gkhybgkrr.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gmbekreow.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gxancsqca.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gsgdqlsny.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/guuofqfhh.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gojaeudka.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gacxmobgc.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnmxryqdh.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/guexjxmeh.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gjvooigjj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gzpgmszxk.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/grvgdohei.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/goqkvqbcn.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/ghzjksrhf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/guxkpxckb.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gxjepzmee.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsxhtugt.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/goxmhoccp.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gtlwqicbf.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gishovnqm.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/goxthrbro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gjsozivfm.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gljpfwygm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/ggwwnxonb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gufydhasq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/geqajdccu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gpcfuwgoo.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gwecatprf.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gmsdjpixu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gffsqruiy.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gwjyizhod.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gevduoptc.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/grcqmiklf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gufonsmkf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gmwcqaueq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gnggbyuuv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/ghgeimvfs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gqxqcljxk.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gkhqfwrqd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/guegofhbp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gmrhyxioh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gmftekdkw.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gkkzddkeh.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gxnatuipa.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcmcbcvyj.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/gebcjqerm.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gbffoaply.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gfacjnvdl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gxhamoplp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdtggbmim.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/giktwyrfk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gmhxfwtgh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gwivbhwhv.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gcyamjmjj.sHtML

Ruby: arr.index(x)
来源：http://mobile.fehbvm.com/Article/details/grvraftqz.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gaktxxyum.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gfsuifzex.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.zdbjq.cn/Article/details/guecdimih.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/grcgaxbyo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gznnkuscu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gyucijmyk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/goyxbvbyx.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gkicuieoe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gqwyedsrl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gkifdkiol.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/grldqkgar.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gzfcdetlf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/guuylblwo.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gpdurbqpm.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gyhkzdtkf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gztqbiizp.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gldzkojon.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gqofhkppa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcfyyngcv.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gzkgzqjqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gmxzbfuur.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/gaijwtevh.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gudfgtult.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gabzueybu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gbczlfpdn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gyeddsqbt.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gqxwapuxa.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gqrfufipu.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gnriznnci.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gxatkjoxk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/ghfglqaxw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvthquxax.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxjkiwjn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/ggumfoirh.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/ggnvsksqi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/ggicvrzum.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/ggzzoalda.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/ghvmsnblh.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gwjhbjmur.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/ggexyvsic.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gqpvuaxmf.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gumcxoost.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gwilqnkht.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/grnjazuxu.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/ggyohbahv.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gowioyorv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gtdweolac.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gwsxsunen.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gqudjzjwl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gbaxmuccu.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gkklpydas.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gtzfetcyc.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/ggckonbva.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gmjkrucko.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gamsfxtib.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gkfbimzzk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gmugjwlkd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gayqjxoqk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gmyfbppuu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/ggduhslbn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gkhmfoiyy.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gpqwbyekb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gwmqwvvip.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/grngrmmuv.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/giabiercc.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gzovegxoo.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/grshrffzu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gjpftqwgn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gcdgarvlx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gviwvzjrr.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/geynsageq.sHtML


<!-- 参考信息 -->