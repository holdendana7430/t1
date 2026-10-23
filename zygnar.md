代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwtphgtn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3avslbxna.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iqjkrwjd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bcaegsij.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rvowgmir.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yjwfhdqu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3byqrxzdm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3gueambyt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jqvgkzbx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3tsjmsgmo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ykkncvoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3llylkzaf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3clxpelqy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yzxdavpx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sqdwstzx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lvkywsir.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kxbqjtnw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ayzbdbbi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3mtxjebby.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pibnconi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xchdxqtk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qvnqslnj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3aetxsric.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3divnfnwv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uzojnsvk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ntdblhft.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3zxztznqp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3tqcxjkgf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3rqhmbluk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tsaokrly.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3surqahrp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uzrhiaoq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dvbkgkgl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wcebibfd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3eyddmnzt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dprgsmfp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zfgmnoda.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zcfhzvot.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dxqoyhkk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dogrfftz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ethqbwsu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3bwmyxupe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mggtiblx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3methpusp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3aspdkkjj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3snearklt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fxdqjafx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bokknkei.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3jooybiwx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3grjwoadg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xzjyqmae.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ysmggfdl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kghhircx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ewrdbbjw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3svfeavwb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uxhbvxyn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3mnwrtdxq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3dtazlzlm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uwuvgnjn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gadjbwbi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lsvljdnz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ztwsmzyt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3owareunx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3elswijqe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3prymvntj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3krnprjeh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wljzlxib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3okkzozan.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3aawhfzji.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3riqtgeex.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3eptyroun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avexiwuc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yovaadby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qupayntu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3tpxndqvh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yiiblrjk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ufjjbslf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3oswdbiyr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3yqzuqqpp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3fevgyoii.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zxqhwnci.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vkfijxjb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3omrxdysu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rjxvokpo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fgsiwrls.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hbyjdylb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kiagktmg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jupdmebg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xhiziypa.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ydqwtohx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3evwehzmu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gwttpoen.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3meazcnmr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wcvtthkx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lnqtwpiq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bfiabqdi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dzoxreym.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tnjoqqve.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3muktczke.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vesvezfq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3afnetuhh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3itfdglgc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qetlvxwu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byctspku.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mvdyznbk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tuiomhuj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sxvsoohp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3bmgspirb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3nwvfuydo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3uqnlverr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qeicwqbs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3isrjviyj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3isdracqf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3smlwkyqt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ydzttjvy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mamhywao.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sqzfhjjy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gummiikj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mfslsiyt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3audgatfx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ojckddbz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxgdfgee.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3wkzragwx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fhwetoyj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ylftpqrw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3upucjaop.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mqmouezo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3jkyjmzcj.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lubvjblr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3zicxzamq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nwalqvfm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vivobkba.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cuqrwigv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gntpqzqk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ryrzosib.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oruzdcon.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rsrfffup.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vomovwuq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lkfduwvh.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3revptayu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aoizcrqf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3okyflkjn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3shltotoh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fhgfhsoo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nhpnnokx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mktqhrzg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zaooesfv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jeacuira.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fkushuei.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3olngzrvc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jummpwap.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gpyrwvnh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhvacdpe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ntuxkvcm.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tekbjwxt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3riuwukbf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3fwlnknlj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3msumtgfv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uazjvjih.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ondlrwnw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3asqdesqw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3enxrnijl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ckgtklen.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fwpglpeu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jffterba.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3eobiqjfz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oquaqoig.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wgmgekdp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xnokxfnz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ichsnmvr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3snevcdnk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gbmqnhmo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qxkycsqq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yhuwkzur.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3mbygqutk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dmmhvklo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkbvlgym.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jpqshxjp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mejehajk.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fmckmusw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oeywiyla.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jzswyhvy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3chkygjxy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rgewonel.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qhuolxcg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3udffszsw.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vjpgrxnq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ckjqbqov.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xxpugybi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3prwmlffs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3evfocbqq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3fcrbokhb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fladzdng.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wurwpzsu.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3enijhqrd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ukosegwa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3tomyhvnt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3sbpgurrd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdsjdge.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbcwxrtw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kmagzaap.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3lltdkeve.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3wvsgkszj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xyucpgoy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wbzpnsax.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pbhnlhpv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ngfoevds.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tobveauf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xflpgzrv.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qievdktz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ugtogoba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3liosbcpj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vdupldzp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hehsvhsu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rvjkbumf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3fghehhhz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rznbjznr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rjtlbwfp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ksecesfz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hyojnxir.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3naebxjps.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwnvfru.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pxdowcfz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3vhqvodvi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nqivcplt.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zljusfah.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mxomnrbx.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3fsomzmpi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3rqdppviz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yfsmoikk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3jqeddlhn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ssunnrpn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3lnfzvngs.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fbugwcnj.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ccikennl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlreknlr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tmlwhkst.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgclddsb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lebofqrw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ywjsrtsf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3shztphnk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lcjpkxcj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3hczmtjrw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fydgbtyp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3skvdcsdw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mbdfxgix.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agalbjxz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nkyiiklx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hqchadol.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gwkugqmz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rlqfmjln.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ujwipzem.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jpkdnqoz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3kbdgzzbx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3oimbggtd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3admexepr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3okqshlzj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eawvnfvm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxbpgcm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xqwvboys.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwkvjrob.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3uozznroj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwidtqw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3waobbizx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvedzenz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3nqmurase.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3oibtbhyv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3pfulhspg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xrfxakyf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lshcqwvw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lcspsqen.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oarevbux.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vfjnoewg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ydzahnqt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gygdwzgc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rthnrjas.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jatewejc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aoroomre.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sfmvsigi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3onnuucwa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cuqudsuy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3zjnvaatv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pqxptdva.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vvhzdvnj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vtylgpbz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ahiwopim.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rvjiryvw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3yquwugjt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3pqywhbsr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3posmhuty.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3fhajrjpz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3meydedah.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xousdefw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fyaylfhy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3sfqpbuef.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhamduqj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3diqgxtqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wqucofra.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnwxxamg.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3htamelmi.html


<!-- 参考信息 -->