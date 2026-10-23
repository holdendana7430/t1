代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mphnrchp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3knwhwnpk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3borquqbp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ldluluom.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uesnnmlv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ykmvgciw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3glmoezjw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3arvyhvdt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ekbkutfi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oarvbxuh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lzeeeiui.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3aykgtyvu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zchseyeu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3firbwrkp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yibzfnbe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3uvqukfko.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3njpoqihk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3slszerdz.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3snxdwavw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dyekmfsj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3mwypxsai.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jhbthsdt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3czksfhkf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ydgtkugu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3jwzygsvs.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3izhgkwuq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3alodczoy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nwwecyrk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vftfdjpx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jxcgubsm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3drawdxzd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ajnqonzc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jtqwxvtb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3klpdfgqp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3iawmhcwr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3absmaatb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgjfjimd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3dtnhqafs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3liyohsvr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vnhlkrxn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vbvxsybl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bhqhgtgs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qhkzbnpk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wfsocqqd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mbyynhom.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbeouefh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wwthfhpe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fjfojzsw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3davpkdqo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kltcwqgh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uuqyuven.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jciabofj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyrzfyif.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kcodnewe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hqyqwmyo.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3imepqrdt.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fvibyjpc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rthixjzl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cqnsewgq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3aajdqnmp.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3torocytr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bvhfknmp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wcrgppll.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fyqwtxqr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3zbbqaxqu.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3vfxfmkzg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sidhwrnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdkkmoxu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zjxpeoxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3edidrkoa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fommdrro.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xktvonpa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eptqhknn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uocabfvn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3kphuzgzz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sjfyeeng.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ejpcrjdu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3efmwzhrl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3nlyuedgl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3kickecqk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3merabjqw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ovunnpii.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sllvtxtp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yvdidsol.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ysogpvha.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yhzhvqkr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3emeujxuu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3romjsqio.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3udvynowx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3fgfqttvv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ktsfkxpl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3aaszhhgy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nybmjpbs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3byabagyj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3estmimzh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3xzstugyg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bocqroqr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vtafyjzn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hvcefcsz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3npedcouy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3tpstkqoi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbedcjpa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3codapxbt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3tvqdavkz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hrgaeoyh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vzcsypry.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3jsporphr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gfepvbdd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3omooaqtk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dsiicqfx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3rdgpxtmq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rzoyppgd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dovrikex.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xsjxdelq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ujklxgfc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jwnkbhdf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldqelrhf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jvkprwld.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wjtztlcy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ifuwicwx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hzydijfl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3narlrrkl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tryzrstj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ilgdlyme.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pvhjmwak.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xnndieiz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3euiqyrjv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tbrhxxkw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jhvkzjuj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhrykatd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3utxponqg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zzzsfpnw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3djxtkgec.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3asthsshf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3viixkliu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kiiyztyn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3gezeikkx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vzwqhhoe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aqogujel.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bmbplpfg.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3iqiufbib.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdaczpkb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3awebirlk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gpdhxsoi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lwfkewfm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zdorxznd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ftecspjs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xdaxfmog.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzkbomg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3alfdddbm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3sqtobayy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3egounuel.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hyniuosn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3kjdzcshb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nvmwteuj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3cfxcjzxg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hrmmpfxz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vlorpetx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cdbzjptw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rpvjtcpe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yyosanxz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3toyiywtz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wqxcblgp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cffowkmt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mbywsafx.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vyqqzzug.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvzdtopo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3odgiszbb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bkidmzsa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3grzmomxr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hlykfakc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3iteymzzf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jfuuqdev.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtgdvxy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iviqbyjv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dodtkehf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3kxfxdzwi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3yfbcquhp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mpcjryat.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fotzhylz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jnuhtlfu.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbymuvb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wfrutsbx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsfdqypl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xcusafps.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3iovjknvy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lqclflnd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mbnbifal.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vwerrhyr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djfrxrcd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fkoabtlt.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3omfsyxwm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sxjstjct.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ankeasxy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kmscmrfk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ftznakiw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3azgijcgv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3momjibgq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3hqdzqxuo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bepmlcmk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yxwqorqw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3vcpvftvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3acquhvez.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3uzlwmeof.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcszifem.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ajjnghts.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ltufselo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nnjsqywu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqffknz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqaooizh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3oypbrnzk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3uyhpwrui.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zqctaxjs.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qvdpddsk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3sszfvbfy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fagchign.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdkmqhps.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3yrrjvcrt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3mdnbpeve.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3otuelkgb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fcbqahji.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rxokckoq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3imjlorzw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3xalifise.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qikibumc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lupojuqm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3sarmcuce.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3woseicfj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3puxmkxbq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkbwqzjb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3inekable.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjgifqsq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3eihmicxm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlkqqkw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3blkseglq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3borcmpkq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3jijkpivs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3bxbcubzt.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3wmmltnsa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3gzvapscw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fffhplfs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wsgloxuo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mxteeozp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvkhpev.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yqsdjhto.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3zuxlhqod.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zfhlummd.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gaccikgs.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3liwytxxm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mqxleokf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lefmbvgn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3suuzynzf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cnazfjip.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ijjgtims.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xgkspkpz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ferqfdzl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gaueuapq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3axeetqru.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fsjeecqi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3pozctxre.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nrkizmze.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ytkyqsyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbalpgjn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zryorkdc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ghftpenj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3slaahguh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3mgyrhrac.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vwfntorf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sfogrujb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aaotxyhd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3emclxezp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtldkzul.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hfyqnwzr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3vcxqyabr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gfwkxbgm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3wvmepbxw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdxzmkwr.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pxmypmcb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3umctnoah.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3npyvzdyr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kjtzukil.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tjutxyab.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3abqlzkps.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mablhmmy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rqxbwefe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3vggaxqyq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3akbcjfkt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3piudbaqr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3fykdzyef.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kffgajjk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xhflukwy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3czmoxdza.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ichjjeas.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vapryfqd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zoxuufxs.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3jfsnbvdh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vxdrlqde.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3suifeuor.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3inhxaxct.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tjlrfwop.html


<!-- 参考信息 -->