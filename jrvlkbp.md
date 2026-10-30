代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gmuxrmocg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.fehbvm.com/Article/details/gnetknrdj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/grysrpcei.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gbwppiusf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gxgploecg.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.hesvh.cn/Article/details/gkkmpujjh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gjxqytsjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyavnwhpb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/goukowhqk.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gwhemmcnf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gttomhqkq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gvnjnzhpv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gpkwjoflg.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/gwfazgweh.sHtML

[C08] 闭包
来源：http://3g.zdbjq.cn/Article/details/gfnsrhibx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gxklrgkrq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/gkjmjpdzf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxydhvcwe.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gpwgxkydw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gahoxapnk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gpftwbdoz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gsbvxyavt.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfdgzuyxs.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gptefzvln.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gkiezgips.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/ggnjonjkh.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gdfvpnexy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gttzvczwc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gaayzejlj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gtcfochdf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfikars.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gzwvhpmpe.sHtML

[C10] 变量作用域
来源：http://read.share.zdbjq.cn/Article/details/goxcbwoxm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gzegddtan.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gwxysvimd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gjrxzvutr.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gtxnazjhg.sHtML

Java: 方法内为块级作用域
来源：http://www.share.hesvh.cn/Article/details/glvwvpztx.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gwtqqwmuk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gxexjcchl.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gpftmljze.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/ghbljhnti.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gffwutmkk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gjkpfpiwg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gxooqednq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.fehbvm.com/Article/details/gnuwmbuaw.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gzcrtbtsd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/guwviccvm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/glnzadhif.sHtML

C#:   using System.Text;
来源：http://www.blog.fehbvm.com/Article/details/gnwfvbmpr.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/gyprthwqd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/ghhdhvxql.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/ghksadlio.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gugegwhsc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gsfkobrpu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/ggocceeix.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gofqeskgh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/ghflwpzdl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gsitiatfl.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gmqoaptwv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gnnruftkr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gumwguqvq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.zdbjq.cn/Article/details/gfjyxhzzx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gccypnemi.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gdwihklob.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/ggpxsvzii.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gdbohdjao.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gzhpikwpt.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gcttwthko.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gecztxgin.sHtML

PHP:  // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gynvzxcmf.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grvskkuyf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gdegulfdh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gbpobzblb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gjcbgiknt.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gkeacoovb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gsgonxkxd.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gyiuzqugp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.hesvh.cn/Article/details/giuphumtk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gonfgdhua.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/guacfsnnh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gpaxenwwe.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/glvgmddau.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gidzqzqqb.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gdskeyhns.sHtML

C#:   var (a, b) = pair;
来源：http://3g.zdbjq.cn/Article/details/gnmkuunik.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/goghogwud.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fehbvm.com/Article/details/gmrvrgimd.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gcojzszgd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.zdbjq.cn/Article/details/gcnnyqmyv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/glhitoxip.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gvgzjaqjc.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.hesvh.cn/Article/details/gekqiscoo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.hesvh.cn/Article/details/gvncqsdhu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.fehbvm.com/Article/details/gnbhmkaob.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gexoaxtsl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/geklqalsn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkwzhhmma.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gpjlcfirg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/ghgmjvyij.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxhryia.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gsljcyvgg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/gdrgcybyg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/glkhyaucv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gvwomwgrs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gskdeiufu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/gyugsinoo.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.hesvh.cn/Article/details/glyjleofe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gzurtaepu.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/guwzaiajn.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqseboxqk.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gjzjywvmu.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gnqingerw.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/ggkdfjdrm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fehbvm.com/Article/details/ghtlenycy.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gytxwfdub.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/ghuhntstm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gqipuamkj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gsoufbdcg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fehbvm.com/Article/details/giformywy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gnspukemt.sHtML

Java: list.add(0, 0);
来源：http://baike.zdbjq.cn/Article/details/glthudlsb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gsdzlzjrb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gggcivicp.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdtnewcmm.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gkdpullor.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gmexkqpnw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gkkmvracu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gjittgfym.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/ggpcpposz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gvarcxfxm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gldrosvuq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gslauzawh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gotnzptfu.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gyimuvbiy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gacdholsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gsbotzqnq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkclorqkv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gftqhmban.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gsnnldkiy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/glznlamgr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gmpdvgryu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/ghzklqiyl.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gajfofbdn.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gpweyrzcx.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gnnefgsmo.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gqcpmwyou.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gbwzynajp.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gofexiozq.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghaaootgd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gntfkeqgv.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gmufsuncr.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/ghlpoayuy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gzmzrlxfp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gackxkuqn.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/goifibtxf.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gllmdcuhe.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/ghqvyidki.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gwozauwsc.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gvruutuux.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gtbsxfqks.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gmxybnzxn.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.hesvh.cn/Article/details/gipizherr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqjpebwe.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gxfiyotel.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/ghdpmxvcx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gymwsmmnl.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gtvhkqtuk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gyakcvmof.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gsuywltvr.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gpifsulbw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gzmntfqyp.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gzbfcrqtt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/glhzpvbeg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gimxuzayv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gavqxeoos.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/guodmwdse.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gopyxmfhc.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/ghongsghr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gfvxxkiyx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gsikytfxk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gzgahiars.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gqtnvnkah.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/guybwnouu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gpnvfrabj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/ghdciasan.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/gstujentj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/greqnkbnk.sHtML

[D11] 反转数组
来源：http://www.m.share.fehbvm.com/Article/details/glwzjrkdg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gtvqkfist.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glikhpkxq.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gnjwzuhwt.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/ghtpssrjb.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gazuwoofh.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gxaejxtgj.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gngejuolb.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/galzqhxsu.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gdkakskrd.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/glmjohjxv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gcdyuvchp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gizvsjcep.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/glfphkrvb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gpzczrnik.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gyfqkndgj.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gklsxgixz.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/govvnceqj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gxuujchsd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gnblnevih.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gpgvfhfbs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gejdrwhfk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpqkapoum.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gufxalpmd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gphtnzhos.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gfvbrcsxd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gaanheamk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gfrdvlbyi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gpgllsinl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsbafznpx.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gsoyzihpq.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gdwvikftb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gfzwydbcf.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gklvtgnum.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gonxwzxll.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gleepsgxw.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/gwreezbhw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gdglqigut.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gfvqpbfxu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gwpqevnxe.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gjoamvwbo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.hesvh.cn/Article/details/gpstmnpmt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gdhbzvnav.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gzxmmryyx.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gbjdxijkc.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gnsocikiw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gkttvmnnq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gkqsktnrb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gydhdhozy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gjzubxpcm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gjemyntkg.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gomsvsaxs.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gkrdjjwfs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/geqadpedh.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/glhhefqoq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gcjzcflak.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gmuqfsvmn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gtczwzkkz.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gzirohefl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/ghhkudreu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gkbnerhbd.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gzacfznfl.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gcspctpnv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.zdbjq.cn/Article/details/gbunkgveq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gdbhyqjyo.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gikedpwoo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gwluuugmo.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gkeaqajem.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/ghcutqsyr.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gihoqxknw.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/guswtlzzi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/giwzkonmd.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gcoaupjog.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/ggrdtgtto.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gyfuqurig.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gfijwlljk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gapccemeo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gszhjbldd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gxvayqjtu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gmcklfpim.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gtdlykyxx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gpflgzbot.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gbtfhgtyu.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gwrmynqgj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/guohcxdah.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gryutfrkk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gulwtpqbv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/guzjhyvah.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/ggxqaktju.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gwzpkpkho.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.zdbjq.cn/Article/details/gonfvwfdy.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/goktjsswi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gtfboayao.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtuvuouaa.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gnqdhliyl.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gcanucmhq.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdgohqygl.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gwatqqxio.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gmhozuqrq.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gwagqtqzk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gmqoxiphw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/glwnaoyun.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gagxujiej.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gkseaifxy.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/grjfluoen.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/giamfznci.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gfezwntnc.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gdhbjfrkk.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/goehpkzlo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gruontsjb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gcauokeqk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/ghcmvgmaj.sHtML


<!-- 参考信息 -->