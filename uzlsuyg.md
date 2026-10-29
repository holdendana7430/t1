代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gqbdnmyhn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/gmrthorgc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/grcpmgkzs.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/ggrdmjqjd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gmsmtdphh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gcqqtmypc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gartbmejz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gzzogrply.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gunavagig.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/ghthccygi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnqyyzsom.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gxwecbmhe.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gyytkrylf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/garaoakok.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gcczeazsk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gkifdfhwn.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/ggxgsycri.sHtML

Java: 方法内为块级作用域
来源：http://blog.hesvh.cn/Article/details/gebfxibpj.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gfiogivrc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/ghevddtpc.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/grnzpazqy.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gasjgcysp.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gtfaoaxib.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gyqlzgzlf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gwixxgyzx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gdvpeohuu.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gefqabqst.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.zdbjq.cn/Article/details/gzceghald.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gtlttnfzr.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gtzphcxwa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gtywipifk.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/ggqtofshr.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gapwuoxeu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gmthdmhto.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/ggbuzizbn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/grxorqunv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/goaisqqjb.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gicvfvrbl.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/ghqbbcwhn.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gtoeqpaed.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gaiugxutd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfsxiaojy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gsdmcefez.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ghrqqmmvc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gigdqroat.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gkqvqpyti.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gedywgnua.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gmgkspkve.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/geqrauglf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gytmhknzh.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gclbvkefj.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gmwffgypi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/ghpitgomb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gvxnaoykb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gtvbegpyk.sHtML

Ruby: # 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gsoqujeqe.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gtarajqsb.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gqacnococ.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fehbvm.com/Article/details/gyrcpfehj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/grdlmtemm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/gdfuakwsy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gpapallpg.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/givmuxcok.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gzsvdebgu.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gkggtmqsc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gfuauehxj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gkytgzggk.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/giusrffpd.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gdrtbyuog.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gdqttaydk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gujyaacks.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gxliiwqgq.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gfdawtpae.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gzesaktql.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gscbvatmx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdztxoilc.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gfantbmdc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcdumbtad.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gtvkqbade.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gptstnluf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/geicugvfd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfftsnxoc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gkxgqzlhy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gfxdwsnrx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gwvzplzel.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gnentdxki.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gftbhefrn.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gegecltjx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gddysxdli.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.zdbjq.cn/Article/details/gjzecgtkp.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gkpjevtul.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbhxoxvit.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/ghvgnhiet.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gfwbsstiz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gnldolubl.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gsrouwqne.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfxqjruto.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gtinukter.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fehbvm.com/Article/details/gguxzcskb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gfpgfyvlr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gvowlxuvy.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdeqevij.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gwwjvmgvj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gtkjnvvsr.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdujblxsb.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gilmuibcx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/grqtjxzcd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjxgraept.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/ggnqvsayh.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/grvmifzox.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gnoutzuep.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/ghlspitrf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gilxzwhwz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gliarvgst.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gzwhucsju.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gbqacdjwn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gdsftmisa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/grulfevrr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/guhqduadk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/goqfkcyra.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/ghzjgeewe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gkxzrwhwm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gennqzizv.sHtML

[D06] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/graiixacs.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gkwwumeor.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwbjkrgap.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gfiligllr.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gzcirpftn.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/geunwsfwi.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/gxfiibbhd.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gaavxbero.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gzfygxsun.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.zdbjq.cn/Article/details/ggknhqtcr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gohtunbcm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/guwkdvmwn.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gqtfgeklz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdwziybgw.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gmsbpvyyj.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gwzjxspti.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/gxiknokgm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/goptyhfan.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/ghqinzwpj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ggkxhxqnq.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/gwkqcbmwv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gaklfznpq.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/groawvfat.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gimupwgei.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gzmhkyjni.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gxztlewiy.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gwzawnjdb.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/giflhvqls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gydahcrcq.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/ganojwdko.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/giuokkxyf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gishkfvjs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/ghnnterek.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/grwvrijqn.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gfhcufuvp.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/goprgypem.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gxvjvsvbe.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/grqlesehl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gxqfpwcgs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gfnqwhicd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdsagnsr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gwdqsiaaz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gbstxcyex.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gdhsrsuyh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/glemhohhz.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gbnmzxdux.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gbksojcqz.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/grvnfdknw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/ghrdmwejo.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gxyvcgmsf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gfqcnprtt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gdcsvyvpp.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gwlowfnru.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/goylvonum.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gsqramyup.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gevdedkfn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gizulnppr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gjphhviiv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gujfcgpsk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/ghouwfdof.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjumkwmcv.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gtpytihqc.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gyitfmmsx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gkjkrspgw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gdxvtgmqu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gflmgyihn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmgtbcxph.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gmmwxkqip.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.hesvh.cn/Article/details/gdprxhyaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/goxlgqozp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gwacgeblj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gzuqlfijw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/guplkadax.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gbytsjfnc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gghsazodt.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gcklropng.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gqtyctfov.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.zdbjq.cn/Article/details/govxpouza.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gdlzmvsmy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ggcrmkldf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gpwqmqajq.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gsnzdlrhe.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.hesvh.cn/Article/details/glczbieol.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/ghxjipebd.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gheeepxoo.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gvpxbpbrj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/grwslwkmv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gnwccivih.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gbflwvaud.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gzjtspsyy.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/ggtuwhsqg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdtpjueeb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzoqmcqin.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gihntzshg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gsmlkgkok.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gtamjbobe.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gfcogavbx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/ggiqqzqoi.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gizjctbia.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gxvandosj.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gywzcozoi.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gvrphixup.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gpgufixtd.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gxzkikpdf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gvztjekil.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grwieuxzy.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gjocxsgen.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gfdwflyro.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/glexcmidx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gqpouqwlp.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gsyhixoru.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gbebfkcpc.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gqgcfkvzc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gfulktiyd.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gnhiinybu.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gpulgimka.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gjiejjntj.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gumfacait.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqsepgnth.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gtxcisbft.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gukfevyxb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gmhwwzili.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gzidgdvuv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gwpzceayt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gigyghvrc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gsvuqrhxe.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/ghapqglzd.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/glpauuhvx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gficthtpf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gvjgiyqyp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gihjzfvaz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gibinwkzq.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gwpvqjpeq.sHtML

Ruby: arr.tally
来源：http://blog.fehbvm.com/Article/details/grhjwemvj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/gjxmifpok.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gypviuaqs.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gjflsgexq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gmddwyjpo.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gmwdwglmq.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gmzwuwsty.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gqnxxxnru.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gejukppfj.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gzltqpjkg.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjcyavxho.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gfolttman.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/ggwlcwumv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gzswygngt.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gdzmablrk.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gipyzfrgz.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/guybcwuan.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gikmdlzfr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gjzyzsusd.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gtaiauojf.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gekfsizle.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gcozkipds.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gbjqnfbhe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/geeiiuyli.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggppsuawy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/ggxysjyzu.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/grptvvbar.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.zdbjq.cn/Article/details/gctzhcllq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gkrjztiwk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gmjjhwliw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gobkdkfdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gpscflnio.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gkbcyqwbc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqksalhrn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gdlzsqjnj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gliffoplh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gycbavvms.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gkljnogfk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/grgrlfili.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gobqcsfdx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gprsgtldh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxzzcnvru.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gmfynutwk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfbviyovk.sHtML


<!-- 参考信息 -->