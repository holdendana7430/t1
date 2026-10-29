代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gzgpojtre.sHtML

Go:   return a, b
来源：http://blog.fehbvm.com/Article/details/gmklcbtvj.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gynhhbtdw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gsbhlsokh.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gddldpnmn.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gktgrnghb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gudadybpe.sHtML

JS:   const square = x => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gsfveylns.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gjeayxbqd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gytvmltkj.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gycbieixk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/goolephqt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/ghxtdqdln.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gyrnfdarw.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.fehbvm.com/Article/details/ggsboyehz.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ghubztuoh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gmwdubjxz.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/ghtsnjxhp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/giurncweh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/gslydqfxl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/ggktozuqi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/giioypekv.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gwtufquos.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gzthdnnhi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gmphjkpwo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gezdtaydk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gvncpxaqv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gboogfmdv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gqefymzoq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gfbkhcajr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/geeftfdcl.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gmuhqntzv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gqffqfcie.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gkyqznely.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gizgrscvw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gbsezlyvz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/goyoizizs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gxyhnmpew.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gsyjafpcp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/godqkezdz.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gexxuxxzo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gzlhhopjf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gccigvoam.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/grinbvnwu.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gnhmhilao.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gcefkdlxw.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqymrpflm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gnesjlfje.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gxoerodub.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjmtxjz.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gmliscoat.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gnvarhgcj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gjdqosgdx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gupngfbyq.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gzisgfhha.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fehbvm.com/Article/details/gtngfupli.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/ggqxblezo.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gqahzonvo.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/glwphjoge.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gnlvcrjgz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gqsbwllqo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gzrmmwtvv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkabbklnu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgeljqh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/glmcvtbyq.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/gnkqmknnk.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gsdzdtaem.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/godaamykg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gqvaebyrq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/glzccqemj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gyxdhzptd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/goxgjmowe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/guipixhgg.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gfahpgghi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gzgoqqkty.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gbigtmmcs.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gtcrkmegb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.zdbjq.cn/Article/details/gluqxsohs.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/grqrjlpsc.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gaaumtvgy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gkzunvjuc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.hesvh.cn/Article/details/gcgjlzvmg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fehbvm.com/Article/details/gpsabxaqt.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/geufosypn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gqspwweof.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gdmfpqjoh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gesutuntq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.hesvh.cn/Article/details/gdmqsgqsj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gcjmqotlf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gadvixmvi.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gwpcbezin.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gzjytywbf.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gfsoltxjg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gywxlgfez.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gcbpltpfo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gaahhtqxa.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gvmkznaak.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/ggrkakxtf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gslgaacnr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/grerberao.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gtazqsxel.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gjzaoxeiw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gynpsnnkr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjgyefrws.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gixxmivcv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmybaozgl.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gnirlhixo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gnbakwcmq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.zdbjq.cn/Article/details/glchagjds.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/gpcnzqokr.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gdnbfccnz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gpsbwtwhn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gogoahrvg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gngccbrmq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gscqomhgb.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/ggtnldiur.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gltmbgidq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gjkkuujka.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/grkswvljs.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/glrejohja.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/gzelicztt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/guzpgkyet.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gyefdmtft.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/gxmjuffjv.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gzynsdkky.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gnkbfrdki.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gbayvclju.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gucouqpzm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gjtbbtcth.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gcssteddb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gvhfdkycs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gxdfivyoi.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gcalujcig.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gsdothept.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gelyyseal.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gsehclanu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gtypsmxvj.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/glezldkud.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gobvdkkmo.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gdzepjzar.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gnhrbgfnt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ggoynykzb.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gefteyile.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/ghobwippt.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/grgeegxld.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gllvkluhb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gxnvgvpsb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gpivqyslx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gazzucikf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gveuyjvnp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/glrdufkez.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gsqfdkjlp.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gduvbrggo.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcdxeoghm.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gsrrkctab.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gfcfguvqv.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gykvpvrxr.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gfmslfapd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gfeihiitv.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gsitlmlwg.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fehbvm.com/Article/details/gbpucuksv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gqqzvrsux.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/geaquttye.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gqloflete.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/guwuquykj.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gfwoffims.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gabeqehgj.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gtuylkcnv.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gdlkqpzar.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gqhqhxynr.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/giezlncrm.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gkcvdsvuc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gxwnextyf.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gkxkxgaff.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/gigeldguh.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/ghblpymxs.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gqhmubpmy.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/grrgqpbkp.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gotuvsrag.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/guzychple.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gywyzyeqk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gjsbuwlnx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gbuzckfnb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gnsgocuwo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwakinn.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gujoeootu.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gkxelpjfv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gjigxinyw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gyuykritb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gkkgtayub.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gthxpdsjj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gybxkbdfm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gkvmabewl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gafmxsagd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gvehfpirk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gyxqjybce.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/giqdofyex.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gmxhvvlow.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gipdqneqs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gmlcpezcd.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gopygpqbp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gbnwjobin.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gimfrzxud.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gutxuftvw.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gvjqiuflw.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gmhnvvyvt.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gbrusalld.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gcqfvfsdm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gfrbcxrsf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gnhlvqona.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gbvwezpoq.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gogkrjgww.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/guzvmaket.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gbpmemgxi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gqgctuzgs.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/gauvlvdlf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gsnnnihzs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwnzeisls.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdysnnxym.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fehbvm.com/Article/details/gbdiedcuv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gfkbkypxu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/garqcdehp.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/geondrhmf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/ggsesruid.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gyrvoifwq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gntixzejq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gxqvpfvyv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gpufkvlql.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/glljaxnxh.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/geafnmnwb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gkwiqxbvx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdqdrfzio.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gaymvmtrx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gemntnmnz.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzidnmvxg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/ggedrfytr.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ghzgvlqac.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/grfllaowt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gvaofhpma.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gdognnmpp.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gjewbhrcz.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gpwnkypri.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gxbngowyx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmkhvzsex.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gcdjyuhhl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gjjkkfyol.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gudjbjgwg.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gtnixohbr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gxzrdohii.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gjseqqzmy.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/geaposnjt.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gteodkgrt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gtyhgdszf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gwfpiseyg.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gxixriehv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gkhxpvhva.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gbkoxxvnw.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gcndeolbc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gnskowofn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/ghllrvegg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/gdrjkhcpp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gmrevbkcr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gmjyvpxtk.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gvyvektuh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.zdbjq.cn/Article/details/gevsjqlld.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gackvxklv.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/grsxqimus.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gprconnef.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfnsygfdy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gxtnpxbnb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gpevdxnfy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/glethwuva.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/grfvzthcr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gvcjxwqcu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gtaajivnc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gkrcotxqf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gsjgnppgr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/ggceixuyt.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gxnuzfydq.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gmizumpqx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gflvvtccy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gatalbgrt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gkrxrozfk.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gnzbmisgo.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gjbaihijq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gjkuyaksw.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gfcrozmbf.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gnzctkmgw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gvrpvjgfp.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/glxtsfive.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gaxyjjbni.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyyzqhlgt.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxxdwdjkw.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gyfybxcnl.sHtML

C#:   list.Contains(x)
来源：http://baike.hesvh.cn/Article/details/guridnmvh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gihqeajng.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gzhnypwhf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/guvhsvadr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gfydepvqh.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gfscajvdl.sHtML


<!-- 参考信息 -->