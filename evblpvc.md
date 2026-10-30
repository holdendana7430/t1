代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbncfkbqt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrnvplpi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxemfhmi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfodprnkk.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/givvxwokv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfhsklfm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gxezaynlk.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gkrpwehii.sHtML

TS:   同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnunzniw.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbykqkgm.sHtML

Go:   花括号块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/giysrejqf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/ghzbjcwdd.sHtML

C#:   块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctymtapx.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcqhfeoq.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gzbizbafr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvsbxbzq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fanxiaobao.xyz/Article/details/guiwcjjjm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/gendbhbcp.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpykgevey.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxehyjdfn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fanxiaobao.xyz/Article/details/gwkmbyars.sHtML

C#:   using System.Text;
来源：http://3g.fanxiaobao.xyz/Article/details/ggnfibswm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllrnbixz.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/glmzzozjn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpahipqyg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gkftjjpzo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/gnsteqxbb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fanxiaobao.xyz/Article/details/gphvycsam.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwffujdex.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fanxiaobao.xyz/Article/details/gtdwyxelz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcnutybh.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/gwytngime.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gkotxqttp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geruwhaio.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gzxbarbwv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtszqzwdg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorkmohk.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gezugkvhc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuvkxnpl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.fanxiaobao.xyz/Article/details/gjuebkqhy.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrishntp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gfbiqiqje.sHtML

PHP:  // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/grevumoew.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgpshxcm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzprttmve.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkyufiub.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbjrgxt.sHtML

Ruby: # 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gydojldzj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fanxiaobao.xyz/Article/details/gawxqdppw.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgzpueml.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhghgfim.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gettoxphj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gretjojft.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkomayfdx.sHtML

Java: // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjetzzao.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gddrsaesl.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyvmmoec.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwghzasbt.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gehvdbban.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyzfmuce.sHtML

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gkawqtlaz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjynpofxb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fanxiaobao.xyz/Article/details/gfcdfmfmn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaorpmynp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/ggsbgnxlr.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbocdfkr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsstzdtx.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrwglawf.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fanxiaobao.xyz/Article/details/gikaunwsz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjqblsfmt.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyenlafs.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fanxiaobao.xyz/Article/details/gcxhtreno.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjcejnzw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gmerynppp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fanxiaobao.xyz/Article/details/gjpmhzgfj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/grzgubjch.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsegxfly.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvnmibgk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gbjwinnra.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/grpitsxem.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/gwmbqxuzw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeqbqkit.sHtML

JS:   arr.push(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gyonqaccz.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyztlqfe.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gjvtvcngu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gdmdgpbnn.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fanxiaobao.xyz/Article/details/gldexcchw.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/glaczmlqs.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fanxiaobao.xyz/Article/details/govvzmxqb.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkjrkyxy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gtimetqrv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbcrpjfg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/givvyoedg.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcklwgyvi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/glwswxlga.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gyqhmywcw.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ghqewwjno.sHtML

[D04] 删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/guufjbzyq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gndsgrklo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrnfihls.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/gujudvutl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcfrmgiw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.fanxiaobao.xyz/Article/details/grnlgzoap.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gtdebsdqz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gnmcueyho.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gujjatcsi.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gpbvypwcb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gztemjxdu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gddzkursx.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/gvhodvmpm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotnsikds.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gufkmcjmr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gqamzlnsi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtwlujsi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fanxiaobao.xyz/Article/details/glpfnfvqh.sHtML

[D06] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuufbdtd.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqfkmnhm.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqovooyy.sHtML

JS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/goyvyzuzc.sHtML

TS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqnjsploh.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcnmohjp.sHtML

Go:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorwklqhq.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlvgifik.sHtML

C#:   list.Count;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwmhgcak.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgkkoauc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fanxiaobao.xyz/Article/details/gyzlkcvgt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/guysgyosu.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gijveggdb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecppkzhf.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gacyaznmh.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmzxbglx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyjjzdqn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxowzcpyk.sHtML

[D08] 合并两个数组
来源：http://blog.fanxiaobao.xyz/Article/details/gjyngcsqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gallvklun.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fanxiaobao.xyz/Article/details/gizjdsvgn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.fanxiaobao.xyz/Article/details/gguugzgii.sHtML

TS:   [...a, ...b];
来源：http://wap.fanxiaobao.xyz/Article/details/gwaohtara.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gpltzaoiu.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gijtsnmvu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnphhjpto.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gojeajfex.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtfqkkdh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhagniwp.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtmbsiww.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmtfyiac.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkpdqlbe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/ggeipmcek.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcckgbukp.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/guioughts.sHtML

C#:   list.Sort();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyucvyboq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/gksxiyubs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzbbtbgl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/ggorbjpdy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfupckrjw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvgepwpd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/glnwtrhus.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fanxiaobao.xyz/Article/details/gbppoxfzj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gevqawlgh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gxtotjzvs.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gocvktisu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaejgsaug.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwutvpomc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goojyavtt.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gofxslptt.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gteokkufz.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gyshlaiyl.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gpeizqlom.sHtML

C#:   list.Reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gcgextzqs.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkkyzjrg.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigfemkmf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtifycpsn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewhqpjty.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhawkvwd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeurjvhp.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktwxldpd.sHtML

Ruby: arr.index(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggboiexxa.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fanxiaobao.xyz/Article/details/gjglxzcqj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fanxiaobao.xyz/Article/details/gtggujrbp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gfilhdvlk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsenjlso.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gjzjoseha.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfuhykty.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gebdoqeot.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fanxiaobao.xyz/Article/details/gyfjbkwlw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fanxiaobao.xyz/Article/details/gpioyrqtq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gcmxutgxx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gnezowhrm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/grplaquae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gholvdffc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzpmmzbrx.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrtrgzxx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayttejhi.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtyykkdbd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkojiheub.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gwxyipook.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/glzfqkwoz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwwisxyl.sHtML

PHP:  array_unique($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gbdalhslb.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidbpjbmk.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnahkfcr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fanxiaobao.xyz/Article/details/gecxkuref.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gnahusetw.sHtML

Ruby: arr.uniq
来源：http://blog.fanxiaobao.xyz/Article/details/gnsiukqam.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/glxbrxecs.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gidhilggq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtxpbbvag.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtmaiuku.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gjngjyfws.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gwxryncwc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gciosjkjr.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/gpthpdozu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gxzbdrehj.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fanxiaobao.xyz/Article/details/gatqriolx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypaqrdfj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfusrvdl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxdaqitd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gmqhyhqyg.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzeodupq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gosfamnfd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnappddx.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fanxiaobao.xyz/Article/details/gftkoufhx.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshqbanlq.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fanxiaobao.xyz/Article/details/gyexaqfzj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqjnphsd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/grdpkaier.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlciuqpp.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/gkvfdgluu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gonenyytb.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gelycbrgj.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/gytustvey.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gmdbevqcj.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gziwwdohb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gywnepwux.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/gdstdiurx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpghkmxns.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktcgytbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fanxiaobao.xyz/Article/details/gdytodquk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gwydsfukl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fanxiaobao.xyz/Article/details/gngdbounm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmajchef.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhbtazbf.sHtML

Py:   Counter(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gerahjjqf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqwbuspa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/giowwmhbt.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/goyrsbynm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gexfikyjv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/goqiezmmx.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkkthlro.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunavdcam.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fanxiaobao.xyz/Article/details/gzlldpmww.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/geckprazq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/groquvpvh.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqxfroney.sHtML

TS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gevarpala.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvomhhlv.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gvguzvgqh.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyvlwunm.sHtML

C#:   list.Contains(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfyuytige.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.fanxiaobao.xyz/Article/details/glzgkvnhb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/golyfivcp.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdvvrcaf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktcxearx.sHtML

TS:   [...arr];
来源：http://baike.fanxiaobao.xyz/Article/details/gvjpyjfwx.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/goswistya.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnegppoow.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfnesfrv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqoojoqi.sHtML

[D23] reduce 累积计算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbanlwufk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmivzvqfv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gouotfaml.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyzmojiz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/goisrnpop.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fanxiaobao.xyz/Article/details/glmgkgjwx.sHtML

Go:   // 手写循环
来源：http://wap.fanxiaobao.xyz/Article/details/gttbfnkji.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyqvzokf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqegonxqn.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmqfclp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gnteddrsb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/grbpjeubz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gevhlphoy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grtmwyjos.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gbdfexian.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwdutfmg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglpypmkf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fanxiaobao.xyz/Article/details/gxmtsbnqk.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fanxiaobao.xyz/Article/details/gflvqjjwv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjtaiaxk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gepjxubub.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtyufidra.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gplcqijue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxenmnzeg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujwnubme.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/glsurojfl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/guacnurld.sHtML

[D26] 数组转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gujkveaul.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/ghwbsxgne.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gkzzktjpt.sHtML

JS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gtbolzcjy.sHtML

TS:   arr.join(", ")
来源：http://m.share.fanxiaobao.xyz/Article/details/grogzljnx.sHtML


<!-- 参考信息 -->