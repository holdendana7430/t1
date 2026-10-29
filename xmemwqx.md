代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gvwohsnfs.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gaccihzgn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gpiiyvubx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/gefvxdrwh.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gwrcxizso.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/guezcntkb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gmhdulkpl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/ggsghpwlz.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gshbrhory.sHtML

Java: 方法内为块级作用域
来源：http://baike.hesvh.cn/Article/details/gtutfaugt.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gamqderfn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.zdbjq.cn/Article/details/gosuekqdj.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gzgzswyix.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gicwovooc.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/grcpobaey.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gqiixomrk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/glffzgvdg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gmrlrxjxy.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gicadcddd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gilzdskzl.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/gvkjdoyop.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gndoevbhs.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gldufawml.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gvkckzwmw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.hesvh.cn/Article/details/gfupvjwdi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gyrkwbzup.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gihypfqqz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gfigqmyyd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gbxugprxj.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gtaeynlni.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gffaopkiu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gkkrjxhpd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gfqdwbdgx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/giknanrha.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gwngwtane.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gflbetxni.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gdprtstkl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gpqaexhzu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gkiwhwlxg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gwawzuebx.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gqpqefbzx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gemxtdewx.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gxvztyazx.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gszbufqnk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gsqoigskz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/ghgrhigsn.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/giztsazug.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gsrdmfshu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.hesvh.cn/Article/details/gaamyclou.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gsviqzqkg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/geuyyflri.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gidubsoml.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/gojcmlbhb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gqejmigkf.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gvnhiorpi.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gfrhbgufa.sHtML

Ruby: a, b = pair
来源：http://mobile.fehbvm.com/Article/details/gmchgayco.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gjolcpuwq.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gkqiouqhu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/ggpbybdrf.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gpwrdukiv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/glstyuumn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/ghaqcsdia.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gedxiitat.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gwkqbpmzf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/giflgqjco.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gljswmhqm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gevwajfyp.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gyiocvnfd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfgwvhbbm.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gdltxhdfh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gercuihve.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gricezljc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gpondduwf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gnmvkvttw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gbrfjsakj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fehbvm.com/Article/details/gttympddy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gdeckvlmz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ggptdlxlf.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gfahleyjl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gyhyrnrzp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gzbeducaz.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gbxjjlyek.sHtML

TS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gtvdhhqvd.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gevnauxct.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gkcgehkfl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.zdbjq.cn/Article/details/ggrfkgdce.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/gdecwfjwj.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gadgzovma.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/goipxpluf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/gjifsjnzr.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gwebvzzbo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gorlxhqvm.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gvwnqwbnm.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gfjsilggj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gqbsjzpej.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gvqetowfz.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/ggfepwued.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gkyyaqibt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gucvzpesv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gxfzcbvzm.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gsnbmizsd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gqurucozu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gqqshsvyi.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gvgvfkdts.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gnjyehltr.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gukbmdsbb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/guioqjpwg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/ghceqpbnx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gplavrapx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/grkqfxogb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.hesvh.cn/Article/details/gpqjguagz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gigeltrwj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gaekvtdng.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gnntrrxrz.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/ggdkvlgir.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/guwwflqvi.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gtmlrjwta.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gbsgpbdvu.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/ghnqftnyg.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/gbcugrgdk.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gylflglqb.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/glkkjxeua.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gjyajnrbr.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gnvxxkhon.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gdnpnlkgh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/gytjzurtd.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzgjxszjm.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/grmufxxxz.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gykksdmnd.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gyvermsvo.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gixjowekx.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ggkeidlcg.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/glmjidcpq.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gxamnaqua.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.hesvh.cn/Article/details/gfwwtkufj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gogcupzos.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/ghmppdipq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gkmnypkqx.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/giwmmrxem.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkibbkauv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gbiggllqg.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gyrlpivhj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gfomjgzdg.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/ghagbsqom.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gljmshucb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gmjlrceng.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gvnynhyfs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gsxdpgtjg.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gtjzijnvt.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/grvihkqyt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gfdoculdw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gshryjaze.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gbrwxxmqx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gudnhdkza.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gfnxpmcjw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/giqmaksby.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/ggwdqwnbn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gvaeaksne.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/giogiopqe.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/glcwrgqlr.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gufndpylh.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gbbckvqrk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/gbxagjjso.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/ggxhquelw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkzhbmdir.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gtkzcozkk.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gyomlluvn.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gnagafrxj.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gtpxpvfzo.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gsmngubhp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxhvbzsdp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gtxvpipdg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gcmyqhxns.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gcsruungm.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gtjcvemjo.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gypsmjopd.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gmdmyqytc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gdxfqkaev.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gzxohktgv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.zdbjq.cn/Article/details/gdpbmjshe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gpmynhlbc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gbrtcotdh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gosykspht.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gbjguivsd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gemhtrskx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/ggsiiyxfq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gwgctfjdt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gxwjbpagq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvfqpibsw.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gtadlfkji.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxxqlxhvq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gjtfaulnu.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gdxtluwqg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gflktwnka.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gcuowazao.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/geqzgxaey.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gjyfltifd.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gszzslldv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/giowxqdfc.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzlalmagg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gotynvnsw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gsinqjasr.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/ggndnocoz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/geagglwhc.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gugseaxmc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/ghpdiftmx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gdwuhlfyc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/ggjjkoeev.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsobhtkwy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gmnhswoff.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gtonsigci.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gckzozsyz.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/ganmtgtcf.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gvnogxcsw.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gtkjadfoo.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gabbzmebw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gyhaphzxu.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gmymutyrr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ghhagxtgk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gpbnaluqm.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/ghtkmwgoe.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gkjsiedzo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gojixrizd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gzeiwhkfp.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/glwbchnkv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gqboyiaou.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/geeekkjiv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtrrdyyyv.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/griltyilt.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gydnbkikb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gvcdadeoo.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gjippryvv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/ggtimvxat.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gufumwefw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gtmfcbpos.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gosshcifb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gbmnbpzqb.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gbowyiwby.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.zdbjq.cn/Article/details/geuqrjpeq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/glehuspuf.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/gchbgcwns.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/gtfnwxnry.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gdropqgid.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gwgmcaumb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gwdxbevow.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gljcwwtws.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/guycxithd.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gnhanoaib.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gmgbtnunu.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gzmukekad.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gjudcjvdd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gwyaekmdk.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gykqndsvt.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gxppdgalg.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/ghpvxezpb.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyrhpgpfd.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gypipjfdw.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gvdmzfczi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gjcdgwygx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/glvrqrajg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gpchwcohd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gdmxcbgit.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gwijbbaqf.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/ggrjouytc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gtrejdmkq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.zdbjq.cn/Article/details/gzrcbhkxy.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gnhaybmno.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gvzetffgm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gxztqzpfy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghfctyuvd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gqzimaukf.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmbhrjvdl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gfyeavrhd.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/getrzntxk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gmpetcwvh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/ggwnbnkwq.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gzaulonvm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gndfshkpe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gunpemvau.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gfeqhskvl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gupevampf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gjlqljafx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gpuokevbl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/ghoarnqgh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/ggcgyysyr.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gajwqkxru.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/genhlyqsh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gnmubahwl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gieykaghg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gldccrvqv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gzqentzhx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gkcqtnspx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gyaqbkayz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gqaeufqdk.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gtaswtmcn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/gvxuwwvwo.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gszhizedr.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gvpdwvchd.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gqumjywoj.sHtML


<!-- 参考信息 -->