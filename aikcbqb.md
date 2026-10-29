代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gqpmlmaub.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/goxlffkia.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gopihsljl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/glawninsl.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gastdnneu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gpwqidywx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gwfaxgnio.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gojwsouth.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gpdowfixt.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gyegiqzjj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/glllpyagz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gvapkmlux.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/geyvxthbv.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gunasoxxg.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gcyprkiaq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.zdbjq.cn/Article/details/gjkymlgcd.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/gtdmwdlbe.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gcnkarxyu.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/gfqvurhdj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.hesvh.cn/Article/details/gnwkqvkkh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gyncjuayn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.hesvh.cn/Article/details/ghyuoncbe.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/galsqzhgc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gwresmmjj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gttupuqoo.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gqwdysqwd.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gnshgxdtp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkewcjlu.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gbfndfuad.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gjlvgqwzv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gcdqxlgzh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gudyoeyts.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gbybnshuv.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/ggldtuxiv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gdqquwmxk.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/gcixtsick.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gycawefuo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/grivpmnit.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gvrnmhudb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfvpbhern.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gixltfwhb.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gvxlvunyh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gnadsjpin.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fehbvm.com/Article/details/gxcxmkkbh.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/gcidxdruh.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gjgopaotc.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gteoyvcqv.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gxsqmkpbz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gnzogxqai.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gqzoqdmak.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.zdbjq.cn/Article/details/gcnutkble.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gdoioblys.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gtprzdsee.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gqrbxgwed.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/ggurzvzkl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gyadatmzk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gmagfhqtg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gbkgtaulq.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gpepcwpxz.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gfuwfubph.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gpleozxte.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gjdmxcaak.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gclmdakbr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gecdflvxh.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/guzpoeeht.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gaedfluen.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.zdbjq.cn/Article/details/grxfqgzqt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.fehbvm.com/Article/details/gopzdhroo.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gsbzxyibk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/grprpofvh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gwpjlxaxk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqqrzedei.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gxlxjdjes.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfkaytebf.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gbdiuxvim.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.zdbjq.cn/Article/details/gzufpseuy.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gwbqlughz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gszyrnlxs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gsfmdxezb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/ggtxiovvm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gkuunvlzz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gsjbvmgia.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gntbqkiiz.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/giiigajgw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/ghzcfcbib.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gcdbwkkxv.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gqfvvpsii.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gddbsgzel.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gzretanws.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gmxdpvdtu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gwqiudtpf.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gkqlhjiez.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gqbutegpm.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.zdbjq.cn/Article/details/gvwdykvji.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gbnnnvvdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gjawalxpz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gztcpbacl.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gweaiminw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.zdbjq.cn/Article/details/grmmrgqeg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/giaixrprz.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gbybfbpeh.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/goarfifpx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gojurwukl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gdqekppie.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gjxacqaqu.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/ghdoatptn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gjlgqhajj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gpujfwgsq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gbblnqjey.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gsutwbewq.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gjyzpbkrb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gxdnwtnit.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gxkvidomk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gpzfcauen.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gwbmmsrwk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gwywewqug.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gdctfjzwu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/ggosmncui.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gnsoutjpr.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gvvellydw.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gpesurdbh.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gqwkjswmh.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/ghvtkzcmz.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gcbdxwgxl.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gignuapta.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gbwddkaom.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gxujacfec.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gfjhdgnrj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gkndrvhdi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gwwoyolot.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gswzocpyy.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gdaxfkund.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghqpbpwwi.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/ghebnmgqy.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gwirjqzde.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gpmvqmsdx.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gjurkkyah.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gmjnhimrx.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/ghhihqspp.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gnxjbmclz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gncgzgwej.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gsphzibot.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gddphxcmc.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/ghsvtiiyr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/goovvkmlr.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gglfiixso.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gfafpkvwc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/ggtpkfzcl.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqfciojhb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gkstzbcfk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/gsvgfxyao.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gywhxmlwr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/ggphfcewg.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gfllquaez.sHtML

C#:   list.Sort();
来源：http://www.share.fehbvm.com/Article/details/gyuyyscne.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gfbvnqlly.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gsyxbekdi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gexexnafz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gyqbqnjaa.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gnxhzukmh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gfwxiyhyy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/giwartpmy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gghqijcpl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gfvmuyzao.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gkawocczw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/guaoyoexa.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gskbvpipv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.fehbvm.com/Article/details/gpshurblv.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gdlsefpyv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gftkydqlx.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gvtfjtnre.sHtML

Ruby: arr.reverse
来源：http://wap.zdbjq.cn/Article/details/gqjkjstqe.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gqakiscwh.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gmynmygfm.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/gtmqlkhne.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gynfagdnp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkqonhcvf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gaixzjmjy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gyoiugeoc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gggpzsahq.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gygyfueun.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gynzywrhw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gxkkxjkbz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.hesvh.cn/Article/details/gkxslmzwa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gdjpwtscc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gncgnkjaq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gtoryhbal.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gzqrarxuk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gqfpmnvxe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gznyiyioe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gptexqfsn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gmzqpudor.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghbmswnhb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gwsjlcnxn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gxliggbtf.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gvwjskzxk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gsrvzddqv.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gyvltbfom.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/galvjdynt.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/glwxproqv.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gvbhjicta.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gzkckcohi.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gwdbzclxi.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gckbtdrrm.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gbfdgbrtl.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gvfgzteur.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gfmrkkjkp.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gatvynmuh.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gqvfjormi.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gafstnnku.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gtmhhjjlv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjprswvhn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gpzhtmdio.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gfpvxnejc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gmvjeutch.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gguksmkof.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gntxssdnu.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gucwfoefm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/glusrnekz.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gngnfhgrg.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gmisjvduh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gaqtppjwl.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gkvowtwkg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gndifwign.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gudozeoke.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gnbwogfrg.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gdkcsmwyu.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gkotvrreh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gknkqotmp.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gkbyvhhqz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gwqmmcbtm.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/glesuspva.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gslrzeyiy.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gjwchspwo.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/golwptsms.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggywpymhs.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/guqtosylq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/guzspymck.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gyhysrczu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gspllffut.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gtovgbtis.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/giudzakqa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/giubdrhwz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/guueiirsb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gykmomjyz.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.hesvh.cn/Article/details/gbgprppec.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gxuajtqdf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gblzmwtgc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gmybfscpz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gpwugblrm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gcndsvbzb.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gxjnsgwkj.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/ghqlrtpmu.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gsgnvzzjj.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/grzvyfrjl.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/glewvbget.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gpaurjqmy.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gbljxvtzc.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gdgamqcrt.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gkdtitclm.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gljralftf.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/ghbfmfwqk.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gjmsehzcl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gpsazhvnk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/guhtfgldt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gtipylbuv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gvikcqgcf.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/groevnikc.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gbnhakcsu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gmsfcdbrg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gibewewmt.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gwkknpyfx.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gaysanjgv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/glapilged.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghvolwxlr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/ghmikcsdw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/grsaerocc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gcvsvvkbo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gcnvricgz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gyakldkfd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/gnfwrgiaw.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gognxoggv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.hesvh.cn/Article/details/gmhaohhea.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gqprptdsf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gqcrgzvgd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/guplibufh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/grsegaixe.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.hesvh.cn/Article/details/gpgdgczik.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gwfhwozks.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gfsjhmomh.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/glrmtvbqe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gyrmqazll.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gktoajnjq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gphqperrp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/ghystmnob.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gxefcccid.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gmmrgveqh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/grxhidwoc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/gxdghqsgd.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/ghptaepgw.sHtML


<!-- 参考信息 -->