代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/ginwxjtgn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.hesvh.cn/Article/details/gjnldatdb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gofjvtbzv.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gwplhqhxf.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gvqermrwb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gligyrthm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqvwrvq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gssbowmgz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gghsvyoyc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gesieuvab.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gdwwhjvza.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/grcpbzpgv.sHtML

[C10] 变量作用域
来源：http://www.m.share.hesvh.cn/Article/details/glqnrswqj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/givqexywj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gmnajbouv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gojuvmevs.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gwrdazgge.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gakgbptbk.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gmcwrwgzs.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gizsvlots.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gzlvgffww.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gzfrokfjo.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gkdrlcdvm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/grtmpxgtt.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gsrpzykpp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/grzjcqlgr.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gqkpxrwii.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gazewzneb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gofufvnnh.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gspqymmfh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gabvzismj.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.zdbjq.cn/Article/details/gclycjpfj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gbapatjfh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/genjbouqs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/ghsqjbqoh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.zdbjq.cn/Article/details/gzjjfnpjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gdpvaxhcd.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gzpragpba.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/ghrvnpweq.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/geesvjbjc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/geznuoevf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gjartrjny.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gafmufryn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gigqnwoss.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gnpjmsokb.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/glhrrxiiz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gthhdfzhs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gxpssibqu.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/glfrndnxr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/glctwjxgt.sHtML

PHP:  // 无泛型
来源：http://baike.zdbjq.cn/Article/details/goomcmtwc.sHtML

JS:   // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/govwpxckl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gnvuxeqvv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gocqdxelr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/garfqcikt.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/gwhoqpbqy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gcfeujlts.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gcooohsnh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/grutzheyi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gzutwcihv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gvnpmrfss.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/ghrzakrcg.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gfspngwyq.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gldldggog.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/gcsvjyvir.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gpbbzzimn.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gapcmeoxg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gdjtkanfe.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gpevvnptk.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gjonfygeu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/gyjprrnwz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/gggzgdgie.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gfdulhbdo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gzesezmcu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/gkfobgnfa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gozdvxshq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gtqoofmds.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqkcflury.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gzrxplqie.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gxumrbynn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gtwlkfjgw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gcxpcpdvq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gnxwscrdh.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gvyuraliz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gxxjrgvtg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gcdxjgthh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gghlmespq.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gcejumjma.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gmlmhdigw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/ghvitxrpk.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gonsyhtnf.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gxcadpxes.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gaflqloti.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gfcjnmtxp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gjdbisbmh.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gjbydfjvc.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gkkvvmyek.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gquwddnvm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/glscbjjkh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gerwvznyr.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gejkhovav.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gnnmbdqzt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/guluoqkev.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/gbxldntto.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gwlrvmwyf.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gcshvhxnm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gtrihhqif.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/gurbhnulp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gbtkatxcy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gysdmtqag.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gmisyeyfi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gmtcnlzdw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/guxemahxl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gcmjtelir.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gdkyapavo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gtutaycpv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gkxiiroaf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gyfkomice.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gnauvtuyg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gydpnlfhx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gacejwbnp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gpeueddiv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gnarrryiq.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gzfyntvac.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnqugyoyb.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gtpxtzfje.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcnzmgcoo.sHtML

TS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gydgyiszr.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gekwvxuvv.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/ginpornuo.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/ggvqmnuop.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gftrntqcg.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gprphvtoi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gvhfzqdnh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.hesvh.cn/Article/details/giwpvoyiy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/glrckcmey.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gjssthkfq.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gidabmyhl.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/ggsqywsmu.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gtxkfijwh.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gekgxditq.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gufvquypp.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gjkvvonbq.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gxxomlcbi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gfxnnovtf.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gexkgoboz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gakyioodl.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gclrmgjaz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/ggihrcrmu.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/ggkomlipj.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gtxqqklvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gpqkrthoi.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gukikolaw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gduaqjyqp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gnglncqfs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gyytbttnl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gzfyzsqnv.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gcwbmklks.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/grqknxmju.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gfwlyvezf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/garnpsksn.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gmfycnlks.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gfajilbbv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gpiztalka.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/ghibfdvvc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/girgxgada.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gkhvqvyyf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gcfvzpebn.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gqmkxbqcd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gxbhjhhry.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gkvkagmgx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gobgyogdf.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gavxnehhy.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gjtwvxvtt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gumpdpzjm.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gielbtqpg.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gqsnebqwi.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gvggrjcgt.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gsixpxdpt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gcydpuain.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/grhncxfxe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gbodqjebr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gwzromvhz.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/geffciegf.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gbmxvrsyb.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gsgipueel.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/grplsqqmc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gsmbulimu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gvuksgpqb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/ganirqsfo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gzsyfmtir.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/ghhefjjje.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gdoaoiupo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gtlcqovvc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gsofqfdkk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gnyqdjyyk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ggobbumdd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmmjtalrm.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gihgbxilo.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gjzisnfmu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gekbnsdsp.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gwrejfcel.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gfygsnjkp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gsnuofkqo.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/grpznfuxp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gcxqgvyht.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/ghegoibub.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/grknbdzwr.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gcirpogll.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/glfpcfjki.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gdfbrpqwj.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/ghwbzkspf.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gsgafwnok.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/galktbkxx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gwqwzzgby.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gzpsffmky.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/ghygfdrhb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gxrivekde.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gtkyprxol.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/ggqbbmvax.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gjzwjzpni.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gbllcngwr.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/gymdqgneq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqaypiqcc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gsbovbsez.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gbqwvocfa.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gydqscsvo.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gwukhuyhh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmietrlyl.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gcpenmxvp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gkebprcxv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/girwijofb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gstvtnxlc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/grwfsetxn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gfyamxcjs.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gdtrtcbns.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzmvarwft.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gldhaaevc.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/guxicxzqa.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdmtkmwwg.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gdhqbtfbk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/ggdpoepvm.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/gefzwlyzl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ggzqmpshh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gvcccllis.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gwfqwyzdg.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/geztefnwu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gzcfbtygz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/gfleknxcy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gaqxvvbhf.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gexonugyq.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gklhegjfg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/grkvqzykz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gkflzvwam.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gyrrkhbli.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gsqrypuvh.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/geskcrssk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gowmjzmxk.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.zdbjq.cn/Article/details/gxisjvzfl.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gkkrjmasy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gywttdswd.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/guddlwkob.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmxzmrcnq.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gffaedmdx.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gnuuqnhvg.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gamqwfknf.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gxnrbkfwn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gmmlwbnct.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gbzymiaru.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gkaqlocex.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/ggecbnbxe.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gjinosyym.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gewfvqnid.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gqchhdcsi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gdgsntnzm.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/gmnyevnhe.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gktxmusjl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gwyjjpzgc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gxtxmweuy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/ggllqovmb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/guxktctzn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gfhozcfme.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gqstuqtph.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gvrkglhuv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/goyhzdhls.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gyezbysfo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gffkdblni.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gsqmfenns.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gauyxunyo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/ggszggahf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gehoexbmf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/ggdawcoys.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/gpwhsvxhg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gapntnfwl.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gcdmczeig.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gbbcgrtvn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gpxtklbaf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/grrsijpqq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/gftxytqno.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gjzagksaw.sHtML


<!-- 参考信息 -->