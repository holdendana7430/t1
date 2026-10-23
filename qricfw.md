代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezcqktjo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lcwjdrdt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fnsvride.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3odxlxxhz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ulsqbbgk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3otwxovrg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3bwhmvqls.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3yewcksff.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jhyfksks.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xiukchct.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yjbrcbvm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3djoursqn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxwstfvp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3rommazvf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gmusqbpe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bziqaals.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pzigjgxk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hcwvkufr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jwlalmmc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3jyqowwqi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3plzigkmh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xporzbvl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eaeossic.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3gttexawx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3sklvcknv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dpjojskf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zdnnwcwa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3yjjnqanp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3igpkgyhl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ruikzuja.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kfcaxqfd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3zhcmrgrr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tremqbue.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3iwwlhryb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3bvmkoauq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofdvtqny.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3awuywgxl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nzrsbmwy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pnueyxgk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3lzozdtrj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3ngoukinz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ywwecbjs.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ebuabubw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ntocggmm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrykgobv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuawnxnn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3vdwoyzhk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gxqaevax.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3aolukeut.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3oarqdjmq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wryxvhsv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3eneoikoe.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ultoojoy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnunfamj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dekxhrht.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rplappiz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3eomuekre.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3spwhynqy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uhxlylte.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3awhniijs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3efkoglyf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tejdemjd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlfpwh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3hluadejd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3blqyzqmk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ghhluwlj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzkpltvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gcinwdkl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ffjarzjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zeztuesp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vqhgstbb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3swbkbkzy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dsyeapas.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qhkntswy.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dhmdpejf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ovehhisf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vwnmflfu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3kcxkugdn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3muvytnov.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3yukvhjpt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wkdankfz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bpxwpasd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tglrqral.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qiuilkvp.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vzgkebhc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjwvvuo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3dmlbhkvu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hthcvvds.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fnazexne.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3szdqxxoi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hucctrpr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3hmmbayex.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lewumyhn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vewbpksr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hxrxcign.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsfxxayv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mtydonkb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3aozkkscl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3njntyuqg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihgwsrgk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kjdkgsfk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bjngtpwh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lwmyxzoq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jdjculbu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3haivybah.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3sfzvwjsk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3dauchwlw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jgrjvaby.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3omfayxsp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3umkwusdc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3srmxgujd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xpujkqes.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nmupjbtt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dspsqoyz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kgbszfyr.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dhaaxexc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzliitol.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uedplivt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zbthrlmh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ooljfklp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3gmyybwni.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3knmmwsdc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pgunwgpf.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nrxjtoyg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3auckjjsm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3fbpcjfnd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3myufjrxn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cegxvlqu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rpspaxwh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3legapapf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3obwpwtyx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cuibelvk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3znpviapc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ozyttuas.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqdmpch.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kejxmkev.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3taajzcav.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3mkulvqdf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vnzwdgel.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3xknzufdt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3epjygvuk.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jdewhuse.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3npscgoqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pkjgqaoh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gccunyal.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fsternwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hyaadwgu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uspjnaqp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxamjpr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wdubpfwm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xkirfddk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3wnpeoiki.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zoygudih.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rszhezme.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3aspasixj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3czehmkjq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ioljtxix.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nvarpveo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3clnuosdq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ohryfqjx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3bqsusqvr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ixhsdszx.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rjcosnyg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3trijhhew.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hneesslt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ygfgghda.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfvtfkru.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3psycklto.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3cxsdgmly.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3kdmdewud.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rpurrgvm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gjusgbvj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ibewdbhn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3casyhrsz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lbrhljqk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qsavfjsg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtkyahic.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kdoihjpd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3rmwpuevz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mnizfonl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3sbfgdcpn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhxvhcp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jubcccpd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3csieywnz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bwqepalg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bypwyiik.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nheighlb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wtmnbqdd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ihlfvxua.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vweahttz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3imagwyhx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qppaycie.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuzqafwq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yuhcfswi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqszpcxo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cekpqtyx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ontwbfue.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dnhhbphs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bhkmmxhl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jcijifoc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3inraiepo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bgebuxpa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3eiyssmmu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3dmdpybwf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lhkgwosh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kgyuibza.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzbeluds.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rnufxeos.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tzwgvoao.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cafwxtrs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ivrdsjfx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3gncozrgl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rmtyfbwc.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3zavinvzc.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3crgvuixj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydgcgpfb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nvphicrw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3jkekpuwl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3chkfrkhx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3syinzruh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwurenda.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dqcqcnia.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yalbflmy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3urnmlujl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3alfbyrod.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3mddsmhqf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ushnjjgn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3omizqtlx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tktzdtbh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jwnrdizr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dwugzeow.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3twxpgjhf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pvnaykpd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzcfztbh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jxycokqt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ovnsbhgf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rsofecdf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gajlyqri.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3shqgjajv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rvxlioxt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gtbegnav.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hoiqgeun.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blwafkwk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3limcygbp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gbjshail.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jndptjej.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lnbdjcnk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3wniwtjod.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3lbbkojnv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ladgvlka.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3caehdnal.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3rdskmyyp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3jxgrwgcf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtohyfs.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtqzqnv.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzeqmpiz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtiicgtx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrnvosbw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eeztydap.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ioellwws.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3earbcpao.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3llzsswgz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snbtxnww.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3cytbeboy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3voyrllnn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vacpxtqi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xwnxsesh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3onypblzh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lzgumesq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uvdnpjop.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3itrfmazx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nkynqckd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kwlqbhns.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bpzfyefx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nuymckwo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3spoqjvje.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdjxwto.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3syyibfzt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lxbihzpb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nfaoyrwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3laxihqkt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kgxbtqil.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xlgwplyv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3syyawigc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rvfeuhvc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3wurqnmmu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dljoegsm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xrekbrly.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gjsayraq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3pecguinl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ptdryoxm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kzzzjcci.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ypdcyqap.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3bjnpszpx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahmcfdvh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vjobuyan.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3inspvdvl.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exqerjej.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cafojito.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jawwdvzv.html


<!-- 参考信息 -->