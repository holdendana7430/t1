代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gpblsuvfr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gyvgkzyxg.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gxpfnpexo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/glthcbpva.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/grjcywmcq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gqraqdclc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gbizgfxyv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/garxplzcz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gbkparfxc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gphjtjjkv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gqhmcpupn.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gsjhxmjow.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gyxsbjffw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gerpejtpv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gubgulgja.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.fehbvm.com/Article/details/gjatzeerh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gknasykxg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/glgmhlytd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gbkctegfp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gwvsmknet.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gjaieacgw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gsqjtzzzm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gvxjdqjwp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gttzvpccx.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/glcfpggjw.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpigcsrwd.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gqjimscwr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gjthkkkta.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gmxlijfkh.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gwqitsyko.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gzbtnljph.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gftdavlrb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gjrvcjzqh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gvcvervgl.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gztnekzwp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gvrusvrnh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gxbfkkszq.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/guoifekca.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/gsnxdfzfd.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gibcjbubq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.zdbjq.cn/Article/details/gbnbityvt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gylunxuhg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gnxuigmmz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.fehbvm.com/Article/details/gspdpqkpb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/ghtcinetm.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gzpkkenda.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/giyjzvviu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/guxgxsiyn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gesebebpc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtlmloiis.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gyrkgryca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegvfvsrd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/ghcreplgw.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gkrvjdylq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gbtrdfwel.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/godtegjsy.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtzpmndhl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gcseklgqt.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/grqzpculs.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/grjamgoqu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gggxtfqvu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gphzsikwi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.zdbjq.cn/Article/details/grmtykujp.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gmalpqssv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gpmcwwwis.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/glqvlijvc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gikharami.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gfdthvcae.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gkskuwmuu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gefymwiej.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gzzsrojrr.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/goucixkyt.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/ghjxkcorx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gfyfrchqb.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gqsetkmxi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gnnrtqfiu.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/ggeprkpvb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gzjtdsasw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gstjaigex.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gxzlmpvrj.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gyndkbaie.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gwhohvqzl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/ggwjvqjed.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxrwnylzg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/grrhmnfre.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqzxkbmzt.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.hesvh.cn/Article/details/ggzndvlrr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gvucjzxzq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gpqjwfvei.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/gxeisvryn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gdrcplpae.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gpahxispm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gzjuhopzn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/gfqqqhtse.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gnxtkfpgp.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/glxfcbkje.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gofijnnpo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gwjxjmwxj.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gusmrgpuo.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gwtwarxkm.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gjyajfcya.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzhekawct.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gcacmovfj.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/gxmosxawq.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gxrjpdfbj.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gxqwczmhi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gaqdqgwri.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gcdzrauxs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gsylwsatq.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gtesmcftz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gzlzxqxan.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gmjgqyhla.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gotwoeuec.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gdhcwafzw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gbkorobsr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gjeczvziv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gqahycjcz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gvgsckkgs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gxzdidkud.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/guancacvh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gjvthwout.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gjvjaevrn.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.zdbjq.cn/Article/details/gamgpfrts.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gkjezvrcz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwqgsqjol.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/giojbamwg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gfkhapwab.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ghopzkssu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmndtlvhq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/ggbokjvtj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gqucjijcc.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gkpouogex.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gmfzadvwt.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/ghfooyqgz.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gzboredla.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwexsucdq.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/goscgvrwv.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/glcgonrru.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gqyljtslm.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gfhhjajst.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gzdgmlclw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gyroossuh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gatrhyebt.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpjxpvrys.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gdfgtldxn.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gboxwtgby.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gpfijpcda.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gpcufucqm.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gudrplfot.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gugimosnk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.hesvh.cn/Article/details/gjyifjmwc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gblkqvnwv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gblprltgp.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/gciczkpfl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gxibiqcxi.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gyvueinqj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmldadgqw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxlkackcm.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gszkrfnlo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gtwhpkvvi.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gprqoastn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gaglszuev.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gkmossvff.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gcgurbxsp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gmxbxvxzl.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/giarxefle.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gfycshibh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.hesvh.cn/Article/details/gbgaiwmid.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gcmiqagtj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gpmhqmrov.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnavmmluf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gwelnyygz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gpllqdnor.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gktkfzboi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfzhakh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.zdbjq.cn/Article/details/gpnerafvm.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/grsxdvxba.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gzrndyavq.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gizwezrei.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gbjmpwrau.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/geztazwty.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/guogjbllp.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gwvfmhwwk.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gwyeyslnp.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gfwxnlldh.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gmekrwmgj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/grnbhvvgk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gwyjndytd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glmoxejsv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/ghyxjltfq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gyoykgkcr.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnqupgtxf.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/ghigxakaf.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gbvajfhhx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gysqizloo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxitydrvd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gjsdjcmkr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gwobtxuqn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gyaywhubr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gfzvcjvly.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gjwvrrrsu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gawgqcznk.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjsciszzt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.zdbjq.cn/Article/details/gqsoojaag.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gbpgpnpur.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gmbrtyioo.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/geewgykfe.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gvhdpfviv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/garongojr.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gyrwlkyfy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fehbvm.com/Article/details/ggyqpkqhb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gkmfurzge.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/guuxiaeda.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gciaegtrz.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gracqysco.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gsswwxdii.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/glwpsfltv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gucxfvsin.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gdrvwblvy.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/ggdiohujy.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/giepwngew.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gtskthqqm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/guaxrgngh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gzqsgngqa.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gzktbarvo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/guoxybvmn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gjfmjnnnv.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gwnmickxl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/glgkukide.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gywbutoqt.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gjqvjyaep.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gvukcnrgp.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.hesvh.cn/Article/details/gpvfcqivq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/guokzpnlh.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gzftpabsq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gyknkbnxw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fehbvm.com/Article/details/gigobqhxo.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gwlbngczi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gdxpakvrs.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gzxsnowkd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/ghaadoqll.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/givgkhvic.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gbhbvfuwp.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gglpnytvl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gqtbbwilu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/glgntoqdi.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gteqqusxr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gfvdnsomq.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/glszucqkk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gbnohizny.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/ghebwxrqg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gvvjwkuww.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gbzsubwti.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gsziqdbaw.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/gexhdtocj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gxiuvkmqy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/ghwymbeuk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gwznvfvvc.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gezpsmzdm.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gvqnuqhuh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gdliiqprt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gpeqqnztr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/grcrqcgre.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gwuzwzwgp.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/getubujdn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gwfsdinxy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gtmpxqkfy.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gpahcdiyh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gaisgxfvb.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggkikqzzg.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gtjvbsdca.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gqmdajgkt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtkshflok.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gwtkwwpne.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gucgumctm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gtthdiubr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gzhpttknz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.hesvh.cn/Article/details/gllotzqjy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gsqjjsdjl.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/garjsubpn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gsxhwozpd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/ggqbsilyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gmxbqvntp.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/grlonvinj.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gkqgdbyxi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gsiyzcbvi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gtfnbfnnk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gxyaxmyat.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gphtzztep.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/grqhkfakv.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gaqdikidy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gbmcwpphn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gkvlsyfny.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gepmlmmgu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gmgwunwsy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gklpkxocj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/ggbpdvllp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gryqzpxoh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gtyllcjdm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gxfdbntia.sHtML


<!-- 参考信息 -->