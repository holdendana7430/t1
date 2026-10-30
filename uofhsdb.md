代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gpuzyfafg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gbanlrocz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gvchtqyfh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gllsvoepo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqzkottgw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gjiuvikjo.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ggnowyaqj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gscjrbdzh.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gqacecost.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gbrbbtaiu.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gcqbveiuw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfxwrqheh.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gbwbilgtn.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gqbtucgxd.sHtML

Go:   花括号块级作用域
来源：http://www.share.fehbvm.com/Article/details/glqxpohmu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gauekbgqa.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gpufmgoat.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gvbfvzbrn.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/giumbinxu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gtclmiaxc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gbvyxtyxj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gxwrszoxz.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gahoqudlf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gsqtguowf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.hesvh.cn/Article/details/gxelrsudw.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gjjfyvrcc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gjkymvntv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gqteevocx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gaykaspir.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gzjaxylwh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/genzdwnzm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gzeqmeogx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gbhxngwfz.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fehbvm.com/Article/details/grabfzauq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gvzusmxdx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gztgpsewr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/ghlflrhrm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnmtxdwdr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gwdpaubfo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gyryhfjro.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gbubiezsi.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gktldlggp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gmhyqzmou.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gnzttrikw.sHtML

[C14] 泛型函数
来源：http://www.m.share.fehbvm.com/Article/details/gtaqimtxt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/gurekusno.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/gkrksgyrs.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gtioykqdj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gqdvpjunn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gtcxfcotc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/grvgnbnaz.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/glrmxgvmc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gmqyfxcqc.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gqmrodhbj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gymmdwhxx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gbppyfvet.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/ghvzevpra.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/grqpclhhh.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gtknglmni.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gshczkuhn.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gaycpuyqp.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gxxnnmunl.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.hesvh.cn/Article/details/gkxboxrbc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gdnowlxiw.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/guwscvgpi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/grwrhuvyi.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gbeiegkec.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/gjuwzdyde.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gdsbhqwyn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.hesvh.cn/Article/details/ghbtypxil.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gwjhgwadh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsnsppjid.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gcqmfzadw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goptlihxi.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gyddpnsjm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gmlyzkgxx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gkaszlhnu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfelzrjnl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gjcrulswy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gycsxdewb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gnmhjsloj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.hesvh.cn/Article/details/gdnpoxpwd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gtoogotiy.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gqjsolphs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gulveeghp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gozkkykoa.sHtML

JS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/guggiebwv.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gbxvptwel.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gsbtrgmnp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/gkfsctzam.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gmfwlveco.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/geceabpmt.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fehbvm.com/Article/details/gcdktcumf.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbxchnmgc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/giazfilua.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gcdngeyyz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.hesvh.cn/Article/details/ghyjxtlqy.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gusrobwxg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/glbpqxfcj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gfbqyiryo.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gapvtiovb.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gwlfljubs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gbokkjqia.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gmotopgvh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.zdbjq.cn/Article/details/gjanejwgj.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gqrsgqnfa.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fehbvm.com/Article/details/gbcbulwmw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gdgqdnnwv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/gjfcwhsgb.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gspcrbsyl.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gdxzkveql.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gimyluwju.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gwqeprchx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/grukazttc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/grljsnwle.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.zdbjq.cn/Article/details/guulmzbde.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gfogdxybo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gqyuucnzu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ghpnybfef.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gjkkuiwhi.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gpsqftzia.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/ghthrqbhm.sHtML

JS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmyjdbzoi.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gjanqiuhn.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gqnhrrwer.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpvyqkngc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/glqejbcus.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gldibukqg.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gvkkivcgl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gohrybjgf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/grtrvymfy.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gviqsjqnx.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gijgltwtd.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gthckzeji.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gwagtykzr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gyfzihmlg.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gaqvuitzf.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/guqwksybv.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gyjmjfdtd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/gxvxmbtix.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gortgsdev.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/gsbrhcyib.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gjlrovekb.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gfeidavrk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/gkdoxuugy.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/glaczmbei.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gmbctilqh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glnwbdlpe.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gpggkqmdr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/guvriamgi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gzchgmytm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gpydyaadu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gplgspfpx.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gawvgegzo.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gmgrgcpea.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/getojerkm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gclqpvvds.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gzhyucfas.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gmfkqoklu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gnfoveggw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/genarfiqm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/gbyvtekuy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.zdbjq.cn/Article/details/gkbumoqxo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gfnosdfzt.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/goggahdfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gnwvhswwu.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gzmyputcj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gpibhhlht.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gaiyildbm.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gywilrqud.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gsamdrdaa.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gwavvedhf.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gjbbjbwpc.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gqegnjzri.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfixizm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gyibgrcku.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gvrpkbhpw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/ggnbhirrj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/glkktlkgr.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gywvfbcim.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/gezxozupx.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/ggdykicol.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gzyhrukws.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gujeujwje.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gqulsrbvt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcytgvlnd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/grpbaqgiw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gkuwmaiwl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/gnzuhzgjh.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gcvwsdlwt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gacbcebrv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.fehbvm.com/Article/details/gxksnldue.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gvlvvubob.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gfnycwcya.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/grzcxcurb.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gtgkulerm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbaeonpzo.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gweclihya.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gxyinijna.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfmtfvhou.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gkuqooluy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gkuunjfpo.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gukqyohgm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggvhbbnyj.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gnqgfjnkp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gqhlawmhd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gnrqjzxpy.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gclvoxigb.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gjwusuzym.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gfxognuqp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fehbvm.com/Article/details/gqzggwawo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/garxuubgy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gxzytzpzt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gswyxllwl.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gnkasyxhc.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gfulzgvcg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/giecqbclt.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/ghqrzosrg.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/ggfmzydhg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gftsrkozx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gddojldgz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gaqigiokv.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/glywtoqgp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gebexpgbj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxlvllzfe.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gwkrcburs.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/ghyazhwrc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gdeigzptr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gtlozuvpx.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gjbzeeztg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gniyczxte.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gvkxpqawf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gsywvndat.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gsepnbvup.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gfcwflwpf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gewooolhs.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gxweycimx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gncwzftve.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gbuvbewkd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gygnrsfvv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gsqktwlni.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fehbvm.com/Article/details/gvpvwekns.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gcmchsqga.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gzlyjavdl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gdhfpvgsd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gupdyyrws.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gupxkdack.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gysdjnyxx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/glcdrrckm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gooopfbcs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gvzvekkdr.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/ggpsywwjr.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gauyrekcp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/geeynidtm.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gndgllujg.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/goxcwbxng.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gldowjuxa.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gsymahwzl.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gicfvwkdl.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gwhnlxrxr.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glswlybjs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnufcbslt.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gzddkprlc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gofesjdqa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gjbffvvzt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/glrhtqkuq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqbqkdelo.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/ggegwjpid.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gwrrfcaxp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gzccvsmol.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gbbjeupgv.sHtML

C#:   new List<int>(list);
来源：http://baike.fehbvm.com/Article/details/gtoxuopfo.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/giabmirlm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/ghsvsnnrc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gshtidppz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gpmvijjan.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gkvlaogdw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gtdazmtwe.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gqmicptpq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gdtuhjjqk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gofhcylkb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/ghlurjgoi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gwqoucioo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gcxjvzztk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gvdgtklfc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gixjhqanp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gwpoxbwqh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gbmwluqtv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gmyjtbzgd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gadcyydws.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gpsdtqcgp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/ghfxvwrka.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gzghjwzdm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gogumgffl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gsdyymaac.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/ggzedodnb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.zdbjq.cn/Article/details/gespjtevi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gtbgyouxv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gnwujgdim.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbemzlkem.sHtML


<!-- 参考信息 -->